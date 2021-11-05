---
title: caseExportOperation 资源类型
description: 表示电子数据展示导出的过程。
ms.localizationpriority: medium
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c3f69f459aec067608f350daddb5892b5e9ec06b
ms.sourcegitcommit: f9e71d3b8a54a98c282ef49783babe5698300c06
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2021
ms.locfileid: "60793901"
---
# <a name="caseexportoperation-resource-type"></a>caseExportOperation 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示电子数据展示导出的过程。 **caseExportOperation** 只能从审阅集导出 的响应 `Location` [中的 标头中检索](../api/ediscovery-reviewset-export.md)。

继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[getDownloadUrl](../api/ediscovery-caseexportoperation-getdownloadurl.md)|String| 返回导出的 URL。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|action|[microsoft.graph.ediscovery.caseAction](../resources/ediscovery-caseoperation.md#caseaction-values)| 此实体的 case 操作将始终为 `contentExport` 。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|azureBlobContainer|String| 将存储导出的 Azure 存储位置的名称。 这仅适用于存储在你自己的 Azure 存储位置的导出。 |
|azureBlobToken|字符串| Azure 存储位置的 SAS 令牌。  这仅适用于存储在你自己的 Azure 存储位置的导出。 |
|completedDateTime|DateTimeOffset| 导出完成的日期和时间。  继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|createdBy|[identitySet](../resources/identityset.md)| 启动导出操作的用户。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|createdDateTime|DateTimeOffset| 创建导出的日期和时间。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|说明|字符串| 为导出提供的说明。 |
|exportOptions|microsoft.graph.ediscovery.exportOptions| 为导出提供的选项。 有关详细信息，请参阅 [reviewSet： export](../api/ediscovery-reviewset-export.md)。 可取值为：`originalFiles`、`text`、`pdfReplacement`、`fileInfo`、`tags`。|
|exportStructure|microsoft.graph.ediscovery.exportFileStructure|提供的选项指定导出结构。 有关详细信息，请参阅 [reviewSet： export](../api/ediscovery-reviewset-export.md)。 可取值为：`none`、`directory`、`pst`。|
|id|String| 操作 ID。 只读。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|outputName|String| 为导出提供的名称。|
|percentProgress|Int32| 操作的进度。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|resultInfo|[resultInfo](../resources/resultinfo.md)|包含特定于成功和失败的结果信息。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|案例操作的状态。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。 可取值为：`notStarted`、`submissionFailed`、`running`、`succeeded`、`partiallySucceeded`、`failed`。|

### <a name="exportoptions-values"></a>exportOptions 值

|成员| 说明 |
|:---|:---|
|originalFiles| 包含原始文件的副本 - 仅在生成报告时排除此选项。 |
|text| 包括每个文档的原始提取的文本文件。 |
|pdfReplacement| 如果在审阅过程中生成修订的 PDF 文件，则这些文件可供导出。 你可以选择通过包括此选项来导出修订的 PDF，而不是原始的本机文件。 |
|fileInfo| 包括摘要和加载文件 - 这应始终包含在内。 |
|标记| 在加载文件中包括审阅期间应用的文档标记。 |

### <a name="exportfilestructure-values"></a>exportFileStructure 值

|成员| 说明 |
|:---|:---|
|directory| 地图电子数据展示工具常用的压缩目录结构。 所有文件都导出到名为 NativeFiles 的根文件。 |
|pst| 电子邮件存储在 PST 中，而来自网站的文档存储在代表原始本机文件夹结构的文件夹中。 |

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|reviewSet|[microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md)| 正在导出内容的审阅集。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.caseExportOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseExportOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "percentProgress": "Integer",
  "status": "String",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
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
