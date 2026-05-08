# C# Data Structures & Collections Cheat Sheet

## List<T>
- Use when:
  - Need dynamic size
  - Need index-based access
  - General-purpose collection
- Best for:
  - Most applications
- Time Complexity:
  - Access → O(1)
  - Search → O(n)
  - Insert at end → O(1)

---

## Array (T[])
- Use when:
  - Size is fixed
  - Maximum performance needed
- Best for:
  - Performance-critical code
- Time Complexity:
  - Access → O(1)
  - Search → O(n)

---

## Dictionary<TKey, TValue>
- Use when:
  - Need fast lookup by key
  - Need key-value storage
- Best for:
  - User data
  - APIs
  - Caching
- Time Complexity:
  - Search → O(1)
  - Insert → O(1)
  - Delete → O(1)

---

## HashSet<T>
- Use when:
  - Need unique values
  - Need duplicate checking
- Best for:
  - Tags
  - Unique IDs
- Time Complexity:
  - Search → O(1)
  - Insert → O(1)

---

## Stack<T>
- Type:
  - LIFO (Last In First Out)
- Use when:
  - Need undo/backtracking behavior
- Best for:
  - Undo feature
  - Browser history
  - Expression evaluation
- Time Complexity:
  - Push → O(1)
  - Pop → O(1)

---

## Queue<T>
- Type:
  - FIFO (First In First Out)
- Use when:
  - Need sequential processing
- Best for:
  - Task queues
  - Scheduling systems
  - Printer queue
- Time Complexity:
  - Enqueue → O(1)
  - Dequeue → O(1)

---

## PriorityQueue<TElement, TPriority>
- Use when:
  - Need priority-based processing
- Best for:
  - Job scheduling
  - Dijkstra algorithm
- Time Complexity:
  - Insert → O(log n)
  - Remove highest priority → O(log n)

---

## LinkedList<T>
- Use when:
  - Frequent insert/delete operations
  - Less random access needed
- Best for:
  - Music playlists
  - Navigation systems
- Time Complexity:
  - Insert/Delete → O(1)
  - Search → O(n)

---

## SortedSet<T>
- Use when:
  - Need sorted unique values
- Best for:
  - Rankings
  - Ordered collections
- Time Complexity:
  - Insert/Search/Delete → O(log n)

---

## SortedDictionary<TKey, TValue>
- Use when:
  - Need sorted key-value pairs
- Best for:
  - Ordered records
- Time Complexity:
  - Search/Insert/Delete → O(log n)

---

# Quick Decision Guide

| Requirement | Best Choice |
|---|---|
| Dynamic collection | List<T> |
| Fixed-size collection | T[] |
| Fast key lookup | Dictionary<TKey, TValue> |
| Unique items | HashSet<T> |
| Undo / Backtracking | Stack<T> |
| FIFO processing | Queue<T> |
| Priority handling | PriorityQueue<TElement, TPriority> |
| Frequent insert/delete | LinkedList<T> |
| Sorted unique values | SortedSet<T> |
| Sorted key-value pairs | SortedDictionary<TKey, TValue> |

---

# Most Commonly Used in Real Projects

1. List<T>
2. Dictionary<TKey, TValue>
3. HashSet<T>
4. Queue<T>
5. Stack<T>

---

# Rule to Choose a Data Structure

Ask:
> Which operation should be fastest?

- Fast lookup → Dictionary
- Unique checking → HashSet
- Ordered access → List
- Undo functionality → Stack
- Sequential processing → Queue
- Priority execution → PriorityQueue
- Frequent insert/delete → LinkedList
