---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: UploadSession 资源提供了有关如何将大文件上传到 OneDrive、OneDrive for Business 或 SharePoint 文档库的信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3537a59da65499e67283d8a0640e5392c65edce1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446784"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="4daa2-103">UploadSession 资源</span><span class="sxs-lookup"><span data-stu-id="4daa2-103">UploadSession resource</span></span>

<span data-ttu-id="4daa2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4daa2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4daa2-105">**UploadSession** 资源提供了有关如何将大文件上传到 OneDrive、OneDrive for Business 或 SharePoint 文档库的信息。</span><span class="sxs-lookup"><span data-stu-id="4daa2-105">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4daa2-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4daa2-106">JSON representation</span></span>

<span data-ttu-id="4daa2-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4daa2-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="4daa2-108">属性</span><span class="sxs-lookup"><span data-stu-id="4daa2-108">Properties</span></span>


| <span data-ttu-id="4daa2-109">属性</span><span class="sxs-lookup"><span data-stu-id="4daa2-109">Property</span></span>       | <span data-ttu-id="4daa2-110">类型</span><span class="sxs-lookup"><span data-stu-id="4daa2-110">Type</span></span>              |<span data-ttu-id="4daa2-111">说明</span><span class="sxs-lookup"><span data-stu-id="4daa2-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="4daa2-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4daa2-112">expirationDateTime</span></span> | <span data-ttu-id="4daa2-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4daa2-113">DateTimeOffset</span></span>    | <span data-ttu-id="4daa2-p101">以 UTC 表示的上载会话过期的日期和时间。在此过期时间之前必须上载完整的文件文件。</span><span class="sxs-lookup"><span data-stu-id="4daa2-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="4daa2-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="4daa2-116">nextExpectedRanges</span></span> | <span data-ttu-id="4daa2-117">String collection</span><span class="sxs-lookup"><span data-stu-id="4daa2-117">String collection</span></span> | <span data-ttu-id="4daa2-p102">字节范围集合，文件服务器缺失。这些区域索引均从零开始，格式为“开始-结束”（例如，“0-26”指示该文件的前 27 个字节)。</span><span class="sxs-lookup"><span data-stu-id="4daa2-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="4daa2-120">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="4daa2-120">uploadUrl</span></span>          | <span data-ttu-id="4daa2-121">String</span><span class="sxs-lookup"><span data-stu-id="4daa2-121">String</span></span>            | <span data-ttu-id="4daa2-122">接受文件字节范围的 PUT 请求的 URL 端点。</span><span class="sxs-lookup"><span data-stu-id="4daa2-122">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="4daa2-123">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4daa2-123">See also</span></span>

- [<span data-ttu-id="4daa2-124">通过上传会话上传大文件</span><span class="sxs-lookup"><span data-stu-id="4daa2-124">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
