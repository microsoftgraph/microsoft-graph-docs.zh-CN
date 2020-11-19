---
title: embeddedSIMActivationCode 资源类型
description: 移动运营商提供的嵌入的 SIM 激活代码。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ea17bc01e37b8e44f3fc904918f76859a9fcb40f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288465"
---
# <a name="embeddedsimactivationcode-resource-type"></a>embeddedSIMActivationCode 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

移动运营商提供的嵌入的 SIM 激活代码。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|integratedCircuitCardIdentifier|字符串|由移动运营商提供的嵌入的 SIM 激活代码 (ICCID) 的集成电路卡标识符。
输入必须与以下正则表达式匹配： ' ^ \[ 0-9 \] {19} \[ 0-9 \] ？ $ '。|
|matchingIdentifier|字符串|MatchingIdentifier (MatchingID) 在 GSMA Association SGP RSP 技术规范部分中指定4.1。
输入必须与以下正则表达式匹配： ' ^ \[ Z0-9 \- \] * $ '。|
|smdpPlusServerAddress|字符串|在 GSM 关联 SPG .22 RSP 技术规范中指定的 SM + 服务器的完全限定域名。
输入必须与以下正则表达式匹配： "^ (\[ Z0-9 \] + (- \[ Z0 \] +) * \.) + \[ a za-Z \] {2,} $"。|

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




