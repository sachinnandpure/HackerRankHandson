NewsService
The Service will have a function called getSectionNews().

This function will fetch news list of the selected section, from the NY Times API.

API URL:

url = 'https://api.nytimes.com/svc/topstories/v2/' + sectionName + '.json?api-key=315a5a51483b469a918246dc2753b339'

Action
Implement the following two actions:

LOAD_SECTION_NEWS: Will be dispatched when the user wants to load a new section.
FILTER_SUBSECTION: Will be dispatched when one of the news sub-section is clicked

Reducer: Sections
Implement LOAD_SECTIONS action.
When this action is dispatched, the reducer will return the state having a list of sections.

Reducer: News
This reducer will implement two actions:

LOAD_SECTION_NEWS: This will load news from selected section to newsList in store.
FILTER_SUBSECTION: Sets the value of filter in store.

Selector
This will get the news list and filter from the reducer.
Return a new list of news, based on the selected subsection