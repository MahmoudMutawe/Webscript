# Webscript
 A web-script that takes a node ref and a user with read permission to the user on the referenced content.
<action id="my-act" type="page-link" label="My Action">
   <param name="page">hdp/ws/my-action?nodeRef={node.nodeRef}</param>
   <permissions>
      <permission allow="true">Read</permission>
   </permissions>
   <evaluator>evaluator.doclib.action.isFolder</evaluator>
</action>


my-action.get.desc.xml


<webscript>
  <shortname>Action Page</shortname>
  <description>action description</description>
  <url>/my=action?nodeRef={noderef}</url>  
  <authentication>user</authentication>
</webscript>
