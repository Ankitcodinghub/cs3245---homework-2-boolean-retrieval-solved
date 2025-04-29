# cs3245---homework-2-boolean-retrieval-solved
**TO GET THIS SOLUTION VISIT:** [CS3245 – Homework #2 Â» Boolean Retrieval Solved](https://www.ankitcodinghub.com/product/cs3245-homework-2-a-boolean-retrieval-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;114624&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS3245 - Homework #2 Â» Boolean Retrieval Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
In Homework 2, you will be implementing indexing and searching techniques for Boolean retrieval described in Lectures 2 and 3.

Indexing

Your indexing script, index.py, should be called in this format:

$ python3 index.py -i directory-of-documents -d dictionary-file -p postings-file

Documents to be indexed are stored in directory-of-documents. In this homework, we are going to use the Reuters training data set provided by NLTK. Depending on where you specified the directory for NLTK data when you first installed the NLTK data (recall that the installation is triggered by nltk.download()), this data set is located under a path like:

…/nltk_data/corpora/reuters/training/

Recall that the dictionary is commonly kept in memory, with pointers to each postings list, which is stored on disk. This is because the size of the dictionary is relatively small and consistent, while the postings can get very large when we index millions of documents. At the end of the indexing phase, you are to write the dictionary into dictionary-file and the postings into postings-file. For example, the following command writes the dictionary and postings into dictionary.txt and postings.txt.

$ python3 index.py -i nltk_data/corpora/reuters/training/ -d dictionary.txt -p postings.txt

Although you can use any file names as you like, in this homework please follow the above command to use dictionary.txt and postings.txt, so that our marking script can easily locate the files.

In order to collect the vocabulary, you need to apply tokenization and stemming on the document text. You should use the NLTK tokenizers

(nltk.sent_tokenize() and nltk.word_tokenize()) to tokenize sentences and words, and the NLTK Porter stemmer (class nltk.stem.porter) to do stemming. You need to do case-folding to reduce all words to lower case.

Skip Pointers

Searching

Here is the command to run your searching script, search.py:

$ python3 search.py -d dictionary-file -p postings-file -q file-of-queries -o output-file-of-results

dictionary-file and postings-file are the output files from the indexing phase. Queries to be tested are stored in file-of-queries, in which one query occupies one line. Your answer to a query should contain a list of document IDs that match the query in increasing order. In the Reuters corpus, the document IDs should follow the filenames (that is, your indexer should assign its document ID 1 to the filename named “1”; also note that while Reuters doc IDs are unique integers, they are not necessary sequential). For example, if three documents 12, 40 and 55 are found in the search, you should write “12 40 55” into output-file-of-results in one line. When no document is found, you should write an empty line. The results in output-file-of-results should correspond to the queries in file-of-queries.

The operators in the search queries include: AND, OR, NOT, (, and ). The operators will always be in UPPER CASE (lower case “and”s, “or”s and “not”s simply won’t occur in your data (but you should probably bulletproof your code anyways). You can safely assume that there are no nested parentheses, for example, the query (a AND (b OR c)) will not occur. However, there is only a light restriction on the length of the query (won’t be over 1024 characters but can be long). Note that parentheses have higher precedence than NOT, which has a higher precedence than AND, which has a higher precedence than OR. AND and OR are binary operators, while NOT is a unary operator. Below is an illustration of a valid example query: bill OR Gates AND (vista OR XP) AND NOT mac

While indexing is an off-line phase, searching is designed to be real-time (the extreme example is Google Instant), thus efficiency is very important in searching. In this homework, we won’t be evaluating based on how fast your program can index a list of documents (the preprocessing), but we will test the efficiency of your searching program (runtime speed), as well as its accuracy.

What to turn in?

You are required to submit index.py, search.py, dictionary.txt, and postings.txt. Please do not include the Reuters data.

Essay questions:

1. You will observe that a large portion of the terms in the dictionary are numbers. However, we normally do not use numbers as query terms to search. Do you think it is a good idea to remove these number entries from the dictionary and the postings lists? Can you propose methods to normalize these numbers? How many percentage of reduction in disk storage do you observe after removing/normalizing these numbers?

2. What do you think will happen if we remove stop words from the dictionary and postings file? How does it affect the searching phase?

Submission Formatting

You are allowed to do this assignment individually or as a team of two. There will be no difference in grading criteria if you do the assignment as a team or individually. For the submission information below, simply replace any mention of a student number with the two student numbers concatenated with a separating dash (e.g., A000000X-A000001Y).

For us to grade this assignment in a timely manner, we need you to adhere strictly to the following submission guidelines. They will help me grade the assignment in an appropriate manner. You will be penalized if you do not follow these instructions. Your student number in all of the following statements should not have any spaces and any letters should be in CAPITALS. You are to turn in the following files:

A plain text documentation file README.txt (e.g., in UPPERCASE): this is a text only file that describes any information you want me to know about your submission. You should give an overview of your system and describe the important algorithms/steps in your system. However, You should not include any identifiable information about your assignment (your name, phone number, etc.) except your student number and email (we need the email to contact you about your grade, please use your [u|a|g|e]*******@u.nus.edu address, not your email alias). This is to help you get an objective grade in your assignment, as we won’t associate student numbers with student names.

All source code. We will be reading your code, so please do us a favor and format it nicely.

(Optional) A plain text file ESSAY.txt that contains your answers to the essay questions (if you choose to attempt the questions). Again, do not disclose any identifiable information in your essay answers.

These files will need to be suitably zipped in a single file called &lt;student number&gt;.zip. Please use a zip archive and not tar.gz, bzip, rar or cab files. Make sure when the archive unzips that all of the necessary files are found in a directory called &lt;student number&gt;.

Grading Guidelines

The grading criteria for the assignment is tentatively:

50% Correctness of your code

20% Documentation

5% For following the submission instructions and formatting your documentation accordingly.

5% For code level documentation.

10% For your high level documentation, in your README document.

30% Evaluation: we will test the accuracy and querying speed of your searching program 0% Essay questions

Hints

In-memory indexing of a few documents, testing the Boolean operators for correctness.

Implementing the stemming, tokenization methods described.

Implementing postings disk-based indexing. Here you can separate the search and indexing parts into two files as suggested.

Implementing the skip pointers.

You’ll need to use the python (lower-)level file input/output commands, seek(), rewind(), tell() and read(). You must use these operations when coding search.py, and not rely on other modules (e.g., linecache).

How do you check the correctness of your results? Exchange queries with your peers! Suggest a few queries that you ran your system on, and post them and the results that you get to the Piazza forum (make sure you use the right topic heading).

Be aware of any differences in data type sizes on Tembusu vs. your development machine. To ensure the portability of your code, check and record the size of the data types in a variable and seek/read accordingly. We will not be responsible if your code works fine on your development machine, but not on Tembusu.

The Reuters corpus has some particularities (as does practically all corpora). There are some character escapes that occur in the corpus (&lt; for &lt;) but you can safely ignore then; you do not have to process these in any special way for this assignment.

Similarly, bulletproof your input and output. Make sure directories (e.g., arguments to -i) are correctly interpreted (add trailing slash if needed). Check that your output is in the correct format (docIDs separated by single spaces, no quotations, no tabs).
