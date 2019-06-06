book social app

\*USER
name
username-email?
password_digest

has_many :books
has_many :book, through: :books
has-one or belongs_to :home, class_name: "book"?

\*BOOKS
name,author
belongs_to book?

\*BOOK
name,author,description
belongs_to :books

\*REVIEWS
content,rating
belongs_to :user
belongs_to :book

rails new book-fellow --api
rails g scaffold user name username password_digest
