============================
relay_nodelet
============================

Why needed?
===========

When you write launch file, you may often remap the topic name.
You may sometimes want to change name to remap, depending on the conditions.
``relay_nodelet`` enables you to do that.


APIs
====
.. code:: xml

  <node pkg="nodelet" type="nodelet" name="input_relay"
        machine="$(arg MACHINE)"
        args="load jsk_topic_tools/Relay $(arg MANAGER)">
    <remap from="~input" to="$(arg INPUT)" unless="$(arg RUN_SELF_FILTER)" />
    <remap from="~input" to="openni_cloud_self_filter/cloud_out" if="$(arg RUN_SELF_FILTER)" />
    <remap from="~output" to="~raw_output" if="$(arg JOINT_STATIC_FILTER)" />
  </node>
