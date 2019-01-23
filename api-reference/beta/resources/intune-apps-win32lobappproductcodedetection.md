---
title: win32LobAppProductCodeDetection 资源类型
description: 包含产品代码和版本属性，以检测 Win32 应用程序
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7f5af1cfc5fffe5241ef3b7883c3ebe6a2100278
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411202"
---
# <a name="win32lobappproductcodedetection-resource-type"></a>win32LobAppProductCodeDetection 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含产品代码和版本属性，以检测 Win32 应用程序


继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|productCode|String|Win32 业务线 (LoB) 应用程序的产品代码。|
|productVersionOperator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|要检测产品版本的运算符。 可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual`。|
|productVersion|String|Win32 业务线 (LoB) 应用程序的产品版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeDetection",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```




