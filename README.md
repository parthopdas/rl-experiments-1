# TODO: \<Project Name\>

## Environment setup

- Create new environment
  - Setup conda
    ```sh
    conda deactivate
    conda env remove --name rl.gym.1
    conda create --name rl.gym.1 python=3.6
    conda activate rl.gym.1
    ```
  - Install dependencies
    ```
    conda install pylint pywin32 jupyter pycodestyle
    conda install pandas scikit-learn scipy numpy seaborn matplotlib
    # conda install spacy gensim nltk # For NLP 
    conda install pytorch torchvision cudatoolkit=10.1 -c pytorch # For CUDA 10.2
    ```
- Export environment
  ```sh
  conda env export --name rl.gym.1 >.environment.yml
  ```

- Import environment
  ```sh
  conda env create -f .environment.yml
  ```

- Load anaconda: 
  ```sh
  & 'C:\Users\partho\Anaconda3\shell\condabin\conda-hook.ps1' ; conda activate 'C:\Users\partho\Anaconda3' ; cd d:\src\c
  ```
