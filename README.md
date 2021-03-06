clj-amazon
==========

Clojure wrapper library for Amazon Product Advertising API, forked from code on Clojars by eduardoejp.

## Usage

Leiningen 2 has been used with this project.


    lein deps

    lein repl


And at the REPL...

    (use 'clj-amazon.core)

    (use 'clj-amazon.product-advertising)

    (def ACCESS-KEY "YOUR-ACCESS-KEY-HERE" )

    (def SECRET-KEY "YOUR-SECRET-KEY-HERE" )

    (def ASSOCIATE-ID "YOUR-ASSOCIATE-ID-HERE")

    (def ENDPOINT "ecs.amazonaws.jp")

    (def gibson-opus-search (with-signer (ACCESS-KEY SECRET-KEY ENDPOINT) (item-search :search-index "Books", :keywords "Neuromancer", :associate-tag ASSOCIATE-ID, :condition "New" :response-group "Medium")))


## Reference

You can find more information about the Amazon Product Advertising API on the following web-pages.

"Getting Started Guide"
http://docs.amazonwebservices.com/AWSECommerceService/2011-08-01/GSG/Welcome.html

"Developer Guide"
http://docs.amazonwebservices.com/AWSECommerceService/latest/DG/index.html?Welcome.html


## License

Distributed under the Eclipse Public License, the same as Clojure.
