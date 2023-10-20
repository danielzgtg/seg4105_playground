# SEG4105-A02 Tutorial 6

|Name|Student Number|
|---|---|
|Daniel Tang|0300068985|

## Place your bets

The individual commentary notes will be documented in the shared project repository. The betting table was done over a weekend instead of the tutorial.

## Notes

Look where we are: We have an existing product.

<div style="page-break-before:always"></div>

### Questline discussion

Allowing users to efficiently work on tasks via the gamification of the Mikado method.

#### Does the problem matter?

Dish: Large graphs need organized guided issue tracker. Phil mentioned it to the client, and the client liked the idea.

Daniel: Will multiple customers use this feature? Dish: We will advertise it and most people will use it for all but the small  graphs.

Conclusion: Yes

#### Is the appetite right?

Dish: Should the questline see through subgraphs? Daniel: No, that will involve loading too much stuff into memory and defeat database partitioning. Dish: Yeah, it’s will be too cluttered anyway.

Daniel: In the client's example graph, how give me an example of a questline. Dish: So the goal node is special, and every branch off of it is a questline.

Dish: All the questlines are separate. Daniel: That might be hard, as opposed to only the nodes coming off the goal node being separate and the children being shareable. Dish: Yeah, that might be easier.

Dish: We want to show the deepest node at the top. Daniel: I would have just partitioned the ready to the top and the completed to the end, as that might be easier to implement. Dish: We can just leave it unspecified for simplicity.

Dish: So we will need to implement a UI and an overlay. Daniel: The other problem is synchronization between the graph and the questline. Dish: We can make the graph the single source of truth, and make sure the questline always recalculates if required.

Daniel: Are we actually going to draw the questline tree and how? Dish: No, we’re only going to display current task and next task.

Conclusion: Yes, the appetite is right. The pitch became articulated better after asking questions. It’s doable in six weeks. We are all interested because we it’s very cool.

#### Is the solution attractive?

Dish: We want the number of tasks done. Daniel: Where is this is the sketch? Dish: I mean I like the percentage better.

Daniel: The drawn questline picture is so basic that a Minecraft mod looks better. Dish: That’s just a sketch, it’s supposed to look like the actual Escape from Tarkov screen.

Daniel: Do we have one current task or multiple? Dish: It’s just one for simplicity. You can change quests at any time though.

Daniel: We can’t put the current task overlay on the bottom right because the FAB is there. Dish: That only affect mobile. Daniel: Or how about the top left? Dish: That works.

Daniel: This is a major enough feature that we will always keep this space for it in the future.

Conclusion: Yes, the solution is attractive.

#### Is this the right time?

Dish: We’re still in development, and we’re only doing polishing at the moment, no major features. (“splash of news with a new feature”)

Daniel: And we really want to give this feature to the client before the end of the semester.

Conclusion: Yes, this is the right time.

Are the right people available?

Dish: It’s a big feature with a lot of work, but we have everyone. Phil already did the rough design, which we modified a bit. Daniel and Dish can all do React fullstack. Jodi can help.

Daniel: We have all the expertise. Midterms are half over. We’ve all been doing small batch and we want to do big batch now. Everyone is here reading week.

Conclusion: Yes, the right people are available.

<div style="page-break-before:always"></div>

### Scanning discussion

Allowing users to import paper graphs.

#### Does the problem matter?

Dish: Important for Andriy to convert all his paper graphs, especially because his graphs are huge. However, if it doesn’t work, it might consume a disproportionate amount of customer support.

Daniel: I suppose it doesn’t matter for most customers who are just starting the Mikado method and don’t have anything to import. As the shapes are different between paper and software, he spent some time moving nodes around at our client meeting, so merely scanning isn’t 100% of the time needed for importing.

Conclusion: Not really, the problem only matters 67% for the client, and probably not for other people.

#### Is the appetite right?

Dish: Image detection will take a lot of time to get right. My previous coop took 4 months to get it working. It’s not even used that often. There’s also the problem of different cameras, and messy handwriting recognition. Camera skew, glare, and contrast were problems.

Daniel: I supposed the derisking part of me saying “off the shelf” only applied to tweaking the settings. Then there’s getting the default settings to work for users' different setups.

Daniel: What do you think about this improving the new user experience? Dish: It doesn’t matter because new users don’t use the Mikado method, and people who want to import their graphs will already be inclined to use the webapp. So the target market is just the number of people who use the Mikado method and those who draw their Mikados, which would probably just be 1 person our client.

Daniel: What about doing it in 2 weeks? Dish: We can’t do it in 2 weeks. OCR is too much risk and finicky to get right.

Daniel: This magically scanning of paper is cool. Dish: However, I don’t want to do OCR from my previous coop anymore.

Conclusion: No, the appetite is too small.

#### Is the solution attractive?

Dish: Yes, we can afford adding the camera button to the home page. If that’s too much, we can put it in the hamburger menu.

Daniel: How would this compare to importing graphs to Andriy manually? Dish: It would take a lot of time, but potentially less time than getting this feature right.

Conclusion: No, this solution is not attractive, and we will import his graphs manually. Dish: Or he can do it himself.

#### Is this the right time?

Dish: In terms of timing, technically this is a new feature, and we want to do features.

Daniel: And we don’t have many bugs that the client wants us to fix anymore.

Conclusion: Yes, this is the right time for a new feature, even if not this one.

#### Are the right people available?

Daniel: Dish, you have experience. Dish: That took me 4 months, and that was a long time ago. The only thing that worked well was corner detection.

Daniel: I kind of have the knowledge about vision transformers if Dish, you don’t want to use OpenCV. However, I didn’t attempt to acquire any hands-on experience, so fixing unexpected issues might introduce a lot of scope creep.

Dish: Phil probably or probably not would have designed it the way you, Daniel, drew it but I’m not sure.

Daniel: I suppose this feature needs to be scope hammered away.

Conclusion: No, we are not certain we have the right people yet. We probably do, but we’re not certain.

<div style="page-break-before:always"></div>

### Conclusion

The questline feature is the winning pitch.

## What's left to be done

- Meeting minutes cleanup
- Apply agreed upon changes from meeting minutes to winning pitch
