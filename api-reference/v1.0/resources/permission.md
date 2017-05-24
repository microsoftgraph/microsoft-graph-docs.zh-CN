# <a name="permission-resource-type"></a>权限资源类型

**权限** 资源提供有关授予 [DriveItem](driveitem.md) 资源的权限信息。

权限具有许多不同的形式。**权限**资源通过资源上的 facet 表示这些不同的形式。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "link", "grantedTo", "invitation", "inheritedFrom", "shareId" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.permission"
}-->
```json
{
  "id": "string (identifier)",
  "grantedTo": {"@odata.type": "microsoft.graph.identitySet"},
  "inheritedFrom": {"@odata.type": "microsoft.graph.itemReference"},
  "invitation": {"@odata.type": "microsoft.graph.sharingInvitation"},
  "link": {"@odata.type": "microsoft.graph.sharingLink"},
  "roles": ["string"],
  "shareId": "string"
}
```

## <a name="properties"></a>属性

| 属性      | 类型                                      | 说明
|:--------------|:------------------------------------------|:-----------------
| id            | String                                    | 在项目的所有权限中，某个权限的唯一标识符。只读。
| grantedTo     | [IdentitySet](identityset.md)             | 对于用户类型权限，此权限的用户和应用程序的详细信息。只读。
| 邀请    | [SharingInvitation][]                     | 此权限的全部关联共享邀请的详细信息。只读。
| inheritedFrom | [ItemReference](itemreference.md)         | 如果当前权限继承自上级，则提供对当前权限的上级的引用。只读。
| link          | [SharingLink][]                           | 如果当前权限是链接类型权限，则提供当前权限的链接详细信息。只读。
| role          | Collection of String                      | 权限类型，例如 `read`。有关角色的完整列表，请参阅如下内容。只读。
| shareId       | String                                    | 可通过 [**shares** API](../api/shares_get.md) 访问此共享项目的唯一令牌。只读。

权限资源使用 _facet_ 提供有关由该资源表示的权限类型的信息。

具有[**链接**] [SharingLink] facet 的权限表示在该项上创建的共享链接。共享链接包含一个唯一令牌，可以为具有上述链接的任何人提供对项目的访问权限。

具有[**邀请**] [SharingInvitation] facet 的权限表示通过邀请特定用户或组访问该文件添加的权限。

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

## <a name="roles-enumeration"></a>角色枚举

| 角色        | 详细信息                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | 提供读取项的元数据和内容的功能。            |
| `write`     | 提供读取并修改项的元数据和内容的功能。 |
| `sp.owner`  | 对于 SharePoint 和 OneDrive for Business，这表示所有者角色。       |
| `sp.member` | 对于 SharePoint 和 OneDrive for Business，这表示成员角色。      |

## <a name="methods"></a>方法

| 方法                                              | REST 路径
|:----------------------------------------------------|:-----------------------
| [列出权限](../api/item_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [获取权限](../api/permission_get.md)          | `GET /drive/items/{item-id}/permissions/{id}`
| [添加](../api/item_invite.md)                        | `POST /drive/items/{item-id}/invite`
| [更新](../api/permission_update.md)               | `PATCH /drive/items/{item-id}/permissions/{id}`
| [删除](../api/permission_delete.md)               | `DELETE /drive/items/{item-id}/permissions/{id}`


## <a name="remarks"></a>注解

OneDrive for Business 和 SharePoint 文档库不返回 **inheritedFrom** 属性。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
