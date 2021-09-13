---
title: report 资源类型
description: 介绍支持多个工作流的 Microsoft Graph API 的报告资源。
ms.localizationpriority: medium
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2af9d026444b42a588a236842b3ee48963193192
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59100943"
---
# <a name="report-resource-type"></a>report 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

返回适用于上下文的内容，包括：

- 设备配置配置文件历史记录报告。
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



