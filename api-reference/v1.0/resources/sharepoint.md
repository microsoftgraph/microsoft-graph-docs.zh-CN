# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a>使用 Microsoft Graph 中的 SharePoint 网站

Microsoft Graph 中的 SharePoint API 支持以下核心情形：

* 访问 SharePoint **网站**和**驱动器**（文档库）
* 支持对**网站**资源进行只读访问（无法创建新网站）
* 支持对 **driveItems** 进行读写访问
* 用 SharePoint ID、URL 或相对路径表示的地址资源

## <a name="sharepoint-api-root-resources"></a>SharePoint API 根资源

以下示例与 `https://graph.microsoft.com/v1.0` 有关。

| 路径                                   | 说明
|:---------------------------------------|:------------------------------------
| /sites/root                            | 组织的默认[网站][]。
| /sites/{site-id}                       | 通过其 ID 访问特定[网站][]。
| /sites/{site-id}/drive                 | 访问给定[网站][]的默认[驱动器](drive.md)（文档库）。
| /sites/{site-id}/drives                | 枚举[网站][]下的[驱动器](drive.md)（文档库）。
| /sites/{site-id}/sites                 | 枚举[网站][]下的子网站。
| /groups/{group-id}/sites/root          | 访问组的团队[网站][]。

还可以使用 SharePoint 主机名，后面加上冒号和网站的相对路径，来为网站寻址。可以选择将另一个冒号置于末尾，转回为资源模型寻址。

| 路径                                           | 说明
|:-----------------------------------------------|:-----------------------------------
| /sites/contoso.sharepoint.com:/teams/hr        | 与 https://contoso.sharepoint.com/teams/hr 关联的网站
| /sites/contoso.sharepoint.com:/teams/hr:/drive | 访问此网站的默认[驱动器](drive.md)。

## <a name="note-for-existing-sharepoint-developers"></a>现有 SharePoint 开发人员须知

Microsoft Graph SharePoint API 与 CSOM API 有几个主要区别。[网站][]资源映射到 `SPWeb`。网站集中的根[网站][] (`SPWeb`) 具有 [siteCollection](sitecollection.md) 方面，其中包含有关 `SPSite` 的信息。由于网站 ID 只在其网站集中是唯一的，因此按 ID 为网站寻址需要提供网站集标识符和网站标识符。

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id},{spweb-id}/
```
仅使用主机名构造的 URL 将指向默认网站集中的根网站 (`SPWeb`)。

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname}
```

仅使用主机名和 siteCollection (`SPSite`) ID 构造的 URL 将指向给定网站集中的根网站 (`SPWeb`)。

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id}
```

[网站]: site.md
[drive]: drive.md
[siteCollection]: siteCollection.md

<!-- {
  "type": "#page.annotation",
  "description": "Getting started programming with the SharePoint API",
  "keywords": "getting started sharepoint rest api programming C# ios android rest http",
  "section": "documentation",
  "tocPath": "Getting Started",
  "tocIndex": -100
} -->
