# <a name="directoryobject-resource-type"></a>directoryObject 资源类型

表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 directoryObject](../api/directoryobject_get.md) | [directoryObject](directoryobject.md) |读取 directory 对象的属性。|
|[删除 directoryObject](../api/directoryobject_delete.md) | 无 |删除 directory 对象。 |
|[checkMemberGroups](../api/directoryobject_checkmembergroups.md)|String collection|检查组列表中的成员身份。检查是可传递的。|
|[getMemberGroups](../api/directoryobject_getmembergroups.md)|String collection|返回 user、group 或 directory 对象所属的所有组。检查是可传递的。|
|[getMemberObjects](../api/directoryobject_getmemberobjects.md)|String collection| 返回 user、group 或 directory 对象所属的所有组和目录角色。检查是可传递的。 |

## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|id|String|用作此对象的唯一标识符的 Guid；例如，12345678-9abc-def0-1234-56789abcde。键。不可为 null。只读。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
