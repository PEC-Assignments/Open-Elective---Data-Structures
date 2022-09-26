# Assignment 2 - Circular Linked List

## Question 1.

#### Q1. While traversing a single-circular linked list, which condition establishes that the traversing element/variable has reached the first element?

## Answer:

- While Traversing a single-circular linked list, when the traversing element/variable reaches the value of the pointer of the head node then it establishes that the traversing element/variable has reached the first element.

   ![Circular Linked List](https://static.javatpoint.com/ds/images/circular-singly-linked-list.png)

   ```python

    def printList(self):
        """Function to print nodes in a given Circular Linked List."""

        temp = self.head        # Assigning head node to temp variable.
  
        # If linked list is not empty
        if self.head is not None:

            while(True):
            
                # Print nodes till we reach first node again
                print(temp.data, end=" ")    # Print data of current node.

                temp = temp.next            # Assigning next node to temp variable.

                # *****This is the condition that establishes that the traversing element/variable has reached the first element.*****
   
                if (temp == self.head):     # If temp variable reaches head node again.
                    break
   ```

---

## Question 2.

### Q2. What are the practical applications of a circular linked list?

## Answer:

- # Some of the practical applications of a circular linked list are:
    
    1. ## Working of Time Sharing Operating Systems.
        
        When more than one task is given by the user, then the division of CPU time for each process is decided by the operating system using Circular Linked Lists.

        ![Time Sharing Operating Systems](https://d1whtlypfis84e.cloudfront.net/guides/wp-content/uploads/2021/01/04130304/Screenshot-856-768x418.png)

    2. ## Used in Multiple Player board game.
        In a multiple player board game, the circular linked list is used to keep track of the players.

        ![Multiple Player board game](https://herluf-ba.github.io/images/turn-based/chess-position.webp)

    3. ## Image Viewer.
        
        In an image viewer, the circular linked list is used to keep track of the images. Previous and next images are linked, hence can be accessed by the next and previous button.

        ![Image Viewer](https://www.techsupportall.com/wp-content/uploads/2018/11/Windows-Photo-Viewer.png)

    4. ## Previous and next page in a web browser

        In a web browser, the circular linked list is used to keep track of the previous and next page. We can access the previous and next URL searched in a web browser by pressing the back and next buttons since they are linked as a linked list.

        ![Previous and next page in a web browser](https://www.pcworld.com/wp-content/uploads/2021/09/pcw-broswers-hero-100838277-orig.jpg?resize=1240%2C826&quality=50&strip=all)

    5. ## Music Player
    
        In a music player, the circular linked list is used to keep track of the songs. Songs in the music player are linked to the previous and next songs. you can play songs either from starting or ending of the list.

        ![Music Player](https://i.pinimg.com/originals/39/e5/fe/39e5fe1aa42d87d29fd9810faa6afba2.jpg)


    6. ## Undo and Redo
   
        In a text editor, the circular linked list is used to keep track of the undo and redo operations. The undo and redo operations are linked to the previous and next operations.

        ![Undo and Redo](https://miro.medium.com/max/828/1*2hvA5ZGL1anqr-Bpx-gweQ.jpeg)
