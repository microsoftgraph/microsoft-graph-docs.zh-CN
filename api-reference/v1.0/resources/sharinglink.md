# <a name="sharinglink-resource-type"></a>SharingLink 资源类型

**SharingLink** 资源将与链接相关的数据项分组到一个单一结构。

如果 [**权限**](permission.md) 资源有一个非 NULL **sharingLink** facet，则该权限表示共享链接（而不是授予给用户或组的权限）。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "type": "view | edit",
  "scope": "anonymous | organization",
  "webUrl": "url"
}
```

## <a name="properties"></a>属性

| 属性    | 类型                    | 说明                                                                                                                                                                                             |
|:------------|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| application | [标识](identity.md) | 链接所关联的应用。                                                                                                                                                                    |
| type        | String                  | 创建的链接类型。                                                                                                                                                                           |
| scope       | String                  | 由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。 |
| webUrl      | String                  | 在 OneDrive 网站上的浏览器中打开项的 URL。                                                                                                                                       |

## <a name="type-enumeration"></a>类型枚举

此表定义了 **type** 属性的可能值：

| 值   | 角色    | 说明                                                                     |
|:--------|:--------|:--------------------------------------------------------------------------------|
| `view`  | `read`  | 可查看共享链接，允许只读访问。                            |
| `edit`  | `write` | 编辑共享链接，允许读写访问。                               |

## <a name="scope-enumeration"></a>范围枚举

| 值          | 说明                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | 任何人均可使用共享链接。                                                                            |
| `organization` | 同一组织（租户）中的任何人均可使用共享链接。不适用于 OneDrive 个人版。 |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharingLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
