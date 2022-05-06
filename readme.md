# Data Modelling Challenge: Event sourcing, state updates, querying

_This case is based on a real life friend. Dates and names were changed so we can stay friends._

Alice is a friend of my wife that I hear a lot about. She's created the most interesting family
and over the last few months I've been piecing together the basic facts of her life.
I'd like to put all this information which is coming up out of order in casual conversation
into a data structure that will allow me to continue to make updates as I learn the soapy details
and make queries about such an interesting family. The schema should abstract and scale up to describe any family.

Facts learned
Alice married Bob in 2010.
Alice and Bob had Clara in 2011.
Alice and Bob had Damon in 2012.
Alice divorced Bob in 2013.
Alice married Oscar in 2016.
Oscar had been married to Paula since 2007.
Oscar and Paula had Quentin in 2008.
Oscar and Paula had Ronda in 2009.
Oscar divorced Paula in 2015.
Alice and Oscar had Julia in 2014.
Alice and Oscar had Gary in 2015.
Gary died in 2016 in a tragic pancake accident.

Basic Queries
Who are Alice's children? Clara, Damon, Julia, and Gary.
Who are Bob's children? Clara, Damon.
Who are Oscar's children? Quentin, Ronda, Julia, and Gary.
How old will Julia be in 2023? 9
How old will Quentin be in 2023? 15

Intermediate Queries
Who is Oscar's oldest child? Quentin
Who is Alice's youngest child? Gary
Who is Alice's youngest living child? Julia
Who is Julia's youngest sibling? Gary
Who is Julia's oldest sibling? Quentin

Advanced Queries
Who is Julia's oldest sibling who's also a child of Bob? Damon
Was Julia born out of wedlock? Yes
Are Quentin and Julia blood relatives? Yes
Are Clara and Quentin blood relatives? No
What should Alice do after she finds out that Quentin allegedly molested Julia? Out of scope
