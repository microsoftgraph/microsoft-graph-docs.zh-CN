---
title: ediscoveryReviewSet 资源类型
description: 表示收集用于诉讼、调查或监管请求的电子存储信息的静态集合。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 130f274e9bb9bff1eb2e573366bba3fbe8d4ed77
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838610"
---
# <a name="ediscoveryreviewset-resource-type"></a>ediscoveryReviewSet 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示收集用于诉讼、调查或监管请求的电子存储信息的静态集合。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 ediscoveryReviewSets](../api/security-ediscoverycase-list-reviewsets.md)|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) 集合|获取 [ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) 对象及其属性的列表。|
|[创建 ediscoveryReviewSet](../api/security-ediscoverycase-post-reviewsets.md)|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|创建新的 [ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) 对象。|
|[获取 ediscoveryReviewSet](../api/security-ediscoveryreviewset-get.md)|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|读取 [ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md) 对象的属性和关系。|
|[出口](../api/security-ediscoveryreviewset-export.md)|无|从 [审阅集](../resources/security-ediscoveryreviewset.md)启动数据导出。|
|[addToReviewSet](../api/security-ediscoveryreviewset-addtoreviewset.md)|无|开始将集合从 Microsoft 365 服务添加到 [审阅集](../resources/security-ediscoveryreviewset.md)的过程。|
|[列出文件](../api/security-ediscoveryreviewset-list-files.md)|[microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md) 集合|从文件导航属性获取 ediscoveryFile 资源。|
|[列出查询](../api/security-ediscoveryreviewset-list-queries.md)|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) 集合|获取与电子数据展示评审集关联的 [查询](../resources/security-ediscoveryreviewsetquery.md) 列表。|
|[创建 ediscoveryReviewSetQuery](../api/security-ediscoveryreviewset-post-queries.md)|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|创建新的 ediscoveryReviewSetQuery 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdBy|[microsoft.graph.identitySet](../resources/identityset.md)|创建审阅集的用户。 只读。 |
|createdDateTime|DateTimeOffset|创建审阅集时的日期时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|displayName|String|审阅集名称。 该名称是唯一的，最大限制为 64 个字符。|
|id|String|审阅集唯一标识符。 只读。|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|files|[microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md) 集合|表示审阅集中的文件。|
|查询|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) 集合|表示审阅集中的查询。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryReviewSet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryReviewSet",
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)"
}
```

