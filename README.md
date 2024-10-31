version: 2.1 
jobs: 
  build: 
    docker: 
      - image: circleci/ruby:2.6 
    parallelism: 1 
    steps: 
      - checkout 
      - run:  
          name: Build packages 
          command: | 
                  sc mining
