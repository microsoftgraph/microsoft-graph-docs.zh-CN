---
title: win32LobAppMsiInformation 资源类型
description: 包含 Win32 应用的 MSI 应用属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6acf39b1a611d7b607eb95ddca119ec63470bd9c
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60450064"
---
# <a name="win32lobappmsiinformation-resource-type"></a>win32LobAppMsiInformation 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Win32 应用的 MSI 应用属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|productCode|String|MSI 产品代码。|
|productVersion|String|MSI 产品版本。|
|upgradeCode|String|MSI 升级代码。|
|requiresReboot|Boolean|MSI 应用是否需要计算机重新启动才能完成安装。|
|packageType|[win32LobAppMsiPackageType](../resources/intune-apps-win32lobappmsipackagetype.md)|MSI 程序包类型。 可取值为：`perMachine`、`perUser`、`dualPurpose`。|
|productName|String|MSI 产品名称。|
|发布者|String|MSI 发布者。|

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



