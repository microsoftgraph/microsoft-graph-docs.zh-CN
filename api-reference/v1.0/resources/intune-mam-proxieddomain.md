---
title: proxiedDomain 资源类型
description: 代理域
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dc90ebd57752fedcaf7acf069da6e653da04978e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968545"
---
# <a name="proxieddomain-resource-type"></a>proxiedDomain 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

代理域
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ipAddressOrFQDN|String|IP 地址或 FQDN|
|代理|String|代理 IP|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```



