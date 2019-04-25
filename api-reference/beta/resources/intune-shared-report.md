---
title: report 资源类型
description: 介绍了适用于 Intune 的 Microsoft Graph API 的报告资源, 它支持多个工作流。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: f523f6df0b8b90cb6649ac81f1e433d6df227aea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534813"
---
# <a name="report-resource-type"></a>report 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

返回适用于上下文的内容, 包括:

- 设备配置文件历史记录报告。
- 注册失败报告。

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



