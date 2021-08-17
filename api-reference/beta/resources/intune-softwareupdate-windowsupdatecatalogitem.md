---
title: windowsUpdateCatalogItem 资源类型
description: Windows目录项实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a5c02bc7678b2487dda1ae61e07fc7d59de2cb829a026c0f8b3a385e3a68e383
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54165642"
---
# <a name="windowsupdatecatalogitem-resource-type"></a>windowsUpdateCatalogItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows目录项实体

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsUpdateCatalogItems](../api/intune-softwareupdate-windowsupdatecatalogitem-list.md)|[windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) 集合|列出 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) 对象的属性和关系。|
|[获取 windowsUpdateCatalogItem](../api/intune-softwareupdate-windowsupdatecatalogitem-get.md)|[windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|读取 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|目录项 ID。|
|displayName|字符串|目录显示名称的条目。|
|releaseDateTime|DateTimeOffset|目录项的发布日期|
|endOfSupportDate|DateTimeOffset|目录项的上次支持日期|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateCatalogItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateCatalogItem",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "endOfSupportDate": "String (timestamp)"
}
```




