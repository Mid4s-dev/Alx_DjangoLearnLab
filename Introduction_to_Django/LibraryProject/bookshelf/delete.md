from bookshelf.models import Book

# Delete the book and confirm deletion
book = Book.objects.get(title="Nineteen Eighty-Four")
book.delete()
Book.objects.all()

# Expected output: <QuerySet []>
