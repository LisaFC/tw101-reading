This is the pre-reading for the *Technical Writing 101* class, giving you a quick tour of some basic technical writing concepts. We'll explore all these topics and put into practice what you've learned in the actual workshop.

---

# Words


### Define new or unfamiliar terms

When writing or editing, learn to recognize terms that might be unfamiliar to some or all of your target audience.

*   If the term is something that already exists, link to a good existing explanation. (Don't reinvent the wheel.) 
*   If your doc is introducing the term, define the term. Consider providing a glossary if you're introducing many terms.

To define a new term, start by writing a clear one-sentence explanation. Your definition will ultimately span more than one sentence, but begin with a single sentence that can stand on its own and serve as a life raft for readers. For example:

>**Frambly** is a sorting preprocessor that selects the optimal sorting algorithm based on the input data's organization.

Notice that we boldfaced the term; boldface guides readers back to the definition. Only boldface the new term once.

Beyond the first sentence, good definitions tend to compare and contrast the new term with something that the reader might be familiar with. For example:

>Conceptually, Frambly occupies a similar niche to Foobar. However, Frambly automatically chooses among a dozen sorting algorithms, while Foobar can only toggle between two.

Readers appreciate definitions that contain examples, such as the following:

>For example, the Carambola Server calls Frambly to choose the right sorting mechanism. That's because the Carambola Server accepts a wide variety of input data.


### Use terms consistently

If you change the name of a variable midway through a method, your code won't compile. Similarly, if you rename a term in the middle of a document, your ideas won't compile (in your users' heads). Apply the same unambiguous word or term consistently throughout your doc. Once you've named a component **thingy**, don't rename it **thingamabob**. 

However, when introducing a long-winded concept name or product name, you may also specify a shortened version of that name. Then you may use that shortened name throughout the document. For example, the following paragraph is fine:

>**Protocol Buffers** (or **protobufs** for short) provide their own definition language. Blah, blah, blah. And that's why protobufs have won so many county fairs.


### Introduce and use acronyms correctly

Acronyms and abbreviations provide another effective way to refer to compound nouns and other large clusters of words. However, even engineers on your team might not be familiar with the same set of acronyms and abbreviations that you use. The cognitive load of using an acronym or an abbreviation is similar to wrapping a class with a long name in a class with a shorter name. So, create acronyms sparingly.

On the initial use of an acronym within a document or a section, spell out the full term, and then put the acronym in parentheses. Put both the spelled-out version and the acronym in boldface. For example:

>This document is for engineers who are new to the **Google Display Network** (**GDN**) or need to understand how GDN serving systems work.

You can then use the acronym going forward, as in the following example:

>If no cache entry exists, the Mixer calls the **OttoGroup Server** (**OGS**) to fetch ottos for the request. The OGS is a repository that holds all servable ottos. The OGS is organized in a logical tree structure, with a root node and two levels of leaf nodes. The OGS root forwards the request to the leaves and collects the responses.

Do not cycle back-and-forth between the acronym and the expanded version in the same document. 

### Disambiguate pronouns

Many pronouns point to a previously introduced noun, somewhat like pointers in programming. Also like pointers in programming, improperly used pronouns tend to introduce errors. In many cases, you should simply avoid the pronoun and just reuse the noun. However, the utility of a pronoun sometimes outweighs its risk (as in this sentence).

The following pronouns incur the most errors:

*   it
*   they (including them and their)

For example, in the following sentence, does **It** refer to Python or to C++?

>Python is interpreted, while C++ is compiled. **It** has an almost cult-like following.

Before using the dangerous pronouns **it** or **they**, consider the following guidelines:

*   Only use a pronoun *after* you've introduced the noun, never before.
*   Place the pronoun as close as possible to the referring noun. As a rule of thumb, if more than five words separate your noun from your pronoun, consider repeating the noun instead of using the pronoun.
*   If you introduce a second noun between your noun and your pronoun, reuse your noun instead of using a pronoun.

And while we're on the subject of wayward pronouns, be careful using:

*   this
*   that

For example, in this following ambiguous sentence, **This** could refer to Frambus, to Foo, or to both:

>You may use either Frambus or Foo to calculate derivatives. **This** is not optimal.

Use either of the following tactics to disambiguate **this** and **that**:

*   Replace **this** or **that** with the noun.
*   Place a noun immediately after **this** or **that**.

For example, either of the following sentences disambiguate the previous example:

>**Overlapping functionality** is not optimal.

>**This overlapping functionality** is not optimal.

---

# Active voice vs passive voice

In an active voice sentence or phrase, an actor clearly performs an action on a target. For example, here's a short, active voice sentence:

>The cat sat on the mat.

*   actor: The cat
*   action: sat
*   target: the mat

By contrast, here's that same sentence written in passive voice, where the subject of the sentence is the target:

>The mat was sat on by the cat.

*   target: The mat
*   action: was sat on
*   actor: the cat


Some passive voice sentences omit an actor. For example:

>The mat was sat on.

*   actor: ???
*   action: was sat on
*   target: the mat

Who or what sat on the mat? A cat? A T-Rex? You?


Imperative sentences, those that start with a command ("Compile the…", "Write the…"), are typically in active voice, even though they do not explicitly mention an actor. That's because imperative sentences *imply* an actor. The implied actor is either the first-person (**I, we, us**), or the second person (**you**) .


### Prefer active voice to passive voice

Use the active voice most of the time. Use the passive voice sparingly. Active voice brings the following advantages:

*   Active voice is generally clearer than passive voice because you're explicit about the relationship between ideas in your sentence.
*   Active voice sentences are generally shorter than their passive voice equivalents.

Most people mentally convert passive voice sentences into active voice sentences. Why subject your readers to extra processing time? By sticking to active voice, readers can skip the preprocessor stage and go straight to compilation.

Passive voice obfuscates your ideas, turning sentences on their head. Passive voice reports action indirectly. Worst of all, some passive voice sentences even omit an actor altogether, which forces the reader to guess the actor's identity.

---

# Clear sentences

Comedy writers seek the funniest results, horror writers strive for the scariest, and technical writers aim for the clearest. In technical writing, clarity takes precedence over all other rules. This unit suggests a few ways to clarify your sentences.


### Choose strong verbs

To engage and educate readers, choose precise, strong, specific verbs; avoid imprecise, weak, or generic verbs. For example, try to reduce your use of the following generic verbs:

*   forms of be: is, are, am, was, were, etc.
*   occur
*   happen

Many technical writers believe that the verb is the most important part of a sentence. Pick the right verb and the rest of the sentence will take care of itself. For example, consider how strengthening the weak verb in the following sentences improves each sentence:


<table>
  <tr>
   <td><strong>Weak Verb</strong>
   </td>
   <td><strong>Strong Verb</strong>
   </td>
  </tr>
  <tr>
   <td>This test <strong>occurs</strong> in cron once a day.
   </td>
   <td>Cron <strong>runs</strong> this test once a day.
   </td>
  </tr>
  <tr>
   <td>This error message <strong>happens</strong> when...
   </td>
   <td>The system <strong>generates</strong> this error message when...
   </td>
  </tr>
  <tr>
   <td>We <strong>are</strong> very careful to ensure...
   </td>
   <td>We carefully <strong>ensure</strong>...
   </td>
  </tr>
</table>


That said, a form of *be* is sometimes the best choice of verb, so don't feel that you have to eliminate every form of *be* from your writing.

Note that generic verbs often signal other ailments, such as:

*   an imprecise or missing actor in a sentence
*   a passive voice sentence

### Clarify statements with examples and caveats


Embrace the transition **for example**. After presenting a statement or rule, provide a good example. Examples help solidify technical readers' understanding. For example (sorry for getting so meta), consider the following two sentences:

>Call the appropriate flags.DEFINE_datatype function to create a flag that accepts values of a certain datatype. For example, call the flags.DEFINE_integer function to create a flag that accepts integer values.

In the preceding passage, the first sentence introduces a rule and the second sentence demonstrates that rule through an example.

While we're spreading the love for transitions, consider the value of **however**. This transition warns users that they are about to encounter something unexpected.

>The following example sets the id field to "required." **However**, in certain contexts, setting id to "required" can get you fired.


### Reduce there is/there are

Sentences that start with **There is** or **There are** marry a generic noun to a generic verb, making the "real" subject and verb less obvious.

In the best case scenario, you may simply delete **There is** or **There are** (and possibly another word or two later in the sentence). For example, removing **There are** from the following generic sentence:

>There are Frambus variables that track these metrics.

strengthens the sentence to:

>Frambus variables track these metrics.

You can sometimes repair a **There is** or **There are** sentence by moving the true subject and true verb from the end of the sentence to the beginning. For example, change the following generic start:

>There are two disturbing facts about Perl you should know.

to the stronger:

>You should know two disturbing facts about Perl.

In still other situations, writers start sentences with **There is** or **There are** to avoid the hassle of creating true subjects or verbs. If no subject exists, you must create one. For example, the following **There is** sentence does not identify the receiving entity:

>There is no guarantee that the updates will be received in sequence order.

Specifying a subject (**clients**) creates a clearer experience for the reader:

>Clients might not receive updates in sequence order.

---

# Short sentences

Software engineers generally aim to minimize the number of lines of code in an implementation. A great engineer can sometimes implement in 25 lines what it takes an inexperienced programmer to do in 100 lines. Great engineers minimize lines for the following reasons:

*   Shorter code typically runs faster than longer code.
*   Shorter code is typically easier to maintain than longer code.
*   Extra lines of code introduce additional points of failure.

In fact, the same rules apply to technical writing:

*   Shorter documentation reads faster than longer documentation.
*   Shorter documentation is typically easier to maintain than longer documentation.
*   Extra lines of documentation introduce additional points of failure.

Finding the shortest documentation implementation takes time but is ultimately worthwhile. Short sentences communicate more powerfully than long sentences, and they're easier to understand.


### Focus each sentence on a single idea

Focus each sentence on a single idea, thought, or concept. Just as statements execute a single task, sentences should execute a single idea. For example, the following run-on sentence (jam-packed with fiction) contains multiple thoughts:

>Pat Connolly invented FORTRAN 55 in 1958, which was a watershed year in computing, since it was also the year that John McCarthy invented Lisp, which gave computing both an iterative way of attacking problems and a recursive way.

Breaking the run-on into a succession of single-idea sentence yields the following result:

>Pat Connolly invented FORTRAN 55 in 1958. By coincidence, John McCarthy invented Lisp in the same year. These inventions gave computer science both an iterative and a recursive language for attacking problems.


### Convert some run-ons to lists

Inside many run-on technical sentences is a list yearning to break free. For example, consider the following sentence:

>To alter the usual flow of a loop, you may use either a **break** statement (which hops you out of the current loop) or a **continue** statement (which skips past the remainder of the current iteration of the current loop).

When you see the conjunction **or** in a long sentence, consider refactoring that sentence into a bulleted list. When you see an embedded list of items or tasks within a long sentence, consider refactoring that sentence into a bulleted or numbered list. For example, the preceding example contains the conjunction **or**, so let's convert that run-on sentence to the following bulleted list:

>To alter the usual flow of a loop, call one of the following statements:
>
>*   break, which hops you out of the current loop.
>*   continue, which skips past the remainder of the current iteration of the current loop.


### Eliminate or reduce extraneous words

Many sentences contain filler—textual junk food that consumes space without nourishing the reader. For example, see if you can spot the unnecessary words in the following sentence:

>An input value greater than 100 causes the triggering of logging.

Replacing **causes the triggering of** with the much shorter verb **triggers** yields a shorter sentence:

>An input value greater than 100 triggers logging.

The following table suggests replacements for a few common bloated phrases:


<table>
  <tr>
   <td><strong>Wordy</strong>
   </td>
   <td><strong>Concise</strong>
   </td>
  </tr>
  <tr>
   <td>at this point in time
   </td>
   <td>now
   </td>
  </tr>
  <tr>
   <td>determine the location of
   </td>
   <td>find
   </td>
  </tr>
  <tr>
   <td>is able to
   </td>
   <td>can
   </td>
  </tr>
</table>


---

# Lists and tables

### Choose the correct type of list

Technical readers generally love lists. Lists organize chaos. Lists enable readers to easily pick out important or memorable points.

The following types of lists dominate technical writing:

*   bulleted lists
*   numbered lists

Bulleted lists and numbered lists are not interchangeable. Use a **bulleted list** for *unordered* items; use a **numbered list** for *ordered* items. In other words:

*   If you rearrange the items in a *bulleted* list, the list's meaning stays the same.
*   If you rearrange the items in a *numbered* list, the list's meaning *changes*.

For example, we've made the following a bulleted list because rearranging its elements will not change the list's meaning:

>Bash provides the following string manipulation mechanisms:
>
>*   deleting a substring from the start of a string
>*   reading an entire file into one string variable

The following list, by contrast, must be a numbered list because rearranging its elements would change the list's meaning:

Take the following steps to reconfigure the server:

>1.  Stop the server.
>1.  Edit the configuration file.
>1.  Restart the server.

### Keep list items parallel

What makes a list effective - easy to read and memorable? Effective lists are typically **parallel**. All items in a **parallel** list obey consistent rules along all of the following parameters:

*   grammar
*   logical category
*   capitalization
*   punctuation

Conversely, at least one item in a **nonparallel** list fails at least one of the preceding consistency checks. For example, the following list is parallel because each item is a proper noun representing the name of a company:

*   Google
*   Microsoft
*   Amazon

The following list is parallel because each item is a complete sentence:

*   Google provides a search engine.
*   Microsoft provides a suite of office applications.
*   Amazon sells things.

The following list is nonparallel because not all items are logically consistent:

*   Google
*   Microsoft
*   llamas

The following list is nonparallel because two of the items are complete sentences and one is not:

*   Google provides a search engine.
*   Microsoft Office
*   Amazon sells things.

Note that the punctuation for all items in a single list should be consistent. For example, if one item ends with a period, then all the other items should end with a period.


### Start numbered list items with imperative verbs

Consider starting all items in a numbered list with an imperative verb. An **imperative verb** is a command, such as **open** or **start**. For example, notice how all of the items in the following parallel numbered list begin with an imperative verb:

>1.  Download the Frambus app from Google Play.
>1.  Configure the Frambus app's settings.
>1.  Start the Frambus app.

### Introduce each list and table

We recommend introducing each list and table with a sentence that tells readers what the list or table represents. In other words, give the list or table context. Finish the introductory sentence with a colon rather than a period.

Although not a requirement, we recommend putting the word **following** into the introductory sentence. The word **following** guides technical readers and assures them that the context really does apply to the list or table after the introductory sentence. For example, consider the following introductory sentences:

>The following list identifies key performance parameters:

>Take the following steps to install the Frambus package:


### Consider tables

Tables are a great medium for the analytic mind. Given a page containing multiple paragraphs and a single table, an engineer's eyes zoom towards the table. Two-dimensional arrays are a natural container for engineering work. 

---

# Paragraphs

You'll demonstrate much of your effectiveness as a writer by how you organize sentences into paragraphs. The work of writing is simply this: untangling the dependencies among the parts of a topic, and presenting those parts in a logical stream that enables the reader to understand you.

### Create a great lead sentence

Start each paragraph with a strong, clear sentence. If your paragraphs predictably start with key information, hurried readers can scan your document more quickly and effectively.

### Answer three questions

Good paragraphs answer the following three questions:

1.  **What** are you trying to tell your reader?
1.  **Why** is it important for the reader to know this? (Or, if you prefer, **so what**?)
1.  **How** should the reader use this knowledge, or know your point to be true?


### Focus each paragraph on a single topic

A paragraph should explain exactly one part of an idea. That is, a paragraph is an independent unit of logic. As much as possible, try to restrict the paragraph to your current topic, without talking about what will happen in a future topic or what happened in a past topic. When revising, ruthlessly delete (or move to another paragraph) any sentence that doesn't directly relate to the current idea.

---

# Audience


### Identify your audience(s)

You should always target your documentation for a specific audience or set of audiences. But who is that audience? Are you targeting every engineer in your company or perhaps some subset of that group?


### Work around the curse of knowledge

Experienced engineers can suffer from **the curse of knowledge**, which means that our expert understanding of a topic ruins our explanations to newcomers. As experts, it is terribly easy to forget that novices don't know what you already know. Novices might not follow an explanation that makes passing reference to subtle interactions and deep systems that the expert doesn't stop to explain.

A common way to spot the curse of knowledge in your own writing is to identify terms that might be unfamiliar to your audience. When you find an unfamiliar term, take one of the following two tactics:

*   Define that term in an appropriate way for the target audience.
*   Write around that term. That is, avoid using that term. Find another way to explain the term.

---

# Documents

You can write sentences. You can write paragraphs. But can you organize all those paragraphs into a coherent document?

### State your document's scope

A good document begins by defining its scope. For example:

>This document describes the overall design of Project Frambus.

A better document additionally defines its non-scope, that is, the topics not covered that the target audience might expect your document to cover. For example:

>This document does not describe the design for the related technology, Project Froobus.

These scope and non-scope statements benefit not only the reader but also the writer (you). While writing, if the contents of your document veer away from the scope statement, then you must either refocus your document or modify your scope statement. When reviewing your first draft, delete (or branch off to another document) any sections that don't help satisfy the scope statement.


### State your document's audience

A good document also declares its audience, so relevant readers easily know it's for them and others can look elsewhere. For example:

>We've aimed this document at engineers supporting Frambus.


### Establish your key points up front

Like newspaper articles, engineering documents should position key points at the beginning of the document. Scientific documents typically put conclusions at the end of the document. Don't do this in a technical document! Pretend that your fellow engineers are busy people who won't necessarily read all 76 pages of your document. When reviewing your documentation, ensure that page one answers all of your readers' essential questions.

Note that professional writers focus a lot of energy on page one just to increase the odds of readers making it to page two.


### Help your audience

Answering the following questions before writing will help drive your document's contents.

*   Who is your target audience?
*   What do your readers already know before they've read the document?
*   What should your readers know or be able to do after they've read your document?

For example, the following represent a set of answers to these questions:

*   My target audience is "All engineers in my company."
*   Most of my target audience is familiar with sorting algorithms from undergraduate or graduate school. Some of those readers are experts, but others are rusty.
*   After reading this document, readers will know why my new sorting algorithm outperforms quicksort in certain instances. Furthermore, they'll want to help my project by contributing lots of unit tests.

These answers might lead you to formulate a plan like the following:

*   Link to references about quicksort or other sorting algorithms, but don't explain them in the document.
*   Explain my sorting algorithm.
*   Explain the circumstances in which my sorting algorithm outperforms quicksort.
*   Get other people interested in helping.
