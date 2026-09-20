Leetcode Problems:

**1832, pangram. (Membership only)**
---
A set tells you what's present; check its size for the answer.

Functions: `.add()` put chars in, `.size()` checked for all 26, `.charAt()` pulled each char.

**771, Jewels and Stones. (Membership plus counting)**
---
The set answers "is it in the group," a separate counter tallies how many passed.

Functions: `.add()` built the set, `.contains()` checked each stone, `.charAt()` pulled each char.

**49,Group Anagrams.(Grouping)**
---
If you need both the original string + an altered version, just make a quick copy of it using toCharArray().

Note, this will make a array of characters that you can sort, or alter as you choose.

But if you need it in string format you'll need to turn it back via
passing the array into a String delaration.

eg: String key = new String(ArrayofTheCharCopy)

Also, if you need to append a value to a hashmap value thats a array.
you need to call the value then append using .add

eg: map.get(key).add(StringYouWanttoADD)

Last, If the hashmap expects an array as a value, you need to add the first value as an array value.

YOu do this by making an array and adding the value you need in that array then passing the WHOLE array into the HashMap Value
eg:

List<String> group = new ArrayList<>();
group.add(strs[i]);
map.put(key,group);