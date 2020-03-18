---
title: embeddedSIMActivationCode 资源类型
description: 移动运营商提供的嵌入的 SIM 激活代码。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 397f0eaaa15272601ddcf432e40086d9d0cd9270
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783317"
---
# <a name="embeddedsimactivationcode-resource-type"></a>embeddedSIMActivationCode 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

移动运营商提供的嵌入的 SIM 激活代码。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|integratedCircuitCardIdentifier|String|由移动运营商提供的此嵌入的 SIM 激活代码的集成电路卡标识符（ICCID）。
输入必须与以下正则表达式匹配： ' ^\[0-9\]{19}\[0-9\]？ $ '。|
|matchingIdentifier|String|GSMA Association SGP RSP 技术规范部分中指定的 MatchingIdentifier （MatchingID）4.1。
输入必须与以下正则表达式匹配： ' ^\[Z0-9\-\]* $ '。|
|smdpPlusServerAddress|String|在 GSM 关联 SPG .22 RSP 技术规范中指定的 SM + 服务器的完全限定域名。
输入必须与以下正则表达式匹配： "^ （\[Z0-9\]+ （\[-a-Z0-9\]+） *\.） +\[-za-Z\]{2,}$"。|

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



