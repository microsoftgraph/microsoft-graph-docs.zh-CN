---
title: deviceManagementTroubleshootingErrorResource 资源类型
description: 到 Azure 门户或 Microsoft doc 可能对象代表链接到故障排除信息的链接。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5653801fb3e4575e642c012721b667f51e791cc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429574"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>deviceManagementTroubleshootingErrorResource 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

到 Azure 门户或 Microsoft doc 可能对象代表链接到故障排除信息的链接。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|text|String|尚未记录|
|link|String|指向 web 资源的链接。 可以包含任何以下格式化程序: {{UPN}} {{DeviceGUID}} {{UserGUID}}|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorResource",
  "text": "String",
  "link": "String"
}
```




