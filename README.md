# README #

Labs for "TDA596 - Distributed Systems" course

### What is this repository for? ###

We implemented a distributed blackboard application, using a subset of the Python programming language. Starting from a simple (barely working) implementation, it will evolve over the labs to a fully working distributed application with different properties. We tested our implementation on the Seattle platform, a platform for networking and distributed systems teaching & research. In the context of these labs, Seattle allows us to run and evaluate our implementation on different machines distributed around the world.

### Seattle platform ###

Seattle is a platform for networking and distributed systems research. It's free, community-driven, and offers a large deployment of computers spread across the world. Seattle operates on resources donated by users and institutions. The global distribution of the Seattle network provides the ability to use it in application contexts that include cloud computing, peer-to-peer networking, ubiquitous/mobile computing, and distributed systems. Seattle nodes run code written in a special language called Repy. Repy is a subset of the Python language (v2.5, v2.6) invented specifically for Seattle. ([site](https://seattleclearinghouse.poly.edu))

### Running programs in Seattle ###

To run a Repy program from the command line, we type the following with the correct values substituted in:
```
python <path to repy.py> <path to restrictions file> <path to source file>
```

But first we have to execute once “start_seattle.sh” by typing the command:
```
./start_seattle.sh
```

Step 1: Run programs in the Seattle – Run Seash in python mode
```
python seash.py
```

Step 2: Log in with our key by loading the public and private key downloaded from Seattle Clearinghouse
```
!> loadkeys vtaxiarchis !> as vtaxiarchis vtaxiarchis@ !>
```

Step 3. Locate the resources (computers) that we have created in the Seattle Clearinghouse
```
vtaxiarchis@ !> browse
```

Step 4. Access the resources (VMs) in the Seattle Clearinghouse
```
vtaxiarchis@ !> on browsegood
```

Step 5. Upload a Repy program in the Seattle Clearinghouse
```
vtaxiarchis@ !> upload example.repy
```

Step 6. Run a program (“Hello world”)
```
vtaxiarchis@browsegood !> run example.repy
```

Step 7. Look up the result of the program executed
```
vtaxiarchis@browsegood !> show log
```

Step 8. Look up the information about the VMs we control
```
vtaxiarchis@browsegood !> list
```

Step 9. Exit from Seash
```
vtaxiarchis@browsegood !> exit
```
