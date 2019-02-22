---
title: embeddedSIMActivationCode 资源类型
description: 移动运营商提供的嵌入的 SIM 激活代码。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 955dccb226332b297e30c4d40768f84936b04dbe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145225"
---
# <a name="embeddedsimactivationcode-resource-type"></a>embeddedSIMActivationCode 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

移动运营商提供的嵌入的 SIM 激活代码。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|integratedCircuitCardIdentifier|字符串|由移动运营商提供的此嵌入的 SIM 激活代码的集成电路卡标识符 (ICCID)。
输入必须与以下正则表达式匹配: "^\[0-9\]{19}\[0-9\]? $"。|
|matchingIdentifier|字符串|GSMA Association SGP RSP 技术规范部分中指定的 MatchingIdentifier (MatchingID) 4.1。
输入必须与以下正则表达式匹配: ' ^\[Z0-9\-\]* $ '。|
|smdpPlusServerAddress|字符串|在 GSM 关联 SPG .22 RSP 技术规范中指定的 SM + 服务器的完全限定域名。
输入必须与以下正则表达式匹配: "^ (\[Z0-9\]+ (\[-a-Z0-9\]+) *\.) +\[-za-Z\]{2,}$"。|

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




