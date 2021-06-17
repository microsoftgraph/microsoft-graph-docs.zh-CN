---
title: cloudPcUserSettingAssignment 资源类型
description: 表示定义的用户设置分配集合。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 704142ce266a826606b6c32b209d69d052d1a3c9
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993683"
---
# <a name="cloudpcusersettingassignment--resource-type"></a>cloudPcUserSettingAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示定义的用户设置分配集合。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户设置分配的唯一标识符。 只读。 如果 `target` 为用户组，则 ID 具有以下结构：{policyID}_{groupID}。|
|target|[cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)|用户设置的分配目标。 目前，用户设置支持的唯一目标为用户组。|
|createdDateTime|DateTimeOffset|创建此工作分配的日期和时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。  |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcUserSettingAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserSettingAssignment",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementAssignmentTarget"
  }
}
```
