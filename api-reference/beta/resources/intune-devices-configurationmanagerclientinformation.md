---
title: configurationManagerClientInformation 资源类型
description: 从 SCCM 同步的配置管理器客户端信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 59c76431ab5812bce62a417297339ee46c59691e80d2f84035cc801ed70f8af6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145374"
---
# <a name="configurationmanagerclientinformation-resource-type"></a>configurationManagerClientInformation 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

从 SCCM 同步的配置管理器客户端信息

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|clientIdentifier|字符串|SCCM 中的 Configuration Manager 客户端 ID|
|isBlocked|布尔值|Configuration Manager 客户端从 SCCM 阻止状态|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
  "clientIdentifier": "String",
  "isBlocked": true
}
```




