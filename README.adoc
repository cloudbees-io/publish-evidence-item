= CloudBees action: Publish evidence item.

Use this action to capture information that serves as evidence of work done by the workflow run.

== Inputs

[cols="2a,1a,1a,3a",options="header"]
.Input details
|===

| Input name
| Data type
| Required?
| Default value
| Description

| `content`
| String
| Yes
|
| Information to capture as an evidence item for the workflow run. The information is captured at the step level for the workflow run.

| `format`
| String
| No
| MARKDOWN
| Used to render the evidence item.

|===

== Usage example

In your YAML file, add:

[source,yaml]
----
      - name: Publish workflow evidence item
        uses: cloudbees-io/publish-evidence-item@v1
        with:
          content: some evidence item data
          format: MARKDOWN

----

== License

This code is made available under the 
link:https://opensource.org/license/mit/[MIT license].

== References

* Learn more about link:https://docs.cloudbees.com/docs/cloudbees-saas-platform-actions/latest/[using actions in CloudBees workflows].
* Learn about link:https://docs.cloudbees.com/docs/cloudbees-saas-platform/latest/[the CloudBees platform].
