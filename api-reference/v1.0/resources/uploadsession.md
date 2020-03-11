---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: UploadSession 资源提供了有关如何将大文件上载到 OneDrive、OneDrive for Business 或 SharePoint 文档库，或作为 Outlook 事件和邮件对象的文件附件的信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b2540c1abdd5e40ea960dc3672ab7cc788e08ddd
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590011"
---
# <a name="uploadsession-resource-type"></a><span data-ttu-id="a735e-103">uploadSession 资源类型</span><span class="sxs-lookup"><span data-stu-id="a735e-103">uploadSession resource type</span></span>

<span data-ttu-id="a735e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a735e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a735e-105">**UploadSession**资源提供了有关如何将大文件上载到 OneDrive、Onedrive for Business 或 SharePoint 文档库，或将 Outlook[事件](event.md)和[邮件](message.md)项作为附件的信息。</span><span class="sxs-lookup"><span data-stu-id="a735e-105">The **uploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries, or to Outlook [event](event.md) and [message](message.md) items as attachments.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a735e-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a735e-106">JSON representation</span></span>

<span data-ttu-id="a735e-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a735e-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="a735e-108">属性</span><span class="sxs-lookup"><span data-stu-id="a735e-108">Properties</span></span>


| <span data-ttu-id="a735e-109">属性</span><span class="sxs-lookup"><span data-stu-id="a735e-109">Property</span></span>       | <span data-ttu-id="a735e-110">类型</span><span class="sxs-lookup"><span data-stu-id="a735e-110">Type</span></span>              |<span data-ttu-id="a735e-111">Description</span><span class="sxs-lookup"><span data-stu-id="a735e-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="a735e-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a735e-112">expirationDateTime</span></span> | <span data-ttu-id="a735e-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a735e-113">DateTimeOffset</span></span>    | <span data-ttu-id="a735e-p101">以 UTC 表示的上载会话过期的日期和时间。在此过期时间之前必须上载完整的文件文件。</span><span class="sxs-lookup"><span data-stu-id="a735e-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="a735e-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="a735e-116">nextExpectedRanges</span></span> | <span data-ttu-id="a735e-117">String collection</span><span class="sxs-lookup"><span data-stu-id="a735e-117">String collection</span></span> | <span data-ttu-id="a735e-118">字节范围集合，文件服务器缺失。</span><span class="sxs-lookup"><span data-stu-id="a735e-118">A collection of byte ranges that the server is missing for the file.</span></span> <span data-ttu-id="a735e-119">这些区域索引均从零开始，格式为“开始-结束”（例如，“0-26”指示该文件的前 27 个字节)。</span><span class="sxs-lookup"><span data-stu-id="a735e-119">These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span> <span data-ttu-id="a735e-120">将文件作为 Outlook 附件（而不是区域集合）上载时，此属性始终指示单个值 "{start}"，即文件中应开始下一次上载的位置。</span><span class="sxs-lookup"><span data-stu-id="a735e-120">When uploading files as Outlook attachments, instead of a collection of ranges, this property always indicates a single value "{start}", the location in the file where the next upload should begin.</span></span>
| <span data-ttu-id="a735e-121">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="a735e-121">uploadUrl</span></span>          | <span data-ttu-id="a735e-122">String</span><span class="sxs-lookup"><span data-stu-id="a735e-122">String</span></span>            | <span data-ttu-id="a735e-123">接受文件字节范围的 PUT 请求的 URL 端点。</span><span class="sxs-lookup"><span data-stu-id="a735e-123">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="a735e-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a735e-124">See also</span></span>

- [<span data-ttu-id="a735e-125">将大型文件作为附件附加到 Outlook 邮件和事件</span><span class="sxs-lookup"><span data-stu-id="a735e-125">Attach large files to Outlook messages and events as attachments </span></span>](/graph/outlook-large-attachments)
- [<span data-ttu-id="a735e-126">通过上传会话上传大文件</span><span class="sxs-lookup"><span data-stu-id="a735e-126">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
