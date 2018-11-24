# <a name="publish-apps-to-your-organizations-app-catalog"></a>将应用程序发布到组织的应用程序目录



将[应用程序](../resources/teamsapp.md)发布到 Microsoft 团队的应用程序目录。 具体而言，此 API 将应用程序发布到组织的目录 （租户应用程序目录）;创建的资源将具有`distributionMethod`  =  `organization`。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。

>**注意：** 只有全局管理员可以调用此 API。 

| 权限类型                        | 权限（从最低特权到最高特权）|
|:----------------------------------     |:-------------|
| 委派（工作或学校帐户）     | AppCatalog.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持|
| 应用程序                            | 不支持|

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a>请求标头

| 标头        | 值           |
|:--------------|:--------------  |
| Authorization | Bearer {token}。必需。  |
| Content-Type  | 应用程序/zip |

## <a name="request-body"></a>请求正文

团队 Zip 清单负载。 团队应用程序 zip 文件，[请参阅创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)。 无法创建应用程序的组织的组织中具有相同的清单另一个应用程序 ID。

## <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应代码和[teamsCatalogApp](../resources/teamsapp.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

有关如何创建的 Microsoft 团队应用程序 zip 文件的信息，请参阅[创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)。 

### <a name="response"></a>响应

```
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```
