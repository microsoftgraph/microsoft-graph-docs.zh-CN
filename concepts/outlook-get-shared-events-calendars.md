# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a>获取共享或委派日历中 Outlook 事件

在 Outlook 中，客户可以与其他用户共享日历，并让他们查看或修改该日历中的事件。 客户还可以授予委托代表他们行事，以接收或回复会议请求，或创建或更改日历中的项。

Microsoft Graph 以编程方式支持获取已由其他用户共享的日历中的事件，以及获取共享日历本身。 该支持还适用于已委派的日历。

例如，Garth 与 John 共享了他的默认日历，并授予 John 读取访问权限。 如果 John 已登录你的应用并提供了委派权限 (Calendars.Read.Shared or Calendars.ReadWrite.Shared)，则你的应用将能够访问 Garth 在该日历中的默认日历和事件，如下所述。

## <a name="get-an-event-in-the-shared-calendar"></a>获取共享日历中的事件

你可以获取 Garth 的共享的默认日历中的特定事件：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

成功完成后，你将收到“HTTP 200 正常”消息以及 Garth 默认日历中由`{id}`标识的[事件](../api-reference/v1.0/resources/event.md)实例。

## <a name="get-all-the-events-in-the-shared-calendar"></a>获取共享日历中的所有事件

获取 Garth 与 John 共享的默认日历中的所有事件：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

成功完成后，你将收到“HTTP 200 正常”消息以及 Garth 的默认日历中的[事件](../api-reference/v1.0/resources/event.md)实例的集合。

## <a name="get-the-shared-calendar"></a>获取共享的日历

获取 Garth 与 John 共享的默认日历。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

成功完成后，你将收到“HTTP 200 正常”消息以及表示 Garth 默认文件夹的[日历](../api-reference/v1.0/resources/calendar.md)实例。

如果 Garth 已经委派 John 进一步访问他的默认日历，或者如果 Garth 已将其整个邮箱委派给 John，那么可应用相同的 GET 功能。

如果 Garth 未与 John 共享他的默认日历，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。 


## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [为什么与 Outlook 日历集成](outlook-calendar-concept-overview.md)
- Microsoft Graph v1.0 中的 [日历 API](../api-reference/v1.0/resources/calendar.md)。