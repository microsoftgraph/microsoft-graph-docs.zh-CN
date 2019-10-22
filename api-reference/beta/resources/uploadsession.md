---
author: JeremyKelley
description: 表示用于将大型文件上载到 OneDrive、OneDrive for Business 或 SharePoint 文档库，或作为 Outlook 邮件对象的文件附件的迭代过程的信息。
title: uploadSession 资源类型
localization_priority: Normal
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 9bf40360d841c88413cb4f08b603432f86e1d8aa
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621390"
---
# <a name="uploadsession-resource-type"></a><span data-ttu-id="23ebf-103">uploadSession 资源类型</span><span class="sxs-lookup"><span data-stu-id="23ebf-103">uploadSession resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23ebf-104">表示用于将大型文件上载到 OneDrive、OneDrive for Business 或 SharePoint 文档库的迭代过程的信息，或作为附件的 Outlook[邮件](message.md)对象。</span><span class="sxs-lookup"><span data-stu-id="23ebf-104">Represents information for an iterative process to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries, or to Outlook [message](message.md) objects as attachments.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23ebf-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23ebf-105">JSON representation</span></span>

<span data-ttu-id="23ebf-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23ebf-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="23ebf-107">属性</span><span class="sxs-lookup"><span data-stu-id="23ebf-107">Properties</span></span>


| <span data-ttu-id="23ebf-108">属性</span><span class="sxs-lookup"><span data-stu-id="23ebf-108">Property</span></span>       | <span data-ttu-id="23ebf-109">类型</span><span class="sxs-lookup"><span data-stu-id="23ebf-109">Type</span></span>              |<span data-ttu-id="23ebf-110">说明</span><span class="sxs-lookup"><span data-stu-id="23ebf-110">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="23ebf-111">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="23ebf-111">expirationDateTime</span></span> | <span data-ttu-id="23ebf-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23ebf-112">DateTimeOffset</span></span>    | <span data-ttu-id="23ebf-p101">以 UTC 表示的上载会话过期的日期和时间。在此过期时间之前必须上载完整的文件文件。</span><span class="sxs-lookup"><span data-stu-id="23ebf-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="23ebf-115">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="23ebf-115">nextExpectedRanges</span></span> | <span data-ttu-id="23ebf-116">String collection</span><span class="sxs-lookup"><span data-stu-id="23ebf-116">String collection</span></span> | <span data-ttu-id="23ebf-117">将文件上载到文档库时，这是文件的服务器缺少的字节范围的集合。</span><span class="sxs-lookup"><span data-stu-id="23ebf-117">When uploading files to document libraries, this is a collection of byte ranges that the server is missing for the file.</span></span> <span data-ttu-id="23ebf-118">这些区域的索引为零，格式为 "{start}-{end}" （例如，"0-26" 表示文件的前27个字节）。</span><span class="sxs-lookup"><span data-stu-id="23ebf-118">These ranges are zero-indexed and of the format, "{start}-{end}" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span> <span data-ttu-id="23ebf-119">将文件作为 Outlook 邮件附件（而不是区域集合）上载时，此属性始终指示单个值 "{start}"，即文件中应开始下一次上载的位置。</span><span class="sxs-lookup"><span data-stu-id="23ebf-119">When uploading files as Outlook message attachments, instead of a collection of ranges, this property always indicates a single value "{start}", the location in the file where the next upload should begin.</span></span>
| <span data-ttu-id="23ebf-120">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="23ebf-120">uploadUrl</span></span>          | <span data-ttu-id="23ebf-121">String</span><span class="sxs-lookup"><span data-stu-id="23ebf-121">String</span></span>            | <span data-ttu-id="23ebf-122">接受文件字节范围的 PUT 请求的 URL 端点。</span><span class="sxs-lookup"><span data-stu-id="23ebf-122">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="23ebf-123">另请参阅</span><span class="sxs-lookup"><span data-stu-id="23ebf-123">See also</span></span>

- [<span data-ttu-id="23ebf-124">将大型文件作为附件附加到 Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="23ebf-124">Attach large files to Outlook messages as attachments </span></span>](/graph/outlook-large-attachments)
- [<span data-ttu-id="23ebf-125">通过上传会话上传大文件</span><span class="sxs-lookup"><span data-stu-id="23ebf-125">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

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
