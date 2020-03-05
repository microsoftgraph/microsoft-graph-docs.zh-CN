---
title: report 资源类型
description: 一种根据工作流（设备配置文件历史记录或注册失败）不同的报告。
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 68939fa29a259d3f5a463d731c79a4a8ebff44d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447813"
---
# <a name="report-resource-type"></a>report 资源类型

命名空间： microsoft. graph

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

一种根据工作流（设备配置文件历史记录或注册失败）不同的报告。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|content|流|尚未记录|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.report"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```

