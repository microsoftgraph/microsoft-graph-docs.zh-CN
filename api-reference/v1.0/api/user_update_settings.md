# <a name="update-settings"></a>更新设置

更新[设置](../resources/user_settings.md)对象的属性。 在同一组织的用户可以根据他们输入首选项或组织策略的不同设置。 若要获取用户当前设置，请参阅[当前用户设置](user_get_settings.md)。 

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.ReadWrite User.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | User.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
```

请求用户 id 或者 userPrincipalName 才可以访问由用户或由具有 User.ReadWrite.All 权限的用户。 若要了解详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。 

```http
PATCH https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a>请求标头

| 标头       | 值|
|:-----------|:------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|布尔|设置为 true 禁用代理人访问的[趋势](../../beta/resources/insights_trending.md)API 或禁止用户访问 Office 深入中的文档。 设置为 true 还会影响的 Office 365 中显示的内容相关性-例如，建议 SharePoint 主页中的网站和中的 OneDrive for Business 的发现视图显示相关性较低的结果。 此设置反映在[Office 深入](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)的控件状态。|

## <a name="example"></a>示例 

##### <a name="request"></a>请求

下面是一个示例请求如何选择退出 Delve 用户并禁用其上为整个组织的内容相关性的贡献。

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a>响应

下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a>批量请求

还有可能退出 Delve 从多个用户并禁用上为整个组织通过批处理请求的内容相关性做出贡献。
若要了解详细信息，请参阅[JSON 批处理](https://developer.microsoft.com/graph/docs/concepts/json_batching)。

**重要说明**： 仅[Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US)角色组的成员可以更新多个用户。 



