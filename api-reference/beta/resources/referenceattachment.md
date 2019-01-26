---
title: referenceAttachment 资源类型
description: '指向文件夹或文件 （如文本文件或 Word 文档中） 上的 OneDrive for Business 云驱动器或其他受支持的存储位置，附加到的链接 '
localization_priority: Normal
ms.openlocfilehash: adf078f7ba678a4fe90a51972c5e4be4788c9c0c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574556"
---
# <a name="referenceattachment-resource-type"></a>referenceAttachment 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

链接到的文件夹或文件 （如文本文件或 Word 文档中） 上 OneDrive for Business 云驱动器或其他支持的存储位置，附加到[事件](../resources/event.md)、[消息](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[发布](../resources/post.md)。

派生自 [附件](attachment.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [referenceAttachment](referenceattachment.md) |读取 referenceAttachment 对象的属性和关系。|
|[删除](../api/attachment-delete.md) | 无 |删除 referenceAttachment 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contentType|String|附件的内容类型。 可选。|
|id|String|附件 ID。只读。|
|isFolder|布尔值|指定附件是否链接到的文件夹。 必须将其设置为 true 如果**sourceUrl**文件夹的链接。 可选。|
|isInline|布尔|如果附件显示为内嵌在嵌入对象的正文中，则设置为 true。 可选。|
|lastModifiedDateTime|DateTimeOffset|上次修改附件的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 可选。|
|name|String|表示嵌入的附件的图标下面显示的文本。 这不需要是实际的文件名称。 必需。|
|权限|referenceAttachmentPermission|指定**提供程序类型**中的提供程序的类型为附件授予的权限。 可取值为：`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView`、`organizationEdit`。 可选。|
|previewUrl|String|适用于仅图像-要获取的预览图像 URL 的参考附件。 仅当**sourceUrl**标识的图像文件，请使用**thumbnailUrl**和**previewUrl** 。 可选。|
|提供程序类型| referenceAttachmentProvider |支持此 contentType 的附件的提供程序的类型。 可取值为：`other`、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox`。 可选。|
|size|Int32|存储在引用附件的邮件的元数据以字节为单位的大小。 此值不表示实际文件的大小。 可选。|
|sourceUrl|String|若要获取附件内容的 URL。 如果这是指向文件夹的 URL，然后为文件夹以在 Outlook 或 Outlook web 上的中正确显示设置**isFolder**为 true。 必需。|
|thumbnailUrl|String|适用于仅图像-要获取的缩略图图像 URL 的参考附件。 仅当**sourceUrl**标识的图像文件，请使用**thumbnailUrl**和**previewUrl** 。 可选。|

## <a name="relationships"></a>关系
无



## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isFolder": true,
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "permission": "referenceAttachmentPermission",
  "previewUrl": "string",
  "providerType": "referenceAttachmentProvider",
  "size": 1024,
  "sourceUrl": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/referenceattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
