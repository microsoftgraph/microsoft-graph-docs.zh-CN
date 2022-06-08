---
title: ediscoveryFile 资源类型
description: 表示电子数据展示文件。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 6e952dcc8299b43817fca48beb4a705c522d12f4
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945174"
---
# <a name="ediscoveryfile-resource-type"></a>ediscoveryFile 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 ediscovery ReviewSet 文件的实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 ediscoveryFiles](../api/security-ediscoveryreviewset-list-files.md)|[microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md) 集合|获取 [ediscoveryFile](../resources/security-ediscoveryfile.md) 对象及其属性的列表。|
|[获取 ediscoveryFile](../api/security-ediscoveryfile-get.md)|[microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md)|读取 [ediscoveryFile](../resources/security-ediscoveryfile.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|content|流|原始文件的内容流。|
|dateTime|DateTimeOffset|上次修改文件的日期时间。 有关更多详细信息，请参阅 dateTime 值。|
|扩展|String|文件的文件扩展名，如 png、msg、docx 等。|
|extractedTextContent|Stream|从原始文件中提取的文本。 对于基于图像的文件，这将是 OCR 文本。|
|id|字符串|文件的唯一标识符。|
|mediaType|String|文件的 mimeType。 Eg：text/plain、charset=UTF-8、application/vnd.ms-outlook。|
|name|String|文件的名称。 电子邮件的主题。|
|otherProperties|字符串|文件的其他属性列表，例如 titleOfSharepointDocument、emailRecipients。 [了解详细信息](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)。|
|processingStatus|String|项目添加到审阅集后的处理状态。 可能的值为：`success`、、`internalError`、`processingTimeout``unknownError`、`invalidFileId`、`fileSizeIsZero`、`fileSizeIsTooLarge`、`fileDepthLimitExceeded`、`fileBodyIsTooLong`、`fileTypeIsUnknown``fileTypeIsNotSupported`、`malformedFile`、`protectedFile`、`poisonFile`、`noReviewSetSummaryGenerated`、`extractionException`、 `ocrProcessingTimeout``ocrFileSizeExceedsLimit`|
|senderAuthor|String collection|该文档的电子邮件或作者的发件人。|
|size|Int64|文件的大小。|
|sourceType|String|内容的原始源。 可能的值为： `mailbox`. `site`|
|subjectTitle|字符串|文档的电子邮件或标题的主题|

### <a name="datetime-values"></a>dateTime 值
|文件类型|定义|
|:---|:---|
电子邮件 |发送日期。
电子邮件附件 | 文档的上次修改日期;如果不可用，则为父级的“发送日期”。
嵌入的文档 | 文档的上次修改日期;如果不可用，则为父级的上次修改日期。
SPO 文档 (包含新式附件)  | SharePoint 上次修改日期;如果不可用，则文档上次修改日期。
非 Office 365 文档 | 上次修改日期。
会议 | 会议开始日期。
语音 信箱 | 发送日期。
IM |发送日期。
## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|托管|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|与文件关联的保管人。|
|标记|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 集合|与文件关联的标记。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryFile",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryFile",
  "id": "String (identifier)",
  "dateTime": "String (timestamp)",
  "size": "Integer",
  "name": "String",
  "sourceType": "String",
  "senderAuthor": [
    "String"
  ],
  "subjectTitle": "String",
  "extension": "String",
  "mediaType": "String",
  "content": "Stream",
  "extractedTextContent": "Stream",
  "processingStatus": "String",
  "otherProperties": {
    "@odata.type": "microsoft.graph.security.stringValueDictionary"
  }
}
```

