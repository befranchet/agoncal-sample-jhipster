# JHipster Samples - autocomplete-combo

Shows how to use [PrimeNG Autocomplete](https://www.primefaces.org/primeng/#/autocomplete) instead of generated JHipster comboboxes.

As a use case, we have contacts that speak one language. So there are 2 entities (`Contact`, `Language`) and a many to one relationship. When creating a contact, the contact form has a combobox for us to select a language. This combobox is declined in several ways:

* no-autocomplete: Bare JHipster application with no extra component nor dependencies. The language combobox in the contact form is the one generated by JHipster
* autocomplete-entity: uses the [PrimeNG Autocomplete](https://www.primefaces.org/primeng/#/autocomplete) component to select a language. In this sample, JHipster generates entities (no DTOs)

The languages are imported via Liquibase. You will find the CSV file `languages.csv` that is imported in the changelog file `99999999999999_loaded_data.xml`

Each example can be executed just by running ` ./mvnw` and going to [http://localhost:8080/#/contact/new]()