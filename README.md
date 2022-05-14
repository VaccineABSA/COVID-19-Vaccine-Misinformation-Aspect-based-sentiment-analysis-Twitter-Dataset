# CoVax-Aspects

A dataset containing 3824 COVID-19 vaccine misinformation aspect annotated tweets from Dec 31, 2020, to Jul 08, 2021. The misinformation labeled tweets, obtained from [15], were annotated for misinformation aspects.  
![VaccineDiagramBERT-Page-1 drawio (1)](https://user-images.githubusercontent.com/102157487/168446338-33e2775f-8f90-4b12-8713-d76793c4542f.png)


The annotation is based on reliable medical resources; Centers for Disease Control and Prevention (CDC) [16], [17].

| **Aspect #1 Vaccine Constituent** | **Aspect #2 Adverse Effects** |
|-------------------------------|---------------------------|
| •	The ingredients of the vaccine are similar to those in many foods – fats, sugars, and salts | •	The vaccine can lead to the development of the coronavirus infection 
| •	The vaccine includes preservatives, tissues (like aborted fetal cells, antibiotics, food proteins, medicines, latex, or metals |  •	The vaccine can cause variants of the virus 
| •	The mRNA vaccine is not considered a vaccine | •	The vaccine causes adverse health conditions such as heart attacks
| •	The mRNA vaccine is gene therapy |  •	The vaccine causes adverse allergic reactions
| •	This vaccine is gene therapy, not an actual vaccine  |  •	The vaccine’s adverse even can lead to death
| •	COVID-19 vaccines authorized for use shed or release their components | •	The vaccine can lead to fainting or passing out
| •	The vaccine contains magnetic materials like metals that make the vaccinated area electromagnetic | •	All events reported to the Vaccine Adverse Event Reporting System (VAERS) are caused by vaccination
| •	The vaccine Contains HIV, Ebola, or Botulism  | •	The reproductive system of both males and females may be negatively impacted 
| •	The vaccine is full of toxic ingredients        | •	The vaccine can lead to a delay in menstrual cycles, painful cramps, and hormonal imbalance                                                      
|                               | •	The vaccine can cause fertility problems in both genders 
|                               | •	People trying to get pregnant should not take the vaccine 
|                               | •	Pregnant females should not take the vaccine
|                               | •	Breastfeeding mothers should not take the vaccine 
|                               |                           |
|                               |                           |
| **Aspect #3 Agenda** | **Aspect #4 Efficacy and Clinical Trials** |
|•	More than the virus, the vaccine is deadly and can kill people, accounting for depopulation | •	The vaccine clinical trials are not complete  
|•	The vaccine fits in a plan to kill certain ethnicities or groups of people | •	The clinical trials compromise science 
|•	The vaccine is a bioweapon | •	The vaccines are not adequately tested 
|•	The vaccine can cause DNA alteration or is part of gene therapy | •	There are no peer-reviews or data to support the efficacy of the vaccine
|•	The vaccine has a microchip embedded within it that may be injected into the body | •	Illegal and unproven vaccine  
|•	The microchip is meant to track patient data | •	The vaccine is fast-tracked, experimental, and liability-free 
|•	The microchip is meant to control the population | •	The vaccine was never tested on humans 
|•	The vaccine affects fertility in a plan for depopulation | • The vaccine is not effective at all 
|                                                            | •	The vaccine cannot prevent sickness or reduce symptoms
|                                                            | •	The vaccine cannot stop or reduce the spread
|                                                            | •	The vaccine is not effective with new variants at all
|                                                            | Human immunity can prevent COVID-19 better than the vaccine

# CSV Dataset Hydration
CoVaxMisinfoAspectAnnotatedDataset.csv contains the IDs of the Tweets and vaccine misinformation aspect annotation. Microsoft Excel changes the format of the Tweet ID to a number, and this causes the IDs to be altered; hence, the hydration will fail or return only a few tweets. Therefore, if you will be using Excel, follow these steps to properly load your CSV data.  

![image](https://user-images.githubusercontent.com/102157487/167255486-7e40181a-2c95-4065-bdd9-689c38007925.png)

![image](https://user-images.githubusercontent.com/102157487/167255494-236676e4-2f38-42e7-8fcc-e4a2f23939cb.png)

To retrieve the text of the tweets and the other attributes including the location and time of the tweet, the dataset needs to be hydrated. 
The link to the hydrator:  https://github.com/DocNow/hydrator 
Add the dataset containing the tweet IDs only. 
![Hydrator](https://user-images.githubusercontent.com/102157487/168446306-e4108ebd-8549-4ee4-89bc-c44fc39c268a.png)

This process will produce a CSV file containing all data attributes. Follow the previous steps for importing the CSV data if you are using Microsoft Excel.  


