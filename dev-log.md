book social app (for children's books-educational, beginner readings)

\*USER
name
username
password_digest

has_many :books
has_many :reviews

\*BOOK
name,author,description
has_many :reviews
has_many :users

\*REVIEW
content,rating
belongs_to :user
belongs_to :book

rails new book-fellow --api
rails g scaffold user name username password_digest
Domain ideas:
bank app
house sale
apps review
