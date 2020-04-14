---
title: macOSKernelExtension 资源类型
description: 表示特定的 macOS 内核扩展。 MacOS 内核扩展可以通过其团队标识符加上其捆绑包标识符进行描述。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 457d13b2f3f78b52457afd7c30bf3b0e36ca4e92
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447050"
---
# <a name="macoskernelextension-resource-type"></a>macOSKernelExtension 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示特定的 macOS 内核扩展。 MacOS 内核扩展可以通过其团队标识符加上其捆绑包标识符进行描述。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|teamIdentifier|String|用于对内核扩展进行签名的团队标识符。|
|bundleId|String|内核扩展的捆绑包 ID。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKernelExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKernelExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```



