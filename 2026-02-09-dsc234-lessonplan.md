# DSC 234 Inside the Machine: AI Literacy Lesson Plan
## Feb 9 - 12, 2026

**Topic:** What is a Semantic Network, and what is/was its role in developing what we now call "large language models" or generative AI and/or natural language processing.

## Materials Needed:
- Checklist and Other Guidelines for "What to Include in your Project Plan/Proposal"
- Datasets dubbed "Fun Libs" by researchers who were trying to train an AI to create humor via a "Mad Libs"-type exercise (.json files)
- Handout of "Fun Libs" story with fill-ins and a word bank. For each word category (of which there are 8) there are 100 words for random selection
- D20, D6 (or online versions will work)

## Learning Outcomes:
- The student will gain understanding and experience with "Large Language Models" and how they process information, in the context of an actual course assignment that the LLM will assist them with.
- The student will discuss and consider ethical issues and other programming limitations associated with training data for Large Language Models. The student will discuss and consider issues concerning AI and humor.
- The student will test an AI's ability to solve a problem in the context of a guessing game with a given riddle.

## Background Information and Definitions

A semantic network is a way of representing knowledge as a graph of concepts and their relationships. Think of it like a web where we have:
- **Nodes** represent concepts (words, ideas, objects)
- **Edges** (connections) represent relationships between concepts

For example, "dog" might connect to "animal" (is-a relationship), "bark" (action), "pet" (category), and "furry" (attribute).

## How Semantic Networks Relate to Fun Libs Humor

When an AI selects words to make Fun Libs funny, it's essentially navigating this semantic network to find words that create semantic incongruity - the clash between what's expected and what appears.

### Key Concepts:

**1. Semantic Distance**
- Words close together in the network are semantically similar ("cat" and "dog")
- Words far apart create surprise and humor ("grandmother" and "exorcises")
- The farther apart, often the funnier - but there's a sweet spot

**2. Context Violation** In a narrative, where there is social, cultural, or collectively understood context and we see a word appear that violates that context:

These create humor because they're semantically distant from a given story context. The network might select them based on the following:
- Expected context: innocent, childlike, simple
- Inserted words: scary, complicated, dark, adult themes
- Result: Comic incongruity

**3. Schema Disruption** A "schema" is a mental framework for understanding situations. Your brain has a schema for "grandmother's house" that includes:
- Warmth, safety, things that one associates with "grandma"
- NOT: trauma, insecure or unsafe things, unpleasantness, things *not* associated with grandma or the expectation of grandma

The AI selects words that activate incompatible schemas within the same semantic network.

### How an AI Might Score Funniness:

Looking at your dataset's wordFunninessGrades and storyFunninessGrades, the AI likely:
1. Measures semantic distance between the replacement word and the original context
2. Checks for taboo/surprise factors (mild taboo often = funnier)
3. Evaluates grammatical fit (must work in the sentence)
4. Balances absurdity (too random = confusing, not funny)

In the training dataset I have provided, "religious theme" words in the Little Red Riding Hood example scored well because they maintain internal coherence (all religion-related) while being maximally distant from fairy tale expectations.

---

## Lesson Details

### Warmup Activity (10 minutes)

**Instructions:** Open ChatGPT or Claude.ai. Prompt it as follows (precisely):

> Let's play a riddle game. I will provide clues. Ask me a 'yes' or 'no' question. I will provide the answer as 'yes', 'no', or 'unknown' if the answer does not help at all and is not known. Each time I respond, you can either guess at the answer to the riddle or ask another question. But you only get 3 questions. Here are the clues: "A bear bum is exposed. I am holding a mug in my hand. There is a privacy barrier nearby." What you must solve: Where am I? What is in the mug?

### Course Final Project - "Write a Plan or Proposal" (25 - 30 minutes)

Hand back students' project proposals for revision

1) Show them how to prompt an AI to help revise their proposal so that it contains all the elements required - use the checklist and other guidelines that had been previously provided to the students.

2) Demonstrate and discuss why this is an effective way to prompt an AI:

> "I am a student given the task of writing a project plan or proposal. I have a rough draft which I will upload to you. In an interview style, ask me questions, one at a time, about the plan that need to be revised. This is for a college class on "AI Literacy". I can also provide you with a checklist of what is to be included, and the grading rubric my professor is going to use."

Give students time to work on this. Walk around the room and offer help as necessary.

### Data Formats - Discussion of Training Data (10 minutes)

Show students the .json file that was used to train an AI for humor. See if they can figure out what the various symbols mean. Discuss the word choices, both ones that were judged to be 'funny' and ones that were judged not to be 'funny'. What sorts of bias exist in the training data? Is there anything inappropriate? (Note: the word 'dimwit') and even some misspellings!

Discuss what .json file format is, and how common it is for applications requiring formatted data.

### "Fun Libs" Experiment Using Random Word Generator (25 - 30 minutes)

Using 2 or 3 of the "Fun Libs" story frames, and the provided word list for each category. The idea is to see if randomly selecting words might produce an equally funny result.

Each student will be provided with a unique "story" in which they will fill in words.

Once filled in, the stories will be shuffled, and the professor will read one to the class. The students each give it a score of 0 = "not funny" or 1 = "funny".

Let the students determine how to score the story of funny or not funny.

If there is time, feed one of the stories into an LLM and see what it comes up with.

Was it funny? Was there anything one could see as potentially problematic with this sort of use of an AI?

---

## Word Bank

**When filling in a Fun Libs Story,** locate the list of words for the required part of speech. Use a random number generator to first select a column (numbered 1 - 5) and then a word within that column (1 - 20).

### 1. NOUNS (100)

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 |
|-------|-------|-------|-------|-------|
| 1. accountant | 21. kale | 41. coverlet | 61. scale | 81. stiletto |
| 2. fedora | 22. jelly | 42. bagpipe | 62. Studebaker | 82. slipper |
| 3. therapist | 23. cluster | 43. tuba | 63. buggy | 83. clog |
| 4. podcast | 24. accordion | 44. ukulele | 64. Cocotaxi | 84. flipflop |
| 5. meme | 25. clickbait | 45. spinner | 65. rickshaw | 85. mukluk |
| 6. router | 26. jug | 46. bracelet | 66. gondola | 86. snowshoe |
| 7. conspiracy | 27. deepfake | 47. unicycle | 67. Yugo | 87. katana |
| 8. labyrinth | 28. colonoscopy | 48. pogo | 68. Segway | 88. dagger |
| 9. bolero | 29. augment | 49. trampoline | 69. scooter | 89. hurdy-gurdy |
| 10. trophy | 30. prenup | 50. castle | 70. kickbike | 90. vestibule |
| 11. selfie | 31. alimony | 51. pit | 71. ebike | 91. sauna |
| 12. crypto | 32. leash | 52. finger | 72. stiletto | 92. swamp |
| 13. disease | 33. feather | 53. visor | 73. slipper | 93. glacier |
| 14. brawl | 34. mullet | 54. blanket | 74. clog | 94. puddle |
| 15. cracker | 35. toupee | 55. onesie | 75. flipflop | 95. marsh |
| 16. shorts | 36. shapewear | 56. romper | 76. mukluk | 96. bedrock |
| 17. x-ray | 37. bidet | 57. thong | 77. snowshoe | 97. pebble |
| 18. muzak | 38. scooter | 58. turtleneck | 78. katana | 98. escalator |
| 19. algae | 39. hoverboard | 59. ascot | 79. dagger | 99. dirigible |
| 20. gluten | 40. kazoo | 60. cummerbund | 80. hurdy-gurdy | 100. dump |

*(Note: Additional entries include aquaduct, cairn, aerialist, ether, magma, oobleck)*

### 2. ADJECTIVES (100)

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 |
|-------|-------|-------|-------|-------|
| 1. moist | 21. crusty | 41. scaly | 61. voluptuous | 81. slimy |
| 2. throbbing | 22. musty | 42. scabby | 62. lit | 82. greasy |
| 3. engorged | 23. dank | 43. oozing | 63. busy | 83. oily |
| 4. tumescent | 24. rancid | 44. festering | 64. mid | 84. slippery |
| 5. turgid | 25. putrid | 45. weeping | 65. basic | 85. slick |
| 6. swollen | 26. fetid | 46. seeping | 66. cringe | 86. smooth |
| 7. glistening | 27. rank | 47. gnarly | 67. awkward | 87. silky |
| 8. pulsating | 28. gamey | 48. frisky | 68. uncomfortable | 88. velvety |
| 9. jacked | 29. funky | 49. randy | 69. questionable | 89. supple |
| 10. ripped | 30. sweaty | 50. amorous | 70. dubious | 90. tender |
| 11. shredded | 31. clammy | 51. lusty | 71. shady | 91. juicy |
| 12. thick | 32. damp | 52. aroused | 72. shifty | 92. succulent |
| 13. problematic | 33. soggy | 53. titillated | 73. slimy | 93. plump |
| 14. toxic | 34. limp | 54. stimulated | 74. greasy | 94. rotund |
| 15. unhinged | 35. flaccid | 55. agitated | 75. oily | 95. portly |
| 16. feral | 36. wilted | 56. flustered | 76. slippery | 96. chunky |
| 17. deranged | 37. droopy | 57. bothered | 77. slick | 97. hefty |
| 18. unwell | 38. saggy | 58. riled | 78. smooth | 98. beefy |
| 19. concerning | 39. wrinkly | 59. torqued | 79. silky | 99. meaty |
| 20. sketchy | 40. leathery | 60. voluptuous | 80. velvety | 100. substantial |

*(Note: Additional entries include tubular, bloated, distended, bulbous, bulging, protruding, jutting, thrusting, erect)*

### 3. VERBS (100)

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 |
|-------|-------|-------|-------|-------|
| 1. twerk | 21. lug | 41. incentivize | 61. microdose | 81. unfriend |
| 2. thrust | 22. eviscerate | 42. leverage | 62. macrodose | 82. unfollow |
| 3. gyrate | 23. defile | 43. pivot | 63. detox | 83. block |
| 4. undulate | 24. desecrate | 44. disrupt | 64. cleanse | 84. mute |
| 5. pulsate | 25. gaslight | 45. innovate | 65. purge | 85. ghost |
| 6. throb | 26. manipulate | 46. ideate | 66. exfoliate | 86. catfish |
| 7. quiver | 27. exploit | 47. brainstorm | 67. moisturize | 87. troll |
| 8. shudder | 28. weaponize | 48. workshop | 68. hydrate | 88. lurk |
| 9. convulse | 29. monetize | 49. onboard | 69. marinate | 89. stalk |
| 10. spasm | 30. optimize | 50. downsize | 70. simmer | 90. creep |
| 11. twitch | 31. synergize | 51. restructure | 71. percolate | 91. slide |
| 12. flinch | 32. incentivize | 52. doomscroll | 72. ferment | 92. swipe |
| 13. recoil | 33. leverage | 53. binge | 73. pickle | 93. match |
| 14. wince | 34. pivot | 54. overshare | 74. brine | 94. screenshot |
| 15. cringe | 35. disrupt | 55. vent | 75. cure | 95. screencap |
| 16. squirm | 36. innovate | 56. unload | 76. age | 96. dox |
| 17. writhe | 37. ideate | 57. unpack | 77. ripen | 97. hack |
| 18. wriggle | 38. brainstorm | 58. process | 78. mature | 98. phish |
| 19. jiggle | 39. workshop | 59. manifest | 79. unfriend | 99. spam |
| 20. wobble | 40. onboard | 60. visualize | 80. unfollow | 100. upload |

*(Note: Additional entries include download, stream)*

### 4. PART OF THE BODY (100)

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 |
|-------|-------|-------|-------|-------|
| 1. giblets | 21. giblets | 41. jowls | 61. shin | 81. nostril |
| 2. gizzard | 22. junk | 42. wattle | 62. calf | 82. earlobe |
| 3. spleen | 23. bulge | 43. dewlap | 63. hamstring | 83. eyelid |
| 4. pancreas | 24. cankles | 44. gullet | 64. glute | 84. eyebrow |
| 5. coccyx | 25. bunion | 45. esophagus | 65. buttock | 85. eyelash |
| 6. colon | 26. corn | 46. windpipe | 66. cheek | 86. cuticle |
| 7. rectum | 27. callus | 47. trachea | 67. rump | 87. hangnail |
| 8. sphincter | 28. blister | 48. larynx | 68. haunches | 88. knuckle |
| 9. anus | 29. wart | 49. uvula | 69. backside | 89. fingernail |
| 10. butthole | 30. mole | 50. tonsil | 70. posterior | 90. toenail |
| 11. taint | 31. cyst | 51. adenoid | 71. derriere | 91. kneecap |
| 12. perineum | 32. boil | 52. appendix | 72. gluteus | 92. forearm |
| 13. groin | 33. pimple | 53. gallbladder | 73. maximus | 93. bicep |
| 14. loins | 34. blackhead | 54. bladder | 74. nostril | 94. tricep |
| 15. privates | 35. whitehead | 55. urethra | 75. earlobe | 95. quadricep |
| 16. giblets | 36. pore | 56. prostate | 76. eyelid | 96. pectoral |
| 17. junk | 37. follicle | 57. testicle | 77. eyebrow | 97. abdomen |
| 18. bulge | 38. pustule | 58. scrotum | 78. eyelash | 98. sternum |
| 19. cankles | 39. abscess | 59. nipple | 79. cuticle | 99. clavicle |
| 20. bunion | 40. fistula | 60. areola | 80. hangnail | 100. scapula |

*(Note: Additional entries include bellybutton, navel, innie, outie, armpit, underarm, elbow, ankle, tendon, vertebra)*

### 5. ADVERBS (100)

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 |
|-------|-------|-------|-------|-------|
| 1. menacingly | 21. provocatively | 41. moistly | 61. haphazardly | 81. tragically |
| 2. ominously | 22. tantalizingly | 42. damply | 62. recklessly | 82. devastatingly |
| 3. threateningly | 23. teasingly | 43. clammily | 63. carelessly | 83. crushingly |
| 4. aggressively | 24. coyly | 44. stickily | 64. thoughtlessly | 84. numbly |
| 5. violently | 25. flirtatiously | 45. greasily | 65. mindlessly | 85. hollowly |
| 6. vigorously | 26. coquettishly | 46. slimily | 66. stupidly | 86. emptily |
| 7. enthusiastically | 27. demurely | 47. goopily | 67. idiotically | 87. vacantly |
| 8. zealously | 28. bashfully | 48. sloppily | 68. moronically | 88. blankly |
| 9. fervently | 29. sheepishly | 49. messily | 69. foolishly | 89. glassily |
| 10. passionately | 30. awkwardly | 50. frantically | 70. absurdly | 90. lifelessly |
| 11. ardently | 31. uncomfortably | 51. desperately | 71. ridiculously | 91. listlessly |
| 12. lustfully | 32. painfully | 52. urgently | 72. laughably | 92. lethargically |
| 13. wantonly | 33. excruciatingly | 53. feverishly | 73. pathetically | 93. sluggishly |
| 14. lasciviously | 34. agonizingly | 54. maniacally | 74. pitifully | 94. torpidly |
| 15. salaciously | 35. torturously | 55. hysterically | 75. miserably | 95. languidly |
| 16. lecherously | 36. unbearably | 56. wildly | 76. wretchedly | 96. indolently |
| 17. carnally | 37. insufferably | 57. erratically | 77. deplorably | 97. apathetically |
| 18. sensually | 38. intolerably | 58. chaotically | 78. lamentably | 98. limply |
| 19. seductively | 39. moistly | 59. haphazardly | 79. regrettably | 99. weakly |
| 20. suggestively | 40. damply | 60. recklessly | 80. unfortunately | 100. feebly |

*(Note: Additional entries include halfheartedly, reluctantly, begrudgingly)*

### 6. TYPE OF FOOD (100)

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 |
|-------|-------|-------|-------|-------|
| 1. sausage | 21. larvae | 41. shallots | 61. ar`chokes | 81. mushrooms |
| 2. cheese | 22. grubs | 42. scallions | 62. okra | 82. truffles |
| 3. tripe | 23. eggs | 43. chives | 63. eggplant | 83. fungus |
| 4. chitlins | 24. oysters | 44. kale | 64. zucchini | 84. mold |
| 5. tongue | 25. clams | 45. spinach | 65. squash | 85. yeast |
| 6. marrow | 26. mussels | 46. chard | 66. gourd | 86. gelatin |
| 7. liver | 27. sardines | 47. collards | 67. pumpkin | 87. gravy |
| 8. gizzard | 28. anchovies | 48. turnips | 68. yams | 88. grease |
| 9. kidney | 29. herring | 49. rutabaga | 69. beets | 89. lard |
| 10. heart | 30. mackerel | 50. parsnips | 70. mushrooms | 90. tallow |
| 11. brain | 31. lutefisk | 51. beets | 71. truffles | 91. suet |
| 12. snout | 32. natto | 52. radishes | 72. fungus | 92. fat |
| 13. intestine | 33. tofu | 53. cabbage | 73. mold | 93. blubber |
| 14. stomach | 34. tempeh | 54. brussels | 74. yeast | 94. jerky |
| 15. haggis | 35. seitan | 55. asparagus | 75. gelatin | 95. spam |
| 16. escargot | 36. durian | 56. artichokes | 76. gravy | 96. loaf |
| 17. crickets | 37. jackfruit | 57. okra | 77. grease | 97. paste |
| 18. mealworms | 38. kimchi | 58. eggplant | 78. lard | 98. spread |
| 19. cicadas | 39. sauerkraut | 59. zucchini | 79. tallow | 99. porridge |
| 20. worms | 40. pickles | 60. squash | 80. suet | 100. gruel |

*(Note: Additional entries include slop, mush, pulp, paste, goop, slime, curd)*

### 7. ANIMAL (100)

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 |
|-------|-------|-------|-------|-------|
| 1. platypus | 21. termite | 41. limpet | 61. lamprey | 81. opossum |
| 2. mole | 22. silverfish | 42. urchin | 62. shark | 82. possum |
| 3. blobfish | 23. earwig | 43. starfish | 63. ray | 83. wombat |
| 4. axolotl | 24. centipede | 44. anemone | 64. skate | 84. capybara |
| 5. hagfish | 25. millipede | 45. jellyfish | 65. sturgeon | 85. badger |
| 6. lamprey | 26. scorpion | 46. squid | 66. paddlefish | 86. weasel |
| 7. leech | 27. tarantula | 47. octopus | 67. sawfish | 87. ferret |
| 8. slug | 28. spider | 48. cuttlefish | 68. guitarfish | 88. mink |
| 9. snail | 29. crab | 49. nautilus | 69. ratfish | 89. stoat |
| 10. worm | 30. lobster | 50. anglerfish | 70. toad | 90. marten |
| 11. earthworm | 31. shrimp | 51. catfish | 71. bullfrog | 91. wolverine |
| 12. tapeworm | 32. prawn | 52. carp | 72. frog | 92. skunk |
| 13. hookworm | 33. crawfish | 53. sucker | 73. salamander | 93. porcupine |
| 14. roundworm | 34. crayfish | 54. remora | 74. newt | 94. hedgehog |
| 15. maggot | 35. barnacle | 55. eel | 75. lungfish | 95. shrew |
| 16. grub | 36. limpet | 56. lamprey | 76. mudskipper | 96. vole |
| 17. larvae | 37. urchin | 57. shark | 77. snakehead | 97. lemming |
| 18. cockroach | 38. starfish | 58. ray | 78. piranha | 98. gopher |
| 19. beetle | 39. anemone | 59. skate | 79. candiru | 99. marmot |
| 20. bedbug | 40. jellyfish | 60. sturgeon | 80. vampire | 100. groundhog |

*(Note: Additional entries include prairie, chipmunk, beaver, otter, platypus)*

### 8. TYPE OF LIQUID (100)

| Col 1 | Col 2 | Col 3 | Col 4 | Col 5 |
|-------|-------|-------|-------|-------|
| 1. oil | 21. urine | 41. brine | 61. tar | 81. spirits |
| 2. grease | 22. goop | 42. vinegar | 62. pitch | 82. liquor |
| 3. lard | 23. kacka | 43. pickle | 63. bitumen | 83. whiskey |
| 4. tallow | 24. dung | 44. marinade | 64. asphalt | 84. vodka |
| 5. fat | 25. manure | 45. sauce | 65. petroleum | 85. rum |
| 6. slime | 26. sludge | 46. gravy | 66. kerosene | 86. gin |
| 7. mucus | 27. slurry | 47. stock | 67. gasoline | 87. tequila |
| 8. phlegm | 28. slop | 48. broth | 68. diesel | 88. brandy |
| 9. sputum | 29. sewage | 49. bouillon | 69. fuel | 89. cognac |
| 10. saliva | 30. effluent | 50. consommé | 70. ethanol | 90. schnapps |
| 11. drool | 31. runoff | 51. juice | 71. methanol | 91. absinthe |
| 12. slobber | 32. drainage | 52. nectar | 72. alcohol | 92. moonshine |
| 13. spit | 33. seepage | 53. syrup | 73. spirits | 93. hooch |
| 14. bile | 34. brine | 54. molasses | 74. liquor | 94. rotgut |
| 15. pus | 35. vinegar | 55. treacle | 75. whiskey | 95. swill |
| 16. discharge | 36. pickle | 56. honey | 76. vodka | 96. grog |
| 17. ooze | 37. marinade | 57. sap | 77. rum | 97. mead |
| 18. seepage | 38. sauce | 58. resin | 78. gin | 98. ale |
| 19. leakage | 39. gravy | 59. latex | 79. tequila | 99. lager |
| 20. dribble | 40. stock | 60. tar | 80. brandy | 100. stout |

*(Note: Additional entries include porter, cider, perry, wine, sherry, port, vermouth, champagne, prosecco, sangria, punch)*
