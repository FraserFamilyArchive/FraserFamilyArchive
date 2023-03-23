{% assign imagesample = site.data[site.metadata] | where_exp: 'item','item.format contains "image"' | first %}
{% capture imagesampleid %}{{imagesample.objectid | default: "https://www.lib.uidaho.edu/collectionbuilder/demo-objects/mg101_b6_photographs_01.jpg"}}{% endcapture %}
{% assign pdfsample = site.data[site.metadata] | where_exp: 'item','item.format contains "pdf"' | first %}
{% capture pdfsampleid %}{{pdfsample.objectid | default: "https://digital.lib.uidaho.edu/utils/getfile/collection/ui_ep/id/21768/filename/uiext21768.pdf"}}{% endcapture %}
{% assign videosample = site.data[site.metadata] | where_exp: 'item','item.format contains "video"' | first %}
{% capture videosampleid %}{{videosample.objectid | default: "https://cdil.lib.uidaho.edu/storying-extinction/objects/trailcams/videos/ballcreek-cedarrub-birdonpath.mp4"}}{% endcapture %}
{% assign audiosample = site.data[site.metadata] | where_exp: 'item','item.format contains "audio"' | first %}
{% capture audiosampleid %}{{audiosample.objectid | default: "https://www.lib.uidaho.edu/digital/mp3s/Clouds.mp3"}}{% endcapture %}

## About the About Page

We want to make engaging interpretive pages easier to create, so CollectionBuilder gives you tools to write *with* your collection content!

The template comes with a customizable "About" page layout designed for long form content with rich media embeds.
Content is written in [Markdown](https://guides.github.com/features/mastering-markdown/) and enhanced using "includes" that pull in collection content, external media, and [Bootstrap](https://getbootstrap.com/) features like cards and modals.
We hope this makes it easier for site builders to develop the collection AND add interesting and engaging contextual information. 

Each "include" file has several options, which are documented in the files themselves--copy the examples to see how it works with your content! 
In the demo below, we've given display widths of 25% and 50% to save space, but you can feature the entire image or document.

You can also see a page featuring [a bonanza of feature includes options](https://collectionbuilder.github.io/collectionbuilder-gh/feature_options.html) on our CollectionBuilder-GH demo site. 

{% include feature/button.html text="Feature *Includes* Bonanza page" link="https://collectionbuilder.github.io/collectionbuilder-gh/feature_options.html" color="primary" size="lg" centered=true %}

### Include Collection Items

The template provides includes to pull your collection objects and metadata into your interpretive page, allowing you to write with your materials directly embedded in the content.

#### Include an Image

- Image --> `{% raw %}{% include feature/image.html objectid="demo_001" width="75" %}{% endraw %}`

{% include feature/image.html objectid=imagesampleid width="75" %}

#### Include a PDF

- PDF -- > `{% raw %}{% include feature/pdf.html objectid="demo_002"  width="50" %}{% endraw %}`

{% include feature/pdf.html objectid=pdfsampleid width="50" %}

#### Include a Video

- Video: `{% raw %}{% include feature/video.html objectid="demo_004" %}{% endraw %}`

{% include feature/video.html objectid=videosampleid width="75" %}

#### Include an Audio File

- Audio: `{% raw %}{% include feature/audio.html objectid="demo_003" %}{% endraw %}`

{% include feature/audio.html objectid=audiosampleid  %}

### Include Bootstrap Features

The template also provides includes to make it easier to add [Bootstrap](https://getbootstrap.com/) components to your Markdown writing.
These features allow you to better organize and highlight your content.

#### Include a Card

- Card -- > `{% raw %}{% include feature/card.html header="This is a Card" text="The card features an image from the collection as a cap" objectid="demo004" width="25" centered=true %}{% endraw %}`

{% include feature/card.html header="This is a Card" text="The card features an image from the collection as a cap" objectid="demo_001" width="25" centered=true %}

#### Include a Button 

- Buttons -- > `{% raw %}{% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}{% endraw %}`

{% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" centered=true %}
  
#### Include an Alert

- Alerts -- > `{% raw %}{% include feature/alert.html text="this is an *alert* that 'warns' a user" color="warning" align="center" %}{% endraw %}`

{% include feature/alert.html text="This is an *alert* that 'warns' a user with centrally aligned text." color="warning" align="center"  %}

#### Include a Modal

- Modals -- > `{% raw %}{% include feature/modal.html button="This is a modal using a 'primary' colored button to invite clicking" title="when clicked:" text="A Modal will pop out a box with some more information" color="primary"  %}{% endraw %}`

{% include feature/modal.html button="This is a modal using a 'primary' colored button to invite clicking" title="When clicked:" text="A Modal will pop out a box with some more information" color="primary"  %} 


## Controlled Vocabulary and Tag Descriptions

This is the tag description list. It contains the authorized headings for name forms and spellings used in the database as tags. It also contains compiled and external information and explanations for the people, locations, and photo sets represented in the archive. Note that this lists tags in alphabetical order, so names will be alphabetical by first name. 

#### Alex Fraser Buie
{% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}

#### Alexander Thomas Fraser
Born August 5, 1879 in East River St. Mary’s, Nova Scotia. He married Helen May Stuart on August 21, 1912. 
His children were Hugh Stuart Fraser, Helen Wilson nee Fraser, Ruth Nelson nee Fraser, and Alexander Colin 
Fraser. He was an engineer (see Alexander Thomas Fraser - Bridges and Buildings). He died in July 1965 in 
Leduc, Alberta. 
{% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Alexander Thomas Fraser - Bridges and Buildings
Alex Fraser worked as an engineer on many locations around Alberta. He was the engineer for the Alberta Legislature Building, the Drumheller Bridge, and more.
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Alice Louise Horwood nee Toone
Born April 8, 1874 in South Wigston England. She married Joseph Ernest Horwood at age 27 on July 10, 1901. Her half-brothers were James Henry “Harry” Towlson and George Toone. She had another brother who died at age 2. Her children were Alice Ruth Hollingworth nee Horwood, David Ernest Horwood, and Esther Alberta Louise Fraser nee Horwood. She died June 22, 1954 in Westlock, Alberta. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Alice Ruth Hollingsworth nee Horwood
Born June 2 1902 in South Wigston, England to Joseph Ernest Horwood and Alice Louise Horwood nee Toone. She married Frank Hollingsorth. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Benjamin Toone Snr.
He owned a boot factory, making boots at first by hand. Later in partnership with Black, they marketed Little Duke shoes. Hudson Bay stores in Edmonton sold them. According to the Wigston Historical Society, the location of his factory was what is now the Jasmine Court on Saffron Road, Wigston. He died 1907 and is buried in South Wigston, Leicester, England. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Certificates
Certificates of birth, death, or marriage. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### David Henry Ernest Horwood
Born September 20, 1903 in South Wigston, England to Joseph Ernest Horwood and Alice Louise Horwood nee Toone. He married Doris Reid, and died May 15, 1984 in Toronto, Ontario. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Edgar Horwood
His brother was Earnest Horwood. As a young man he moved from England to Johannesburg in Africa.
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Edna Stuart
 Born in 1885 to William Stuart Snr. and Emily Stuart nee Grey. She married Hanford, and died in 1961. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
 
#### Emily Stuart Jr. 
Born in 1878 to William Stuart Snr. and Emily Stuart nee Grey, she married Blake and they had two children. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Emily Stuart nee Grey
Born in 1857 to Robert Grey and Mah Grey nee Lonet, she married William Stuart Snr. and their children were Emily Stuart Jr., William Stuart Jr., Edna Stuart, Helen May Fraser nee Stuart, Frank A. Stuart, and Robert B Stuart. She died in 1932. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Esther Alberta Louise Fraser nee Horwood
Born May 5, 1912 in Edmonton, Alberta to Joseph Ernest Horwood and Alice Louise Horwood nee Toone. She married Hugh Stuart Fraser on December 24, 1936 in the Allendale Baptist Church in Edmonton. Her children were Stuart David Fraser, Alice May Mitchell nee Fraser, Gordon Douglas Fraser, Ruth Joan Midgett nee Fraser, and Alexander Ronald Fraser. She died September 14, 2000 in Westlock, Alberta. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Frank A. Stuart
Born in 1889 to William Stuart Snr. and Emily Stuart nee Grey, he died in 1956. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### George Toone
His half-sister was Alice Louise Horwood nee Toone. He never married. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Helen May Stuart
Born in 1887 to William Stuart Snr. and Emily Stuart nee Grey. She died in 1965.
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### James Henry “Harry” Towlson
Born 1865 and died May 17, 1883. He was half-brother to Alice Louise Horwood nee Toone [WAS HE FULL BROTHERS TO GEORGE TOONE?] He was an artist. He was of the Manor House in Barkby, England, and was buried in Syston Cemetery. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Joseph Ernest Horwood
Born January 21, 1874 in London England, he married Alice Louise Horwood nee Toone on July 10, 1901.Their children were Alice Ruth Hollingsworth nee Horwood, David Ernest Horwood, and Esther Alberta Louise Fraser nee Horwood. As a young man he left London and became a diamond miner in South Africa. He then was a soldier, receiving a medal from Queen Victoria in 1896. He received the medal for enforcing British Colonialism on the Matabele people in Rhodesia. The story goes that after his service, he came to Canada in 1903 having bought land in BC. When he arrived, the land was flooded so he instead moved to Wetaskiwin, Alberta, also in 1903. He went by ox team to Wavy Lake where he became postmaster. His wife and children came over after him in the fall of 1903. He also worked at a power plant, and ended up in charge of the CPR stockyards in South Edmonton. He died December 1, 1946 in Edmonton, Alberta, and was buried with his wife in Mount Pleasant Cemetery (Edmonton) in Section 0F, Block 0335, Plot 0001. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Newspaper Clippings
Items with this tag are scans or photos of published newspaper articles regarding members of the family. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Portraits
Images with this tag contain identifiable photos of a person’s face. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Robert B. Stuart
Born in 1883 to William Stuart Snr. and Emily Stuart nee Grey. He married Marion Ferrie Stuart nee Hodge. They had 3 children, including Doris Marion Donner nee Stuart. He died in 1955. Him and Marion are buried together in the Innisfail Cemetery. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Significant Locations
Homes, schools, buildings, and other locations of importance to family history. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### Unidentified Persons
Images with this tag contain people who have been categorized as being family members, but who are not yet identified in the record. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### William Stuart Jr. 
Born in 1882 to William Stuart Snr. and Emily Stuart nee Grey, he married a woman named Lillian. He died in 1953. 
 {% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
  
#### William Stuart Sr. 
Born in 1855 to Alexander Stuart Snr. and Jemma C Stuart nee Kellie, he married Emily Stuart nee Grey, and they had Emily Stuart Jr., William Stuart Jr., Edna Stuart, Helen May Fraser nee Stuart, Frank A. Stuart, and Robert B. Stuart. He died in 1919. 
{% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}
