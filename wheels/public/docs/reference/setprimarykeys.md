```coldfusion
setPrimaryKeys(property)
```
```coldfusion
// In `models/Subscription.cfc`, define the primary key as composite of the columns `customerId` and `publicationId`
<cffunction name="init">
    setPrimaryKeys("customerId,publicationId")>
</cffunction>
```