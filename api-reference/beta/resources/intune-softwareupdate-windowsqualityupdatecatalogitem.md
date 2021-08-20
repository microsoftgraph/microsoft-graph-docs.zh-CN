---
title: windowsQualityUpdateCatalogItem 资源类型
description: Windows目录项实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e393f995f07c695ec6d01b36b46dc486fc062f1f2c7f0dd7a7636f5796c4a372
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224332"
---
# <a name="windowsqualityupdatecatalogitem-resource-type"></a>windowsQualityUpdateCatalogItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows目录项实体


继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsQualityUpdateCatalogItems](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-list.md)|[windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) 集合|列出 [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) 对象的属性和关系。|
|[获取 windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-get.md)|[windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|读取 [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) 对象的属性和关系。|
|[创建 windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-create.md)|[windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|创建新的 [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) 对象。|
|[删除 windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-delete.md)|无|删除 [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)。|
|[更新 windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-update.md)|[windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|更新 [windowsQualityUpdateCatalogItem 对象](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|目录项 ID。继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|displayName|字符串|目录显示名称的条目。 继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|releaseDateTime|DateTimeOffset|目录项的发布日期 继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|endOfSupportDate|DateTimeOffset|目录项的上次支持日期 继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|kbArticleId|字符串|知识库文章 ID|
|classification|[windowsQualityUpdateClassification](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|质量更新的分类。 可取值为：`all`、`security`、`nonSecurity`。|
|isExpeditable|布尔值|指示更新是否符合加速条件的标志|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsQualityUpdateCatalogItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "endOfSupportDate": "String (timestamp)",
  "kbArticleId": "String",
  "classification": "String",
  "isExpeditable": true
}
```




