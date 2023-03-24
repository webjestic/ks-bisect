# Using GIT Bisect

WHICH COMMIT WAS THIS ADDED?

You should be able to find the commit hash tag in less than 5 bisect moves.

Your other option might be to checkout every commit yourself until you finally find it. This may not be so bad
for this example exercise, but would be horrible if you had to compule and execute tests in a simulator.

## Introduction

I've created a [GIT cheatsheet](https://gist.github.com/webjestic/2a011d505335de09f5b2fb472a4bc990) to use, so I'll 
always have it, because my memory isn't what it used to be.

## GIT Bisect 

Works great for quickly finding a bug that was introduced, but at an unknown time.

{{FINDME}}

Step 1 - Read the [Bisect Debugging Section](https://gist.github.com/webjestic/2a011d505335de09f5b2fb472a4bc990#bisect-debugging)
Step 2 - Ensure no changes are pending in your active branch
Step 3 - Start the bisect process
Step 4 - Mark the top commit as bad
Step 5 - Mark a commit as good `git bisect bad`
Step 5a - `git log --oneline`
Step 5b - git checkout 415dfc6
Step 5c - if checkouted out branch does not have bug, mark as good `git bisect good`
Step 6 - Repeat processes

## Off Topic Tips

- Using `await` does not block the main thread.
- Does adding `async` to a normal function turn it into a promise?

