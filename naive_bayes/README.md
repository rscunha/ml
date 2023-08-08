# Naive Bayes Classifier

Naive Bayes is a simple technique for constructing classifiers, for example:

Imagine a test where we are going to validate wheter or not the person has cancer, this test has an acuracy of 90% when the people does or does not have cancer, i.e he hits 90% when the person have cancer and he also hits 90% when the person does not have cancer.

So if a survey ask you: What´s the chance that you will get cancer?
Most of the people will respond that is 90%, because if the test has 90% of acuracy so the chance that I do have cancer is 90%. But this answer is very far from the correct answer, because to get the correct answer we need to know how many people in the population have cancer.

Follow the explanation:

Total population: 1000
Test acuracy: 90%
Population that get cancer: 1%

So,

Population that does not have cancer: 990
Population that has cancer: 10

If all that population does the test the result will be:

Out of the 990 who do not have cancer:
 - 891 test results will be that the person does not have cancer
 - and 99 test results will be that the person has cancer (in this case the test failed)


Out of the 10 who has cancer:
 - 9 test results will be right, the person has cancer
 - and 1 test result will be wrong, the test will say the person does not have cancer

 Now, how many people have cancer?

Out of 10 that have cancer, 9 got the test right, and out of 990 the test failed and the result was that 99 people had cancer, so 108 people were diagnosed with cancer. But of these 108, how many actually had cancer? Look at this, only 9 people got cancer out of those 108. Therefore if you were diagnosed with cancer, you are among those 108 people, so the probability that you get cancer is 9/108 (it is about basic probability) and the bottom line is 8.3% of chance of getting cancer.

The Naive Bayes algorithm creates a generic formula from a problem like this one and you will apply the same solution to any problem of this type that you  want to solve. See below the Naive Bayes Formula:

P(A/B) = (P(B/A) * P(A)) / P(B/A) * P(A) + P(B/!A) * P(!A)

Anoter important concept about this theorem is because we can have three diferents types of problems of probability:

    - 1. Calculation with discret number, (1,2,3,4)
    - 2. Calculation with discret numbers and binary values for target variable
        - whole numbers for predictos variables (1,2,3,4)
        - binary values for target variable (0,1)
    - 3. Calculation with continuous numbers (1.2, 3.4, 5.6)

For each of the type of problems we´ll need a diferent function, respectively:

    - 1. MultinomialNB
    - 2. BernoulliNB
    - 3. GaussianNB
