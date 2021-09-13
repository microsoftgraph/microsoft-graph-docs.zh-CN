---
title: iosHomeScreenFolderPage 资源类型
description: 主页上包含应用和 Web 剪辑的文件夹的页面。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb6b27fa9cf033914cc1471c75e78fd2cc244e87
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136451"
---
# <a name="ioshomescreenfolderpage-resource-type"></a>iosHomeScreenFolderPage 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

主页上包含应用和 Web 剪辑的文件夹的页面。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|文件夹页的名称|
|应用|[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合|要显示在文件夹内的页面上的应用和 Web 剪辑列表。 该集合最多可包含 500 个元素。|

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




