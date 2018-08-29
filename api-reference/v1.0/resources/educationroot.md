# <a name="educationroot-resource-type"></a>educationRoot 资源类型

`/education` 命名空间公开特定于教育部门的功能。 `/education` 命名空间中的一些对象可在 Microsoft Graph 的其他部分中找到（例如，[users](user.md)）。 教育命名空间提供有关这些对象特定于教育的属性和功能。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Create educationClass](../api/educationroot_post_classes.md) |[educationClass](educationclass.md)| 通过发布到 classes 集合创建新的 **educationClass**。|
|[List classes](../api/educationroot_list_classes.md) |[educationClass](educationclass.md) 集合| 获取 **educationClass** 对象集合。|
|[Create educationSchool](../api/educationroot_post_schools.md) |[educationSchool](educationschool.md)| 通过发布到 schools 集合创建新的 **educationSchool**。|
|[List schools](../api/educationroot_list_schools.md) |[educationSchool](educationschool.md) 集合| 获取 **educationSchool** 对象集合。|
|[Create educationUser](../api/educationroot_post_users.md) |[educationUser](educationuser.md)| 通过发布到 users 集合创建新的 **educationUser**。|
|[List users](../api/educationroot_list_users.md) |[educationUser](educationuser.md) 集合| 获取 **educationUser** 对象集合。|

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|classes|[educationClass](educationclass.md) 集合| 只读。可为 NULL。|
|me|[educationUser](educationuser.md)| 只读。可为 NULL。|
|schools|[educationSchool](educationschool.md) 集合| 只读。可为 NULL。|
|users|[educationUser](educationuser.md) 集合| 只读。可为 NULL。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationRoot"
}-->

```json
{
}
```

<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->