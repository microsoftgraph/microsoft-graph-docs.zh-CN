---
title: macOSKernelExtension 资源类型
description: 表示特定的 macOS 内核扩展。 macOS 内核扩展可通过其团队标识符及其捆绑包标识符进行描述。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8f430f83dbd166ee93f9e0ebfc4baa4ddb9f39db
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095568"
---
# <a name="macoskernelextension-resource-type"></a>macOSKernelExtension 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示特定的 macOS 内核扩展。 macOS 内核扩展可通过其团队标识符及其捆绑包标识符进行描述。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|teamIdentifier|String|用于对内核扩展进行签名的团队标识符。|
|bundleId|String|内核扩展的捆绑 ID。|

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



