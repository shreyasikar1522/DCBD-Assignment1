# DCBD Assignment 1 : RPC and Map Reduce
# Analyzing Publication Metadata via RPC (MapReduce)

## Objective
This project implements a MapReduce-based solution to identify the Top 10 most frequent first words from publication titles (pub_0.txt to pub_999.txt), retrieved from a remote RPC server.

## Approach

### Architecture
- MapReduce paradigm
- Parallel processing using Python multiprocessing (Pool)

### Workflow
1. Authentication  
   Obtain a secret key using the /login endpoint.

2. Data Retrieval  
   Fetch publication titles using the /lookup endpoint.

3. Map Phase  
   Extract the first word from each title and compute local frequency counts.

4. Reduce Phase  
   Combine results from all workers to compute global frequencies.

5. Top 10 Extraction  
   Identify the 10 most frequent first words.

6. Verification  
   Submit results to the /verify endpoint.

## Technologies Used
- Python 3
- multiprocessing
- requests

## Project Structure
