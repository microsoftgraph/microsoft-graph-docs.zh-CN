---
title: win32LobAppMsiInformation 资源类型
description: Win32 应用程序包含 MSI 应用程序的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e43b3dc9e46ed193b7547a7ce85863253445d30c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846513"
---
# <a name="win32lobappmsiinformation-resource-type"></a>win32LobAppMsiInformation 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Win32 应用程序包含 MSI 应用程序的属性。
## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|productCode|String|MSI 产品代码。|
|productVersion|String|MSI 产品版本。|
|upgradeCode|字符串|MSI 升级代码。|
|requiresReboot|布尔|是否 MSI 应用程序要求计算机重新启动以完成安装。|
|： 键入包|[win32LobAppMsiPackageType](../resources/intune-apps-win32lobappmsipackagetype.md)|MSI 包类型。 可取值为：`perMachine`、`perUser`、`dualPurpose`。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppMsiInformation",
  "productCode": "String",
  "productVersion": "String",
  "upgradeCode": "String",
  "requiresReboot": true,
  "packageType": "String"
}
```





