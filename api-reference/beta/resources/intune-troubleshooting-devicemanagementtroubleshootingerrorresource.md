---
title: deviceManagementTroubleshootingErrorResource 资源类型
description: 表示疑难解答信息的链接的对象，该链接可能是 Azure 门户或 Microsoft 文档。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1da7b75414aafcce5e221cbb5f6e0cfc0ea0209b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266791"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>deviceManagementTroubleshootingErrorResource 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示疑难解答信息的链接的对象，该链接可能是 Azure 门户或 Microsoft 文档。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|text|String|尚未记录|
|链接|String|指向 Web 资源的链接。 可以包含以下任意格式化程序：{{UPN}}、{{DeviceGUID}}、{{UserGUID}}|

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




