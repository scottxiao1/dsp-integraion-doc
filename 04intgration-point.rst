对接关键点
==========

.. warning:: 请确认该章节提及的事项已经满足，否则可能在正式的流量填充过程当中出现流量被屏蔽，填充不高等问题。


客户端UA和IP地址上报
--------------------

请确保 ``UA`` ``IP`` 在发送请求时包含在 ``Http Header`` 当中。

曝光和点击多地址上报问题
------------------------
 * 确保 Response 当中， ``click_tracking_url`` , ``imp_tracking_urls`` 数组当中的所有地址都已经被触发访问。
 * 在 ``click_tracking_url`` 和 ``imp_tracking_urls`` 当中的链接中，可能出现 ``,`` 的URL，请媒体确保该类型的URL不会被特殊处理，以免发生Tracking数据有误差。

.. warning:: ``click_tracking_url`` 和 ``imp_tracking_urls`` 当中的URL是否被有效，正确的触发将会和媒体的收益有关。

设备号数据
--------------------

* android请求中 请务必将  ``imei`` 传递

* ios请求中，请务必将设备的  ``idfa`` 传递
