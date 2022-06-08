---
title: ediscoveryExportOperation 资源类型
description: 表示电子数据展示导出的过程。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 499f019fa9933522b91d9d0f1aeff518e43ff13b
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945178"
---
# <a name="ediscoveryexportoperation-resource-type"></a>ediscoveryExportOperation 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示电子数据展示导出的过程。

继承自 [caseOperation](../resources/security-caseoperation.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[getDownloadUrl](../api/security-ediscoveryexportoperation-getdownloadurl.md)|String| 返回导出的 URL。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|[microsoft.graph.security.caseAction](../resources/security-caseoperation.md#caseaction-values)| 操作表示的操作类型。 可能的值为：，`addToReviewSet``applyTags`，，`contentExport``convertToPdf`，`estimateStatistics`，`purgeData`|
|azureBlobContainer|String| 将存储导出的 Azure 存储位置的名称。 这仅适用于存储在自己的 Azure 存储位置中的导出。 |
|azureBlobToken|String| Azure 存储位置的 SAS 令牌。  这仅适用于存储在自己的 Azure 存储位置中的导出。 |
|completedDateTime|DateTimeOffset| 导出完成的日期和时间。|
|createdBy|[identitySet](../resources/identityset.md)| 发起导出操作的用户。|
|createdDateTime|DateTimeOffset| 创建导出的日期和时间。|
|description|String| 为导出提供的说明。|
|exportOptions|microsoft.graph.ediscovery.exportOptions| 为导出提供的选项。 有关更多详细信息，请参阅 [reviewSet：导出](../api/security-ediscoveryreviewset-export.md)。 可取值为：`originalFiles`、`text`、`pdfReplacement`、`fileInfo`、`tags`。|
|exportStructure|microsoft.graph.ediscovery.exportFileStructure|指定导出结构的选项。 有关更多详细信息，请参阅 [reviewSet：导出](../api/security-ediscoveryreviewset-export.md)。 可取值为：`none`、`directory`、`pst`。|
|id|String| 操作的 ID。 只读。 |
|outputName|String| 为导出提供的名称。|
|percentProgress|Int32| 操作的进度。|
|resultInfo|[resultInfo](../resources/resultinfo.md)|包含成功和失败特定的结果信息。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|status|[microsoft.graph.security.caseOperationStatus](../resources/security-caseoperation.md#caseoperationstatus-values)| 事例操作的状态。 可取值为：`notStarted`、`submissionFailed`、`running`、`succeeded`、`partiallySucceeded`、`failed`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|reviewSet|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|    从其中导出文档的审阅集。|
|reviewSetQuery|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|用于筛选要导出的文档的审阅集查询。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryExportOperation",
  "baseType": "microsoft.graph.security.caseOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryExportOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "percentProgress": "Integer",
  "status": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  },
  "outputName": "String",
  "description": "String",
  "outputFolderId": "String",
  "azureBlobContainer": "String",
  "azureBlobToken": "String",
  "exportOptions": "String",
  "exportStructure": "String"
}
```

