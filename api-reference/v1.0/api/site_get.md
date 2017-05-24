# <a name="get-a-site-resource"></a>获取网站资源

检索[网站][]资源的属性和关系。**网站**资源表示 SharePoint 中的团队网站。

[网站]: ../resources/site.md

**网站**可按唯一标识符处理，此唯一标识符是下列值的复合 ID：

* 网站集主机名称 (contoso.sharepoint.com)
* 网站集的唯一 ID (guid)
* 网站的唯一 ID (guid)

还有一个保留的网站标识符 `root`，其经常为给定的目标引用根网站，如下所示：

* `/sites/root`：租户根网站。
* `/groups/{group-id}/sites/root`：该组的团队网站。

## <a name="prerequisites"></a>先决条件

要执行此请求，需要以下范围之一：

* Sites.Read.All
* Sites.ReadWrite.All

## <a name="get-the-tenants-root-site"></a>获取租户的根网站

若要访问租户内的根 SharePoint 网站：

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a>通过相对于服务器的 URL 访问网站

如果你的服务器具有**网站**资源的相对于服务器的 URL，你可以构建请求，如下所示：

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a>访问组团队网站

若要访问[组](../resources/group.md)的团队网站：

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}
```

### <a name="response"></a>响应

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "d297964f-d325-424b-a002-f54048a4622e",
    "name": "OneDrive / SharePoint Team",
    "description": "Collaboration site for the OneDrive and SharePoint team",
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/Get site by ID"
} -->
