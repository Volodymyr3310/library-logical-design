# Logical Design — Library Management System

## ER Diagram

The system contains the following entities:

- **Book**: id, title, author, genre
- **Reader**: id, full_name, email
- **Librarian**: id, full_name, department
- **Issue**: id, issue_date, return_date, book_id, reader_id, librarian_id

### Relationships

- A reader can have multiple issued books.
- A librarian processes multiple issues.
- Each issue is related to one book.

*(See `er_diagram.png` for details)*

---

## DFD Diagram

The Data Flow Diagram (DFD) includes the following elements:

- **External entities**: Reader, Librarian
- **Processes**:
  1. Check book availability
  2. Register book issue
- **Data stores**: Book DB, Issue DB

*(See `dfd_diagram.png` for visual representation)*
