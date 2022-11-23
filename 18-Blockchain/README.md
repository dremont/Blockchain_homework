# Pychain Ledger 

# Author: Andre Montgomery 

# Instructions

1. Create a new data class named `Record`. This class will serve as the blueprint for the financial transaction records that the blocks of the ledger will store.

2. Modify the existing `Block` data class to store `Record` data.

3. Add Relevant User Inputs to the Streamlit interface.

4. Test the PyChain Ledger by Storing Records.

# Files

Download the following files to help you get started:

[Module 18 Homework files](Starter_Code/pychain.py)

You will also need to run the program using command streamlit run pychain.py 


### Step 1: Create a Record Data Class


@dataclass
class Record:
    sender: str
    receiver: str
    amount: float


### Step 2: Modify the Existing Block Data Class to Store Record Data

@dataclass
class Block:

   record: Record


### Step 3: Add Relevant User Inputs to the Streamlit Interface

input_data = st.text_input("Block Data")
sender = st.text_input("Sender")
receiver = st.text_input("Receiver")
amount = st.text_input("Amount")

### Step 4: Test the PyChain Ledger by Storing Records
<img width="1394" alt="sender_receiver" src="https://user-images.githubusercontent.com/18622578/203456826-9bd22cec-8ecb-4f06-a0e1-beb63fae205a.png">
<img width="1427" alt="validation" src="https://user-images.githubusercontent.com/18622578/203456865-b6f93b4c-b645-43e2-9ff3-41ae69b9bb7a.png">
