# <a name="update-educationuser-properties"></a>更新 educationUser 属性

更新 **educationuser** 对象的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  不支持。  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | EduRoster.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| 授权  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName| 字符串| 显示用户名称|
|givenName| 字符串 | 名字 |
|middleName| 字符串 | 用户的中间名|
|姓氏| 字符串 | 用户的姓|
|邮件| 字符串| 电子邮件地址|
|mobilePhone| 字符串 | 用户的移动电话号码 |
|externalSource|字符串| 可取值为：`sis`、`manual`、`enum_sentinel`。|
|externalSource|字符串| 创建此用户的位置。  可取值为：`sis`、`manual`、`enum_sentinel`。|
|mailingAddress|[physicalAddress](../resources/physicaladdress.md)| 用户的邮件地址。|
|residenceAddress|[physicalAddress](../resources/physicaladdress.md)| 用户所在的地址。|
|primaryRole|字符串| 用户的默认角色。  用户的角色在各课程中可能有所不同。 可取值为：`student`、`teacher`、`enum_sentinel`。|
|学生|[educationStudent](../resources/educationstudent.md)| 如果主要角色为学生，此部分将包含特定于学生的数据。|
|教师|[educationTeacher](../resources/educationteacher.md)| 如果主要角色为教师，此部分将包含特定于教师的数据。|


## <a name="response"></a>响应
如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationUser](../resources/educationuser.md) 对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/users/{user-id}
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

{
  "id": "13020",
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
  "mail": "rogelioC@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
  },
  "externalSource": "sis",
  "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "primaryRole": "student",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->