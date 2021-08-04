```python
def outer(f):
	@wraps(f)
	def inir(*args,**kwargs):
		user=None
		kwargs["user"]=user
		return f(*args,**kwargs)
	return inir
```
