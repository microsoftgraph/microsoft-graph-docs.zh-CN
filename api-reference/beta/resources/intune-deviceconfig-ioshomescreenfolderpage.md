---
title: iosHomeScreenFolderPage 资源类型
description: 包含主屏幕上的应用的文件夹
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fa9462f8fb0640584515d1c209abd03de0e6200
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424173"
---
# <a name="ioshomescreenfolderpage-resource-type"></a>iosHomeScreenFolderPage 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含主屏幕上的应用的文件夹

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|文件夹页的名称|
|应用|[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合|要在文件夹内的页面上显示的应用的集合。 该集合最多可包含 500 个元素。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```




