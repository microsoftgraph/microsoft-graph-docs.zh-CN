---
title: report 资源类型
description: 一种根据工作流 (设备配置文件历史记录或注册失败) 不同的报告。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: ad95fa9ef21a6fbf80ddd8265b5bac2e72c1825b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523775"
---
# <a name="report-resource-type"></a>report 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

一种根据工作流 (设备配置文件历史记录或注册失败) 不同的报告。

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
