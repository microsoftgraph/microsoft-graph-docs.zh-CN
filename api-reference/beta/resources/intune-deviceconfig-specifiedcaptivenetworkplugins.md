---
title: specifiedCaptiveNetworkPlugins 资源类型
description: 指定 IKEv2 AlwaysOn VPN 连接期间允许的所有强制网络插件
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5b162b0aa3da966cb7a55b23163d2a3bf51dc9e466b4a95fcdfe324b32a1bc94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54236939"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a>specifiedCaptiveNetworkPlugins 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定 IKEv2 AlwaysOn VPN 连接期间允许的所有强制网络插件

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedBundleIdentifiers|String collection|IKEv2 服务器的地址。 必须是 FQDN、UserFQDN、网络地址或 ASN1DN|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.specifiedCaptiveNetworkPlugins",
  "allowedBundleIdentifiers": [
    "String"
  ]
}
```




