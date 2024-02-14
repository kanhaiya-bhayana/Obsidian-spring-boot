- One-to-one
- One-to-Many, Manty-to-One
- Many-to-Many
***By default no operations are cascaded*** - DEFINE EXPLICITLY

##### Fetch Types: Eager vs Lazy Loading
- When we fetch / retrieve data, should we retrieve EVERYTHING?
	- Eager will retrieve everything
	- Lazy will retrieve on request - will load the main entity first and load dependent entity on demand (lazy)
- ***Best Practice: Only load data when absolutely needed*** - Prefer Lazy loading instead of Eager loading

###### Default Fetch Types
	@OneToOne - FetchType.EAGER
	@OneToMany - FetchType.LAZY
	@ManyToOne - FetchType.EAGER
	@ManyToMany - FetchType.LAZY
	***We can overrides the defaults value by defining the explicit mapping***

The JOIN FETCH is similar to the EAGER loading   

Join Table
	A table that provides a mapping between two tables.
		It has foreign keys for each table to define the mapping relationship.


##### JoinInverseColumn ----- ?