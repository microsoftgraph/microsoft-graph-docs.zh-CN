---
title：“siteSource 资源类型”说明：“与保管人关联的站点的容器。
author： “SeunginLyu” ms.localizationpriority： medium ms.prod： “ediscovery” doc_type： resourcePageType
---

# <a name="sitesource-resource-type"></a>siteSource 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
与保管人关联的站点的容器。

[dataSource](../resources/security-datasource.md) 中的 IInherits。


## <a name="methods"></a>方法
无。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **siteSource** 的用户。|
|createdDateTime|DateTimeOffset|**网站源** 的创建日期和时间。|
|displayName|String|**siteSource** 的显示名称。 这将是 SharePoint 网站的名称。|
|id|字符串| **siteSource** 的 ID。 可以随时使用 [Get 网站检索站点](../api/site-get.md)源 - https://graph.microsoft.com/v1.0/sites/{siteId}|
|holdStatus|String|**siteSource** 的保留状态。可能的值为： `notApplied`， `applied`， `applying`， `removing``partial`|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|网站|[site](../resources/site.md)|与 **siteSource** 关联的 SharePoint 网站。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.siteSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.siteSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

