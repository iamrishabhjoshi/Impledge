
# Longest Compound Word Finder

**Longest Compound Word Finder**

**Overview:**

The provided Java program calculates the longest and second longest words in a text file that can be constructed by concatenating shorter words also found in the file. It also calculates the total number of compound words. The program utilizes a trie data structure to efficiently process the words in the input file.

**Execution Steps:**

1. Ensure you have the Java runtime environment installed on your system.
2. Compile the Java program using a Java compiler. You can use the `javac` command:

   ```shell
   javac LongestCompoundWord.java
   ```

3. Run the compiled program, providing the input text file name as an argument. For example, to process a file named "words_for_problem.txt," use:

   ```shell
   java LongestCompoundWord words_for_problem.txt
   ```

**Design Decisions and Approach:**

1. The program uses a Trie data structure to efficiently process words from the input file. The Trie allows for efficient prefix and suffix lookups, which is crucial for identifying compound words.

2. It reads words from the input file, fills up a queue with words that have suffixes (candidates for compound words), and inserts each word into the Trie.

3. The program processes the words and their suffixes using a queue-based approach. It explores words that might be prefixes of other words in the file.

4. For each word, it checks for suffixes and adds them to the queue if found. If no suffixes are found, it discards the pair and continues with the next pair.

5. The program maintains records of the longest and second longest compound words found during processing.

6. The total processing time is calculated and displayed in milliseconds.


