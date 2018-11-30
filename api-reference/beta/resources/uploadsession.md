---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
ms.openlocfilehash: 27e3b448b54df0a5d35e2992391a554b73fd2c42
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049407"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="8af76-102">UploadSession 资源</span><span class="sxs-lookup"><span data-stu-id="8af76-102">UploadSession resource</span></span>

> <span data-ttu-id="8af76-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8af76-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8af76-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8af76-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8af76-105">**UploadSession** 资源提供了有关如何将大文件上传到 OneDrive、OneDrive for Business 或 SharePoint 文档库的信息。</span><span class="sxs-lookup"><span data-stu-id="8af76-105">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8af76-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8af76-106">JSON representation</span></span>

<span data-ttu-id="8af76-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8af76-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="8af76-108">属性</span><span class="sxs-lookup"><span data-stu-id="8af76-108">Properties</span></span>


| <span data-ttu-id="8af76-109">属性</span><span class="sxs-lookup"><span data-stu-id="8af76-109">Property</span></span>       | <span data-ttu-id="8af76-110">类型</span><span class="sxs-lookup"><span data-stu-id="8af76-110">Type</span></span>              |<span data-ttu-id="8af76-111">说明</span><span class="sxs-lookup"><span data-stu-id="8af76-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="8af76-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8af76-112">expirationDateTime</span></span> | <span data-ttu-id="8af76-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8af76-113">DateTimeOffset</span></span>    | <span data-ttu-id="8af76-p102">以 UTC 表示的上载会话过期的日期和时间。在此过期时间之前必须上载完整的文件文件。</span><span class="sxs-lookup"><span data-stu-id="8af76-p102">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="8af76-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="8af76-116">nextExpectedRanges</span></span> | <span data-ttu-id="8af76-117">String collection</span><span class="sxs-lookup"><span data-stu-id="8af76-117">String collection</span></span> | <span data-ttu-id="8af76-p103">字节范围集合，文件服务器缺失。这些区域索引均从零开始，格式为“开始-结束”（例如，“0-26”指示该文件的前 27 个字节)。</span><span class="sxs-lookup"><span data-stu-id="8af76-p103">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="8af76-120">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="8af76-120">uploadUrl</span></span>          | <span data-ttu-id="8af76-121">String</span><span class="sxs-lookup"><span data-stu-id="8af76-121">String</span></span>            | <span data-ttu-id="8af76-122">接受文件字节范围的 PUT 请求的 URL 端点。</span><span class="sxs-lookup"><span data-stu-id="8af76-122">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="8af76-123">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8af76-123">See also</span></span>

- [<span data-ttu-id="8af76-124">通过上传会话上传大文件</span><span class="sxs-lookup"><span data-stu-id="8af76-124">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
