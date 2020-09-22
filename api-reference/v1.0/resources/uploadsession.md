---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: UploadSession 资源提供了有关如何将大文件上载到 OneDrive、OneDrive for Business 或 SharePoint 文档库，或作为 Outlook 事件和邮件对象的文件附件的信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ff7ed4278da4d04d1af5158ce8fc01011bcc8598
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090611"
---
# <a name="uploadsession-resource-type"></a><span data-ttu-id="bce2b-103">uploadSession 资源类型</span><span class="sxs-lookup"><span data-stu-id="bce2b-103">uploadSession resource type</span></span>

<span data-ttu-id="bce2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bce2b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bce2b-105">**UploadSession**资源提供了有关如何将大文件上载到 OneDrive、Onedrive for Business 或 SharePoint 文档库，或将 Outlook[事件](event.md)和[邮件](message.md)项作为附件的信息。</span><span class="sxs-lookup"><span data-stu-id="bce2b-105">The **uploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries, or to Outlook [event](event.md) and [message](message.md) items as attachments.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bce2b-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bce2b-106">JSON representation</span></span>

<span data-ttu-id="bce2b-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bce2b-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession"
}-->

```json
{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="properties"></a><span data-ttu-id="bce2b-108">属性</span><span class="sxs-lookup"><span data-stu-id="bce2b-108">Properties</span></span>


| <span data-ttu-id="bce2b-109">属性</span><span class="sxs-lookup"><span data-stu-id="bce2b-109">Property</span></span>       | <span data-ttu-id="bce2b-110">类型</span><span class="sxs-lookup"><span data-stu-id="bce2b-110">Type</span></span>              |<span data-ttu-id="bce2b-111">说明</span><span class="sxs-lookup"><span data-stu-id="bce2b-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="bce2b-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bce2b-112">expirationDateTime</span></span> | <span data-ttu-id="bce2b-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bce2b-113">DateTimeOffset</span></span>    | <span data-ttu-id="bce2b-p101">以 UTC 表示的上载会话过期的日期和时间。在此过期时间之前必须上载完整的文件文件。</span><span class="sxs-lookup"><span data-stu-id="bce2b-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="bce2b-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="bce2b-116">nextExpectedRanges</span></span> | <span data-ttu-id="bce2b-117">String collection</span><span class="sxs-lookup"><span data-stu-id="bce2b-117">String collection</span></span> | <span data-ttu-id="bce2b-118">字节范围集合，文件服务器缺失。</span><span class="sxs-lookup"><span data-stu-id="bce2b-118">A collection of byte ranges that the server is missing for the file.</span></span> <span data-ttu-id="bce2b-119">这些区域索引均从零开始，格式为“开始-结束”（例如，“0-26”指示该文件的前 27 个字节)。</span><span class="sxs-lookup"><span data-stu-id="bce2b-119">These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span> <span data-ttu-id="bce2b-120">将文件作为 Outlook 附件（而不是区域集合）上载时，此属性始终指示单个值 "{start}"，即文件中应开始下一次上载的位置。</span><span class="sxs-lookup"><span data-stu-id="bce2b-120">When uploading files as Outlook attachments, instead of a collection of ranges, this property always indicates a single value "{start}", the location in the file where the next upload should begin.</span></span>
| <span data-ttu-id="bce2b-121">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="bce2b-121">uploadUrl</span></span>          | <span data-ttu-id="bce2b-122">String</span><span class="sxs-lookup"><span data-stu-id="bce2b-122">String</span></span>            | <span data-ttu-id="bce2b-123">接受文件字节范围的 PUT 请求的 URL 端点。</span><span class="sxs-lookup"><span data-stu-id="bce2b-123">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="bce2b-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bce2b-124">See also</span></span>

- [<span data-ttu-id="bce2b-125">将大型文件作为附件附加到 Outlook 邮件和事件 </span><span class="sxs-lookup"><span data-stu-id="bce2b-125">Attach large files to Outlook messages and events as attachments </span></span>](/graph/outlook-large-attachments)
- [<span data-ttu-id="bce2b-126">通过上传会话上传大文件</span><span class="sxs-lookup"><span data-stu-id="bce2b-126">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->

