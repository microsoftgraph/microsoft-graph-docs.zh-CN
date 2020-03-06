---
title: iosHomeScreenFolder 资源类型
description: 包含主屏幕上的应用页面的文件夹
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f06d15dce4ce765111ba02a200b59576a614828e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530680"
---
# <a name="ioshomescreenfolder-resource-type"></a>iosHomeScreenFolder 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含主屏幕上的应用页面的文件夹


继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称|
|页面|[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) 集合|主屏幕布局图标页面，必须为应用程序类型。 该集合最多可包含 500 个元素。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
  "displayName": "String",
  "pages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
      "displayName": "String",
      "apps": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenApp",
          "displayName": "String",
          "bundleID": "String"
        }
      ]
    }
  ]
}
```




