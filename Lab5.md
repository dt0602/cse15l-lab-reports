# Researching `less`

The command `less` allows the user to view the contents of a file one page at a time. To access further pages in the file, we hit `<enter>`, and to quit or exit out of the file contenet, we hit `<q>`.

Command-line options using `less`:

### 1. `less -E file.txt`
#### Example 1: 
input: `less -E Cancun-History.txt`

output: <img width="1000" alt="image" src="https://user-images.githubusercontent.com/122497642/224833054-1183a518-49c6-4378-ab74-3d6e273e1a7c.png">

#### Example 2:
input: `less -E Bali-WhatToDo.txt`

output: <img width="1000" alt="image" src="https://user-images.githubusercontent.com/122497642/224833461-a18be2ec-3ca1-4eb2-9aad-bd7eeb105b9f.png">

`less -E file.txt` allows the terminal to automatically exit once it reaches the end of the file. This command is useful because it allows more convenience for the user to exit a file without having to do extra work into getting out of the file content. For users that do not know how to get out of the terminal by entering `<q>`, this command removes the trouble. The user can still hit `<q>` if they want to exit the file early, or continue hitting `<space>` or the `<down>` arrow until the file automatically exits.

Citation: [Link](https://phoenixnap.com/kb/less-command-in-linux)

### 2. `less -N file.txt`
#### Example 1:
input: `less -N Bali-WhatToDo.txt`

output: <img width="1197" alt="image" src="https://user-images.githubusercontent.com/122497642/224839150-bd9a4ae5-0f61-4396-8207-87b86ca8ec74.png">
<img width="1197" alt="image" src="https://user-images.githubusercontent.com/122497642/224839198-b26102d2-e258-4f71-8ed1-c6575076c6e4.png">
<img width="1175" alt="image" src="https://user-images.githubusercontent.com/122497642/224839251-6474a3df-768d-418e-9f69-eb2242002ca5.png">

#### Example 2:
input: `less -N Nepal-History.txt`

output: <img width="1196" alt="image" src="https://user-images.githubusercontent.com/122497642/224839460-109ba204-1025-40ce-b135-964ab60b1473.png">
<img width="1193" alt="image" src="https://user-images.githubusercontent.com/122497642/224839505-61b51810-3090-49ce-af7d-c4b314e3aa02.png">
<img width="1149" alt="image" src="https://user-images.githubusercontent.com/122497642/224839598-56b10715-a8a2-4fd9-a5fc-3b93aeba34ea.png">

`less -N file.txt` displays the line numbers of the given file along with the content of the file. This command is useful for users to identify specific lines of text for a file of any size. It also helps the user keep track of specific parts of the file. The user can hit `<space>` to access other pages in the file and still hit `<q>` to exit the file.

Citation: [Link](https://phoenixnap.com/kb/less-command-in-linux)

### 3. `less -X file.txt`
#### Example 1:
input: `less -X Bali-WhatToDo.txt`

output: <img width="1198" alt="image" src="https://user-images.githubusercontent.com/122497642/224841269-0ee0d28e-6dcc-4b07-a21d-0f9ccf197992.png">
<img width="1195" alt="image" src="https://user-images.githubusercontent.com/122497642/224841621-1645f24a-8f48-4c7e-9eb1-76f4470b4f06.png">

#### Example 2:
input: `less -X Nepal-History.txt`

output: <img width="1187" alt="image" src="https://user-images.githubusercontent.com/122497642/224841762-b883cd5d-d668-4475-b526-1f32dfec90ec.png">
<img width="1196" alt="image" src="https://user-images.githubusercontent.com/122497642/224841807-bafe6c74-504d-43ba-a905-e4af1eb7cd38.png">

`less -X file.txt` disables clearing the contents of the file on the terminal screen. This is a useful command because it allows the user to view the entire contents of a file all at once, without having to manually scroll through the file. In order to exit and be able to enter new commands in the terminal, the user can still enter `<q>`.

Citation: [Link](https://phoenixnap.com/kb/less-command-in-linux)

### 4. `less file1.txt file2.txt`

#### Example 1: 
input: `less Berlin-History.txt Berlin-WhatToDo.txt`

output: <img width="1199" alt="image" src="https://user-images.githubusercontent.com/122497642/224867690-77ff48a5-2245-427e-af1b-f3f4d8a512b5.png">
<img width="1191" alt="image" src="https://user-images.githubusercontent.com/122497642/224867716-09154d29-3ee8-4b4d-8190-bae8dbe2b047.png">
<img width="1198" alt="image" src="https://user-images.githubusercontent.com/122497642/224867735-e54943ef-7604-48c7-940f-25e0053c65d7.png">
<img width="1200" alt="image" src="https://user-images.githubusercontent.com/122497642/224867762-44b3d34c-7e3c-4b80-8df3-df15f344c3a5.png">

#### Example 2:
input: `less Nepal-WhatToDo.txt Nepal-WhereToGo.txt`

output: <img width="1200" alt="image" src="https://user-images.githubusercontent.com/122497642/224867797-9ea60d70-d551-42c2-9b24-a68bc8216dc8.png">
<img width="1197" alt="image" src="https://user-images.githubusercontent.com/122497642/224867821-da65c4c1-a458-4ffb-952c-9a099dd7c1db.png">
<img width="1195" alt="image" src="https://user-images.githubusercontent.com/122497642/224867850-98f03956-124f-41b6-995c-033a2001e19f.png">
<img width="1198" alt="image" src="https://user-images.githubusercontent.com/122497642/224867877-85753bd7-be00-428b-924f-82185abcad51.png">


`less file1.txt file2.txt`

Citation: [Link](https://phoenixnap.com/kb/less-command-in-linux)
