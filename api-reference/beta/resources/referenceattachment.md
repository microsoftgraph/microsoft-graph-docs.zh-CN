---
title: referenceAttachment 资源类型
description: '指向文件夹或文件的链接， (OneDrive for Business 云驱动器) 或其他受支持的存储位置上的文本文件或 Word 文档文件 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 914d04a6482b96fda0ee55c92f25bf950e594173
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136764"
---
# <a name="referenceattachment-resource-type"></a>referenceAttachment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指向附加到事件、 (或帖子的文件夹或文件（如 OneDrive for Business 云驱动器) 或其他受支持的存储位置上的文本文件或 Word 文档）[的链接](../resources/post.md)。 [](../resources/event.md) [](../resources/message.md)

派生自 [附件](attachment.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取](../api/attachment-get.md) | [referenceAttachment](referenceattachment.md) |读取 referenceAttachment 对象的属性和关系。|
|[删除](../api/attachment-delete.md) | 无 |删除 referenceAttachment 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contentType|String|附件的内容类型。 可选。|
|id|字符串|附件 ID。只读。|
|isFolder|Boolean|指定附件是否是指向文件夹的链接。 如果 **sourceUrl** 是指向文件夹的链接，则必须将此选项设置为 true。 可选。|
|isInline|Boolean|如果附件显示为内嵌在嵌入对象的正文中，则设置为 true。 可选。|
|lastModifiedDateTime|DateTimeOffset|上次修改附件的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 可选。|
|name|字符串|显示在用于表示嵌入附件的图标下方的文本。 这不必是实际的文件名。 必填。|
|permission|referenceAttachmentPermission|指定通过 providerType 中的提供程序类型为附件 **授予的权限**。 可取值为：`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView` 或 `organizationEdit`。 可选。|
|previewUrl|字符串|仅适用于图像的引用附件 - 用于获取预览图像的 URL。 仅在 sourceUrl 标识图像文件时，才使用 **thumbnailUrl** 和 **previewUrl。**  可选。|
|providerType|referenceAttachmentProvider|支持此 contentType 的附件的提供程序类型。 可取值为：`other`、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox`。 可选。|
|大小|Int32|用于引用附件的邮件中存储的元数据的大小（以字节为单位）。 此值不表示实际文件的大小。 可选。|
|sourceUrl|字符串|用于获取附件内容的 URL。 如果这是文件夹的 URL，则对于要正确显示在 Outlook 或 Web 上的 Outlook 中的文件夹，将 **isFolder** 设置为 true。 必填。|
|thumbnailUrl|字符串|仅适用于图像的引用附件 - 用于获取缩略图的 URL。 仅在 sourceUrl 标识图像文件时，才使用 **thumbnailUrl** 和 **previewUrl。**  可选。|

## <a name="relationships"></a>关系
无



## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
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
  "permission": "string",
  "previewUrl": "string",
  "providerType": "string",
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
  "suppressions": []
}
-->


