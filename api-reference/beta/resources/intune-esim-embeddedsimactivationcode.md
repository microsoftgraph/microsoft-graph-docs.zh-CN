---
title: embeddedSIMActivationCode 资源类型
description: 为移动运营商提供嵌入的 SIM 激活代码。
author: tfitzmac
ms.openlocfilehash: 4e768a4047b8ddc785b545d3b850128a8e44f256
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311786"
---
# <a name="embeddedsimactivationcode-resource-type"></a>embeddedSIMActivationCode 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

为移动运营商提供嵌入的 SIM 激活代码。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|integratedCircuitCardIdentifier|字符串|由移动运营商提供，此集成电路卡标识符 (ICCID) 嵌入 SIM 激活代码。
输入项必须匹配以下正则表达式: ^\[0-9\]{19}\[0-9\]?$。|
|matchingIdentifier|字符串|GSMA 关联 SGP.22 RSP 技术规范 4.1 节中的规定 MatchingIdentifier (MatchingID)。
输入项必须匹配以下正则表达式: ^\[a-zA-Z0-9\-\]* $。|
|smdpPlusServerAddress|字符串|SM 的完全限定的域名-DP + GSM 关联 SPG.22 RSP 技术规范中指定的服务器。
输入项必须匹配以下正则表达式: ^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) *\.) +\[a-ZA-Z\]{2,}$。|

## <a name="relationships"></a>Relationships
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





