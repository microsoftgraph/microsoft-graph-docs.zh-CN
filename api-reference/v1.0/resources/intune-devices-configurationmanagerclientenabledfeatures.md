---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f30ff020fdb5bcf8c157b620f2d47823590d5fb6
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735703"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>configurationManagerClientEnabledFeatures 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Configuration Manager 客户端已启用的功能

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|inventory|Boolean|目录是否由 Intune 管理|
|modernApps|Boolean|现代应用程序是否由 Intune 管理|
|resourceAccess|Boolean|资源访问权限是否由 Intune 管理|
|deviceConfiguration|Boolean|设备配置是否由 Intune 管理|
|compliancePolicy|Boolean|符合性策略是否由 Intune 管理|
|windowsUpdateForBusiness|Boolean|适用于企业的 Windows 更新是否由 Intune 管理|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```





