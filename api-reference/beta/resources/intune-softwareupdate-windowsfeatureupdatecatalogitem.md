---
title: windowsFeatureUpdateCatalogItem 资源类型
description: Windows目录项实体
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4e65e6271866e6e1a7b8b8b8b284462a56a11e64
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020250"
---
# <a name="windowsfeatureupdatecatalogitem-resource-type"></a>windowsFeatureUpdateCatalogItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows目录项实体


继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsFeatureUpdateCatalogItems](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-list.md)|[windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) 集合|列出 [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) 对象的属性和关系。|
|[获取 windowsFeatureUpdateCatalogItem](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-get.md)|[windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|读取 [windowsFeatureUpdateCatalogItem 对象的属性和](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) 关系。|
|[创建 windowsFeatureUpdateCatalogItem](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-create.md)|[windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|创建新的 [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) 对象。|
|[删除 windowsFeatureUpdateCatalogItem](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-delete.md)|无|删除 [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)。|
|[更新 windowsFeatureUpdateCatalogItem](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-update.md)|[windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|更新 [windowsFeatureUpdateCatalogItem 对象](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|目录项 ID。继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|displayName|String|目录显示名称列表。 继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|releaseDateTime|DateTimeOffset|目录项的发布日期 继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|endOfSupportDate|DateTimeOffset|目录项的上次支持日期 继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|version|String|功能更新版本|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsFeatureUpdateCatalogItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "endOfSupportDate": "String (timestamp)",
  "version": "String"
}
```



