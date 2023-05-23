# Day 1 Rainbow Builder

```template

player.onChat("rainbow", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
})
player.onChat("tower", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
})
```

## Rainbow Builder

In this activity, you will show what you learned about sequences by coding the agent to build some rainbows!
We'll make a rainbow across the ground AND a rainbow tower!

## Step 1

Two ``||player.on chat command||`` blocks have been provided for you. They should both already contain a block to teleport the agent to you. Confirm that your template looks correct before proceeding. Use the HINT to check! 
```blocks
player.onChat("rainbow", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
})
player.onChat("tower", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
})
```

## Step 2

After the agent teleports to the player, what is the first thing the agent should do to build a rainbow? Can it place a block if it's not holding anything? Look through the ``||agent||`` blocks to see if you can find the right block to add to the code.

```blocks
player.onChat("rainbow", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
    agent.setItem(GRASS, 1, 1)
})
```

## Step 3

Now that we can set what block the agent is holding, what color of concrete should it start with? What's the first color in the rainbow?

```blocks
player.onChat("rainbow", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
    agent.setItem(RED_CONCRETE, 1, 1)
})
```

## Step 4

Now that the agent is holding the right block, what should it do with the concrete? Look through the ``||agent||`` blocks to see if you can find the right block to add to the code.

```blocks
player.onChat("rainbow", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
    agent.setItem(RED_CONCRETE, 1, 1)
    agent.place(FORWARD);
})
```

## Step 5

The first block will now be placed! What should the agent do next? Can it place the block in the same place or should it move sideways first? Look through the ``||agent||`` blocks to see if you can find the right block to add to the code.

```blocks
player.onChat("rainbow", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
    agent.setItem(RED_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
})
```

## Step 6

Now we have code for the agent to place the first block and move to the next spot. Can it place a block right away? No, we need to get the next color of concrete first! Get the Orange Concrete!

```blocks
player.onChat("rainbow", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
    agent.setItem(RED_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(ORANGE_CONCRETE, 1, 1)
})
```

## Step 7

The agent is in the right place and is holding the right block, what should it do?

```blocks
player.onChat("rainbow", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
    agent.setItem(RED_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(ORANGE_CONCRETE, 1, 1)
    agent.place(FORWARD);
})
```

## Step 8

It seems like there there are 3 steps to placing a block in the rainbow. One, move to the right place. Two, get the right block. Three, place the block. We just placed a block. What should the agent do next? Try adding all 3 steps on your own for Yellow!

```blocks
player.onChat("rainbow", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
    agent.setItem(RED_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(ORANGE_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(YELLOW_CONCRETE, 1, 1)
    agent.place(FORWARD);
})
```

## Step 9

You added the blocks we needed for Yellow, now try Lime Green! One, move to the right place. Two, get the right block. Three, place the block.

```blocks
player.onChat("rainbow", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
    agent.setItem(RED_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(ORANGE_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(YELLOW_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(LIME_CONCRETE, 1, 1)
    agent.place(FORWARD);
})
```

## Step 10

Only 2 colors to go, try Light Blue! One, move to the right place. Two, get the right block. Three, place the block.

```blocks
player.onChat("rainbow", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
    agent.setItem(RED_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(ORANGE_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(YELLOW_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(LIME_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(LIGHT_BLUE_CONCRETE, 1, 1)
    agent.place(FORWARD);
})
```

## Step 11

Last color! Add the last 3 blocks for purple! One, move to the right place. Two, get the right block. Three, place the block.

```blocks
player.onChat("rainbow", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
    agent.setItem(RED_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(ORANGE_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(YELLOW_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(LIME_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(LIGHT_BLUE_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(RIGHT, 1);
    agent.setItem(PURPLE_CONCRETE, 1, 1)
    agent.place(FORWARD);
})
```

## Step 12

You'll have more to do, so don't forget to come back, but it's time to test out the rainbow command! Stand in front of the red concrete in the floor and type "rainbow" in chat!

## Step 13

If your code didn't work, check the hints in the previous steps first, then ask a friend or a Sensei for help. Once your rainbow command is working, it's time for you to take on one more challenge.

## Step 14

You have an example of a block placing sequence from making the rainbow command, can you fill in the tower command to recreate the rainbow tower?
Remember that you need to build up and down, not sideways! There are multiple solutions, so feel free to try out your ideas!

## Activity Complete!

You did it! You learned about Sequences and coding the agent in Minecraft!

```blocks
player.onChat("tower", function () {
    agent.teleport(pos(0, 0, 0), orientation.WEST)
    agent.setItem(PURPLE_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(UP, 1);
    agent.setItem(LIGHT_BLUE_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(UP, 1);
    agent.setItem(LIME_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(UP, 1);
    agent.setItem(YELLOW_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(UP, 1);
    agent.setItem(ORANGE_CONCRETE, 1, 1)
    agent.place(FORWARD);
    agent.move(UP, 1);
    agent.setItem(RED_CONCRETE, 1, 1)
    agent.place(FORWARD);
})
```
