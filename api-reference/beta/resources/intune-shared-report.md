---
title: report 资源类型
description: 介绍了适用于 Intune 的 Microsoft Graph API 的报告资源，它支持多个工作流。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f017ce3ec744bb86ee3ea6e9820a0e29f8505514
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630219"
---
# <a name="report-resource-type"></a>report 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

返回适用于上下文的内容，包括：

- 设备配置文件历史记录报告。
- 注册失败报告。
- Microsoft 365 使用情况报告

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|content|流|报告内容;详细信息因报告类型而异。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.report"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```



