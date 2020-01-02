# UndoRedoList

An undo-redo data structure based on the concepts of `DoublyLinkedList` and behaves exactly the same way as undo-redo features do in for example Photoshop and Microsoft Word. 

[Regret](https://github.com/Muddz/Regret) an Android library is based on this data structure.

## How it works

The list adds elements in sequential order as a `LinkedList` would do when the pointer is standing at end of the list.

Adding on an existing <i>Head</i> element or between existing elements as shown in the example below will result in all elements to the right of and inclusive *element-2* being deleted and the new *element-6* taking the tail-position of the list

<img src="https://github.com/Muddz/UndoRedoList/blob/master/src/main/resources/AddBetweenElements.png" width="70%">

An element contains of an instance of the `Action` [class](https://github.com/Muddz/UndoRedoList/blob/master/src/main/java/Action.java)

## Performance
`UndoRedoList` is a linear data structure and has similar performance as Java's LinkedList.
The following is the *time-complexity* for the most important methods in `UndoRedoList`

- `add()` is always *O(1)* regardless of the pointer position
- `undo()` or `redo()` is *O(1)* because we can only traverse to the first next or previous node


## License

    Copyright 2019 Muddi Walid

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License
    You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
