---
title: windows10AssociatedApps 资源类型
description: Windows 10 相关应用程序定义。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5dd5b664bde2970caa4b09c027592684b9ecd5e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425916"
---
# <a name="windows10associatedapps-resource-type"></a>windows10AssociatedApps 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 10 相关应用程序定义。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appType|[windows10AppType](../resources/intune-deviceconfig-windows10apptype.md)|应用程序类型。 可取值为：`desktop`、`universal`。|
|标识符|String|标识符。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```




