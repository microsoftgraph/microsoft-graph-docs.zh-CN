---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fcee21d1d6d9047b273b539ec10d3cfa63c2e3ce
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983223"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>configurationManagerClientEnabledFeatures 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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
|endpointProtection|Boolean|Endpoint Protection 是否由 Intune 管理|
|Officeoffice|Boolean|Office 应用程序是否由 Intune 管理|

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
  "windowsUpdateForBusiness": true,
  "endpointProtection": true,
  "officeApps": true
}
```





