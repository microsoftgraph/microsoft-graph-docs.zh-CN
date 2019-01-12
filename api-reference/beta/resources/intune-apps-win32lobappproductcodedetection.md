---
title: win32LobAppProductCodeDetection 资源类型
description: 包含产品代码和版本属性，以检测 Win32 应用程序
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5536384178ac197d3b52609cb767fef82befd3b2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928524"
---
# <a name="win32lobappproductcodedetection-resource-type"></a>win32LobAppProductCodeDetection 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含产品代码和版本属性，以检测 Win32 应用程序

继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|productCode|String|Win32 业务线 (LoB) 应用程序的产品代码。|
|productVersionOperator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|要检测产品版本的运算符。 可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual`。|
|productVersion|String|Win32 业务线 (LoB) 应用程序的产品版本。|

## <a name="relationships"></a>Relationships
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





