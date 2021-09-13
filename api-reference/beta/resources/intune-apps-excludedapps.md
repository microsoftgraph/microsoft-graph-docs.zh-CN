---
title: excludedApps 资源类型
description: 包含已排除的 Office365 应用的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2025df58d8ff6387fb217ec2d19e7f6d34df2499
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064565"
---
# <a name="excludedapps-resource-type"></a>excludedApps 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含已排除的 Office365 应用的属性。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|access|Boolean|应排除 MS Office Access 的值。|
|必应|Boolean|如果设置为默认值Microsoft 搜索值应排除。|
|excel|Boolean|应排除 MS Office Excel的值。|
|groove|Boolean|如果 MS 为 Office OneDrive for Business - Groove应排除的值。|
|infoPath|Boolean|如果 MS Office InfoPath 的值应排除。|
|lync|Boolean|如果 MS Office Skype for Business - Lync 的值应排除。|
|oneDrive|Boolean|应排除 MS Office OneDrive的值。|
|oneNote|Boolean|应排除 MS Office OneNote的值。|
|outlook|Boolean|应排除 MS Office Outlook的值。|
|powerPoint|Boolean|应排除 MS Office PowerPoint的值。|
|发布者|Boolean|应排除 MS Office Publisher的值。|
|sharePointDesigner|Boolean|应排除 MS Office SharePointDesigner 的值。|
|teams|Boolean|应排除 MS Office Teams的值。|
|visio|Boolean|应排除 MS Office Visio的值。|
|word|Boolean|应排除 MS Office Word 的值。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludedApps",
  "access": true,
  "bing": true,
  "excel": true,
  "groove": true,
  "infoPath": true,
  "lync": true,
  "oneDrive": true,
  "oneNote": true,
  "outlook": true,
  "powerPoint": true,
  "publisher": true,
  "sharePointDesigner": true,
  "teams": true,
  "visio": true,
  "word": true
}
```



