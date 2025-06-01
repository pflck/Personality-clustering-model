# Personality-clustering-model

# Dataset
This data was collected (2016-2018) through an interactive on-line personality test.
The personality test was constructed with the "Big-Five Factor Markers" from the IPIP. Participants were informed that their responses would be recorded and used for research at the beginning of the test, and asked to confirm their consent at the end of the test.

The following items were presented on one page and each was rated on a five point scale using radio buttons. The order on page was was EXT1, AGR1, CSN1, EST1, OPN1, EXT2, etc.
The scale was labeled 1=Disagree, 3=Neutral, 5=Agree

### Big Five Items

#### Extraversion (EXT)

* EXT1: I am the life of the party.
* EXT2: I don't talk a lot.
* EXT3: I feel comfortable around people.
* EXT4: I keep in the background.
* EXT5: I start conversations.
* EXT6: I have little to say.
* EXT7: I talk to a lot of different people at parties.
* EXT8: I don't like to draw attention to myself.
* EXT9: I don't mind being the center of attention.
* EXT10: I am quiet around strangers.

#### Emotional Stability (EST)

* EST1: I get stressed out easily.
* EST2: I am relaxed most of the time.
* EST3: I worry about things.
* EST4: I seldom feel blue.
* EST5: I am easily disturbed.
* EST6: I get upset easily.
* EST7: I change my mood a lot.
* EST8: I have frequent mood swings.
* EST9: I get irritated easily.
* EST10: I often feel blue.

#### Agreeableness (AGR)

* AGR1: I feel little concern for others.
* AGR2: I am interested in people.
* AGR3: I insult people.
* AGR4: I sympathize with others' feelings.
* AGR5: I am not interested in other people's problems.
* AGR6: I have a soft heart.
* AGR7: I am not really interested in others.
* AGR8: I take time out for others.
* AGR9: I feel others' emotions.
* AGR10: I make people feel at ease.

#### Conscientiousness (CSN)

* CSN1: I am always prepared.
* CSN2: I leave my belongings around.
* CSN3: I pay attention to details.
* CSN4: I make a mess of things.
* CSN5: I get chores done right away.
* CSN6: I often forget to put things back in their proper place.
* CSN7: I like order.
* CSN8: I shirk my duties.
* CSN9: I follow a schedule.
* CSN10: I am exacting in my work.

#### Openness (OPN)

* OPN1: I have a rich vocabulary.
* OPN2: I have difficulty understanding abstract ideas.
* OPN3: I have a vivid imagination.
* OPN4: I am not interested in abstract ideas.
* OPN5: I have excellent ideas.
* OPN6: I do not have a good imagination.
* OPN7: I am quick to understand things.
* OPN8: I use difficult words.
* OPN9: I spend time reflecting on things.
* OPN10: I am full of ideas.

### Additional Information

* **Time Spent per Question**: Recorded in milliseconds (variables ending in `_E`). This was calculated by taking the time when the button for the question was clicked minus the time of the most recent other button click.
* **Other Variables**:

  * `dateload`: The timestamp when the survey was started.
  * `screenw`: The width of the user's screen in pixels.
  * `screenh`: The height of the user's screen in pixels.
  * `introelapse`: Time in seconds spent on the landing/intro page.
  * `testelapse`: Time in seconds spent on the page with the survey questions.
  * `endelapse`: Time in seconds spent on the finalization page (where users confirmed they had answered accurately and their answers could be stored and used for research; only users who answered "Yes" are included).
  * `IPC`: The number of records from the user's IP address in the dataset. For clean analysis, only use records where this value is 1. High values may be due to shared networks (e.g. universities) or multiple submissions.
  * `country`: The country, determined by technical information (not asked as a question).
  * `lat_appx_lots_of_err`: Approximate latitude of the user, determined by technical information (note: **not very accurate** — see [this article](https://splinternews.com/how-an-internet-mapping-glitch-turned-a-random-kansas-f-1793856052) for details on how IP geolocation can be problematic).
  * `long_appx_lots_of_err`: Approximate longitude of the user.
