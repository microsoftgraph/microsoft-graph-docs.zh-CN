---
title: report 资源类型
description: 一个报表，随工作流，任一设备配置配置文件的历史记录或注册失败。
ms.openlocfilehash: f79e1264ed82c05ea2fba4a61494589fb54dead5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010252"
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
