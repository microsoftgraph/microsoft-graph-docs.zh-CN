---
title: deviceManagementTroubleshootingErrorDetails 资源类型
description: 对象包含有关错误和其修复的详细的信息。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9cdda64170afc739c23f1b258e5f2f1b31158662
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429362"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a>deviceManagementTroubleshootingErrorDetails 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对象包含有关错误和其修复的详细的信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|context|String|尚未记录|
|failure|String|尚未记录|
|failureDetails|String|发生了什么错误详细的描述。|
|修正|String|如何解决此问题的详细的说明。|
|resources|[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)集合|链接到有关该故障的帮助文档。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
      "text": "String",
      "link": "String"
    }
  ]
}
```




