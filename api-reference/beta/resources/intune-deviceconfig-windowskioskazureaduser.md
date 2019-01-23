---
title: windowsKioskAzureADUser 资源类型
description: 用于标识网亭配置 AzureAD 用户帐户的类
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08c5b53e8e208abac2801146ff70df6023eaedff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420183"
---
# <a name="windowskioskazureaduser-resource-type"></a>windowsKioskAzureADUser 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于标识网亭配置 AzureAD 用户帐户的类


继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|userId|String|将锁定到此网亭配置 AzureAD 用户的 ID|
|userPrincipalName|String|将锁定到此网亭配置用户帐户|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```




