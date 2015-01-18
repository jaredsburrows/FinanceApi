FinanceAPI -- BETA
=================

Simple Finance API for viewing stock quotes

 [ ![Status](https://travis-ci.org/jaredsburrows/FinanceApi.svg) ](https://travis-ci.org/jaredsburrows/FinanceApi)

## Usage:

    buildscript {
    	repositories {
    		jcenter()
    	}
    }

    dependencies {
        compile 'burrows.api:finance-core:0.0.1'
    }

## Examples:

    // Create basic Request URL
    String requestURL = RequestURL.Builder()
            .withCompany(Company.YAHOO)        // Set the Company API
            .withFormat(Format.DEFAULT)        // Set the Format for the data returned
            .addQuote("PG")                    // Add a Quote
            .buildURL();


## License:

    Copyright (C) 2015 Finance API by Jared Burrows

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.