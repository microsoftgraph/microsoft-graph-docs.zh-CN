# <a name="shared-resource-type"></a>共享资源类型

**共享** 资源指示 DriveItem 已与他人共享。此资源包括有关如何共享项的信息。

如果 [**DriveItem**](driveitem.md) 具有非 NULL **共享** facet，则该项已共享。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shared",
  "optionalProperties": [ "sharedBy", "sharedDateTime" ]
}-->

```json
{
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "scope": "public | organization | users",
  "sharedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "sharedDateTime": "datetime"
}
```

## <a name="properties"></a>属性

| 属性       | 类型                          | 说明                                                                                        |
| :------------- | :---------------------------- | :------------------------------------------------------------------------------------------------- |
| 所有者          | [IdentitySet](identityset.md) | 共享项的所有者的身份。只读。                                           |
| scope          | String                        | 指示该项共享方式的范围：`anonymous`、`organization` 或 `users`。只读。 |
| sharedBy       | [identitySet](identityset.md) | 共享项目的用户的标识。只读。                                           |
| sharedDateTime | DateTimeOffset                | 共享项目的 UTC 日期和时间。只读。                                         |

## <a name="scope-values"></a>范围值

| 值        | 说明                                                                           |
|:-------------|:--------------------------------------------------------------------------------------|
| 公开       | 通过使用对具有此链接的用户均有效的链接共享项。               |
| 组织 | 通过使用对所有者组织内的所有用户均有效的链接共享项。 |
| 用户        | 仅与特定的用户共享项。                                          |

## <a name="remarks"></a>注解

有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shared resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
