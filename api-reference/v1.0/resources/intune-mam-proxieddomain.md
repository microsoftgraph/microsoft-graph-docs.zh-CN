---
title: proxiedDomain 资源类型
description: 代理域
author: tfitzmac
ms.openlocfilehash: dc924d75bc2cf1310cb715033281f59b70abb32a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320291"
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



