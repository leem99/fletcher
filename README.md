# Legal Blob

The goal of this project was to use unsupervised natural language processing in order sort all of passed by congress from 1995 until 2017 (104th through 115th congress) and categorize them into human understandable topics. 

The following scripts are included in this repository.

__get_bills_gpo.ipynb__
* Scrape all the laws from the from the [Congressional Publishing Office](https://www.gpo.gov/fdsys/browse/collection.action?collectionCode=PLAW) (GPO) website using BeautifulSoup. 
* Get descriptions (sponsor and originating commitee) from [Congress.gov](Congress.gov)

__generate_all_laws_csv.ipynb__
* Extract the text from all downloaded htm files and append them into a single csv file.

__get_data_from_summary.ipynb__

Go through all of the summary pages obtained from Congress.gov and extract the following summary information.

* Congressional session
* Law title
* Law Number
* Sponsor
* Sponsor party
* sponsor state
* Originating committee(s)
* Link to URL with text

__first_unsupervised_models.ipynb__
* Test the ability of LDA, NMF, and LSA models to sort laws into human interpretable categories.
* Project results of better performing models (NMF and LSA) into 2D space using t-SNE. 

__unsupervised_NMF.ipynb__

__create_custom_stopwords.ipynb__
