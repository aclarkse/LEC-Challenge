###################################################################################################

class 1st LEC Data Challenge 2019:

    """
    information about
    ---------------------------
    datasets
    task
    submission
    evaluation
    important facts
    """

    ####-------------------------------------------------------------------------------------------
    def datasets(challenge.zip):
    {
        number_of_datasets(challenge.zip) = 3
        dimension(training_dataset.csv, test_dataset.csv) = (639, 15)

        if dataset == training_dataset.csv:
            information = training dataset with two groups of faulty measurements
        if dataset == training_solution.csv:
            information = values 0 and 1 indicating the faults (value = 1) in the training dataset
        if dataset == test_dataset.csv:
            information = test dataset where different channels at different records are faulty
    }

    ####-------------------------------------------------------------------------------------------
    def task(datasets):
    {
        task = determine which data points of the test dataset are faulty and which are fault-free
        hint = both channel (column) and record number (row)
    }

    ####-------------------------------------------------------------------------------------------
    def submission(solution):
    {
        if(motivation == big)
        {
            deadline(pre_submission) = July 15, 2019
        }

        deadline(final_submission) = August 19, 2019
       
        form(submission)     = csv-file           # 300 rows and 15 columns
        values(submission)   = 1 or 0             # 1 = faulty, 0 = fault free
        name(submission)     = test_solution
    }

    ####-------------------------------------------------------------------------------------------
    def evaluation(submission):
    {
        tp=#(true positive); fp=#(false positive); tn=#(true negative); fn=#(false negative)
        result     = (tp + tn)/(tp + fp + fn + tn)*100     # number of correctly classified points
        max_result = 100                                   # best possible performance

        if submission == intermediate_submission:
            feedback_deadline = July 29, 2019
        if submission == final_submission:
            feedback_deadline = September 5, 2019
    }

    ####-------------------------------------------------------------------------------------------
    def important_facts(challenge):
    {
        e-mail  = data.challenge@lec.tugraz.at
        website = www.lec.at/datachallenge
    }

###################################################################################################