---
title: report 资源类型
description: 一个报表，随工作流，任一设备配置配置文件的历史记录或注册失败。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 5945343684aa20dc8af403eb094bb29648ff4f8f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970232"
---
# <a name="report-resource-type"></a>report 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。


一个报表，随工作流，任一设备配置配置文件的历史记录或注册失败。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|内容|Stream|尚未记录|

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
