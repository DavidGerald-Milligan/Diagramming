# MatcherFieldSpec  
 ![MatcherFieldSpec](./MatcherFieldSpec.png)

# MatcherQueryVisitor  
 ![Visitor](./Visitor.png)

# FilterFactory  
####This produces the VISITABLE filter.  
 ![Filter](./Filter.png)

# MatcherQuery  
 ![Query](./Query.png)
 
# FilterMapper  
 ![FilterMapper](./FilterMapper.png)
  
####  Usage example:  To filter a document on `CONTENT_PRIMARY` containing `address` 
    Filter<String> filter = FilterFactory.contains("CONTENT_PRIMARY", "address");
    MatcherQuery.isMatch(document, FilterMapper.map(filter, FieldNameMatcherFieldSpec::new));

