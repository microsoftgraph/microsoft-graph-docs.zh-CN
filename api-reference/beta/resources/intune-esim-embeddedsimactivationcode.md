---
title: embeddedSIMActivationCode 资源类型
description: 移动运营商提供的嵌入式 SIM 卡激活代码。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 88e9123d03c86ef8dee3a5252828e884ad043314
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039870"
---
# <a name="embeddedsimactivationcode-resource-type"></a>embeddedSIMActivationCode 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

移动运营商提供的嵌入式 SIM 卡激活代码。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|integratedCircuitCardIdentifier|String|INTEGRATED Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.
输入必须与以下正则表达式匹配："^ \[ 0-9 \] {19} \[ 0-9 \] ？$"。|
|matchingIdentifier|String|MatchingIdentifier (MATCHINGID) GSMA Association SGP.22 RSP 技术规范 4.1 节中指定。
输入必须与以下正则表达式匹配："^ \[ a-zA-Z0-9 \- \] *$"。|
|smdpPlusServerAddress|String|GSM Association SPG .22 RSP 技术规范中指定的 SM-DP+ 服务器的完全限定域名。
输入必须匹配以下正则表达式："^ (\[ a-zA-Z0-9 \] + (- \[ a-zA-Z0-9 \] +) *) + \. \[ a-zA-Z \] {2,} $"。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCode",
  "integratedCircuitCardIdentifier": "String",
  "matchingIdentifier": "String",
  "smdpPlusServerAddress": "String"
}
```



