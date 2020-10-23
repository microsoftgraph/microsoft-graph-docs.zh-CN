---
author: JeremyKelley
description: 表示用于将大型文件上载到 OneDrive、OneDrive for Business 或 SharePoint 文档库，或作为 Outlook 事件和邮件对象的文件附件的迭代过程的信息。
title: uploadSession 资源类型
localization_priority: Normal
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 64c907559337a1e6c5f40e046726c747751aaf03
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723719"
---
# <a name="uploadsession-resource-type"></a><span data-ttu-id="71daf-103">uploadSession 资源类型</span><span class="sxs-lookup"><span data-stu-id="71daf-103">uploadSession resource type</span></span>

<span data-ttu-id="71daf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71daf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71daf-105">表示用于将大文件上载到的迭代过程的信息：</span><span class="sxs-lookup"><span data-stu-id="71daf-105">Represents information for an iterative process to upload large files to:</span></span>

- <span data-ttu-id="71daf-106">OneDrive</span><span class="sxs-lookup"><span data-stu-id="71daf-106">OneDrive</span></span>
- <span data-ttu-id="71daf-107">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="71daf-107">OneDrive for Business</span></span>
- <span data-ttu-id="71daf-108">SharePoint 文档库</span><span class="sxs-lookup"><span data-stu-id="71daf-108">SharePoint document libraries</span></span>
- <span data-ttu-id="71daf-109">Outlook [事件](event.md) 和 [邮件](message.md) 项目作为附件</span><span class="sxs-lookup"><span data-stu-id="71daf-109">Outlook [event](event.md) and [message](message.md) items as attachments</span></span>
- <span data-ttu-id="71daf-110">通用打印 [printDocument](printdocument.md) 项目</span><span class="sxs-lookup"><span data-stu-id="71daf-110">Universal Print [printDocument](printdocument.md) items</span></span>

## <a name="json-representation"></a><span data-ttu-id="71daf-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71daf-111">JSON representation</span></span>

<span data-ttu-id="71daf-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71daf-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession",
  "baseType": null
}-->

```json
{
  "uploadUrl": "String",
  "expirationDateTime": "String (timestamp)",
  "nextExpectedRanges": ["String"]
}
```

## <a name="properties"></a><span data-ttu-id="71daf-113">属性</span><span class="sxs-lookup"><span data-stu-id="71daf-113">Properties</span></span>


| <span data-ttu-id="71daf-114">属性</span><span class="sxs-lookup"><span data-stu-id="71daf-114">Property</span></span>       | <span data-ttu-id="71daf-115">类型</span><span class="sxs-lookup"><span data-stu-id="71daf-115">Type</span></span>              |<span data-ttu-id="71daf-116">说明</span><span class="sxs-lookup"><span data-stu-id="71daf-116">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="71daf-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="71daf-117">expirationDateTime</span></span> | <span data-ttu-id="71daf-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71daf-118">DateTimeOffset</span></span>    | <span data-ttu-id="71daf-p101">以 UTC 表示的上载会话过期的日期和时间。在此过期时间之前必须上载完整的文件文件。</span><span class="sxs-lookup"><span data-stu-id="71daf-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="71daf-121">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="71daf-121">nextExpectedRanges</span></span> | <span data-ttu-id="71daf-122">String collection</span><span class="sxs-lookup"><span data-stu-id="71daf-122">String collection</span></span> | <span data-ttu-id="71daf-123">将文件上载到文档库时，这是文件的服务器缺少的字节范围的集合。</span><span class="sxs-lookup"><span data-stu-id="71daf-123">When uploading files to document libraries, this is a collection of byte ranges that the server is missing for the file.</span></span> <span data-ttu-id="71daf-124">这些区域的索引为零，格式为 "{start}-{end}" (例如，"0-26" 表示文件) 的前27个字节。</span><span class="sxs-lookup"><span data-stu-id="71daf-124">These ranges are zero-indexed and of the format, "{start}-{end}" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span> <span data-ttu-id="71daf-125">将文件作为 Outlook 附件（而不是区域集合）上载时，此属性始终指示单个值 "{start}"，即文件中应开始下一次上载的位置。</span><span class="sxs-lookup"><span data-stu-id="71daf-125">When uploading files as Outlook attachments, instead of a collection of ranges, this property always indicates a single value "{start}", the location in the file where the next upload should begin.</span></span>
| <span data-ttu-id="71daf-126">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="71daf-126">uploadUrl</span></span>          | <span data-ttu-id="71daf-127">String</span><span class="sxs-lookup"><span data-stu-id="71daf-127">String</span></span>            | <span data-ttu-id="71daf-128">接受文件字节范围的 PUT 请求的 URL 端点。</span><span class="sxs-lookup"><span data-stu-id="71daf-128">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="71daf-129">另请参阅</span><span class="sxs-lookup"><span data-stu-id="71daf-129">See also</span></span>

- [<span data-ttu-id="71daf-130">将大型文件作为附件附加到 Outlook 邮件和事件 </span><span class="sxs-lookup"><span data-stu-id="71daf-130">Attach large files to Outlook messages and events as attachments </span></span>](/graph/outlook-large-attachments)
- [<span data-ttu-id="71daf-131">通过上传会话上传大文件</span><span class="sxs-lookup"><span data-stu-id="71daf-131">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession",
  "suppressions": []
}
-->


