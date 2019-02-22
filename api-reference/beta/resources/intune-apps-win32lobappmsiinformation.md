---
title: win32LobAppMsiInformation 资源类型
description: 包含 Win32 应用程序的 MSI 应用程序属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f330111a3e924e54cf23c30cd98d20e85cb38022
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158644"
---
# <a name="win32lobappmsiinformation-resource-type"></a>win32LobAppMsiInformation 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Win32 应用程序的 MSI 应用程序属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|productCode|String|MSI 产品代码。|
|productVersion|String|MSI 产品版本。|
|upgradeCode|字符串|MSI 升级代码。|
|requiresReboot|布尔|MSI 应用是否需要计算机重新启动以完成安装。|
|packageType|[win32LobAppMsiPackageType](../resources/intune-apps-win32lobappmsipackagetype.md)|MSI 包类型。 可取值为：`perMachine`、`perUser`、`dualPurpose`。|
|productName|字符串|MSI 产品名称。|
|publisher|字符串|MSI 发布者。|

## <a name="relationships"></a>关系
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
  "packageType": "String",
  "productName": "String",
  "publisher": "String"
}
```




