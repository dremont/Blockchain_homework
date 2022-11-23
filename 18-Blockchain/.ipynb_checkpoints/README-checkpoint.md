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

# @TODO:
# Delete the `input_data` variable from the Streamlit interface.
input_data = st.text_input("Block Data")

# @TODO:
# Add an input area where you can get a value for `sender` from the user.
sender = st.text_input("Sender")

# @TODO:
# Add an input area where you can get a value for `receiver` from the user.
receiver = st.text_input("Receiver")

# @TODO:
# Add an input area where you can get a value for `amount` from the user.
amount = st.text_input("Amount")

### Step 4: Test the PyChain Ledger by Storing Records
18-Blockchain/sender_receiver.png
18-Blockchain/validation.png