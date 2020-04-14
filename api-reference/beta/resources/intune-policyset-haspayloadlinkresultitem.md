---
title: hasPayloadLinkResultItem 资源类型
description: 包含 HasPayloadLinks 操作结果的类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3194dc0e7c1f154dcb61ab4f4731111a87fefe9d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458408"
---
# <a name="haspayloadlinkresultitem-resource-type"></a>hasPayloadLinkResultItem 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 HasPayloadLinks 操作结果的类。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|payloadId|String|有效负载的键，格式为 Guid。|
|hasLink|Boolean|指示有效负载是否有任何链接。|
|error|String|异常信息指示是否成功检查此项。空字符串表示无错误。|
|源|[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)集合|链接来自的原因。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hasPayloadLinkResultItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hasPayloadLinkResultItem",
  "payloadId": "String",
  "hasLink": true,
  "error": "String",
  "sources": [
    "String"
  ]
}
```



