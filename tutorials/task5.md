### @flyoutOnly 1


# Fish collector


## Step 1

In this task, we need to move clownfish and pufferfish from the ship, over onto the pier.
First though, lets go collect some fish. Use the ``||agent:agent move forward 2||`` command 
to position your Agent over a fish collection point. 
Then use the ``||agent:agent collect CLOWNFISH||`` 
command to pick up only clownfish for now.

```blocks
agent.move(LEFT, 1)
agent.move(FORWARD, 2)
agent.collect(CLOWNFISH)
```

## Step 2
With some clownfish now collected, lets also collect clownfish from the rest of
the pickup points. Why not try and put your code in a ``||loops:Repeat 3 times loop||`` 
(a ``||loops:for loop||`` in Python).

```blocks
agent.move(LEFT, 1)
for (let index = 0; index < 3; index++) {
    agent.move(FORWARD, 2)
    agent.collect(CLOWNFISH)
}

```

## Step 3
With all your clownfish now collected, next write a program to take your Agent
over to the correct drop off point on the pier and use the ``||agent:agent drop all down||``
command to drop all the fish into the bucket.

```ghost
agent.dropAll(FORWARD)
```

## Step 4
Try putting all this within a ``||loops:Repeat times loop||`` to keep picking up 
fish and droping them off.

## Step 5
Finally, replicate the same process to handle pufferfish. It is recommended to do
this separately.
