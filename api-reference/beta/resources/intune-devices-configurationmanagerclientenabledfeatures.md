---
title: configurationManagerClientEnabledFeatures 资源类型
description: Configuration Manager 客户端已启用的功能
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2dfae041f1aab4c4ea74490d372350c5c0c2087b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528684"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>configurationManagerClientEnabledFeatures 资源类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Configuration Manager 客户端已启用的功能

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|inventory|布尔|目录是否由 Intune 管理|
|modernApps|布尔|现代应用程序是否由 Intune 管理|
|resourceAccess|布尔|资源访问权限是否由 Intune 管理|
|deviceConfiguration|布尔|设备配置是否由 Intune 管理|
|compliancePolicy|布尔|符合性策略是否由 Intune 管理|
|windowsUpdateForBusiness|Boolean|适用于企业的 Windows 更新是否由 Intune 管理|
|endpointProtection|布尔|Endpoint Protection 是否由 Intune 管理|
|Officeoffice|布尔|Office 应用程序是否由 Intune 管理|

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



