---
title: mobileAppContent 资源类型
description: 包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c36a306e0b594ff84bffbc3e80fd393d20051371
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759007"
---
# <a name="mobileappcontent-resource-type"></a>mobileAppContent 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppContents](../api/intune-apps-mobileappcontent-list.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合|列出 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。|
|[获取 mobileAppContent](../api/intune-apps-mobileappcontent-get.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|读取 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。|
|[创建 mobileAppContent](../api/intune-apps-mobileappcontent-create.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|创建新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。|
|[删除 mobileAppContent](../api/intune-apps-mobileappcontent-delete.md)|无|删除 [mobileAppContent](../resources/intune-apps-mobileappcontent.md)。|
|[更新 mobileAppContent](../api/intune-apps-mobileappcontent-update.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|应用内容版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|files|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合|此应用内容版本的文件列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```




