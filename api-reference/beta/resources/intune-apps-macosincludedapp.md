---
title: macOSIncludedApp 资源类型
description: 包含 MacOS 应用中包含的 .app 的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 87c7d8b5cc5eb1229b9860fe8192b0cd765c33c5
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/04/2022
ms.locfileid: "61712169"
---
# <a name="macosincludedapp-resource-type"></a>macOSIncludedApp 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 MacOS 应用中包含的 .app 的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|bundleId|String|CFBundleIdentifier。|
|bundleVersion|String|CFBundleVersion。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSIncludedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSIncludedApp",
  "bundleId": "String",
  "bundleVersion": "String"
}
```




