---
author: JeremyKelley
description: <descrption>
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6b047c8eed22647083da07f2e7722269fb872783
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964219"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="aec69-102">UploadSession 资源</span><span class="sxs-lookup"><span data-stu-id="aec69-102">UploadSession resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aec69-103">**UploadSession** 资源提供了有关如何将大文件上传到 OneDrive、OneDrive for Business 或 SharePoint 文档库的信息。</span><span class="sxs-lookup"><span data-stu-id="aec69-103">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aec69-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aec69-104">JSON representation</span></span>

<span data-ttu-id="aec69-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aec69-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="aec69-106">属性</span><span class="sxs-lookup"><span data-stu-id="aec69-106">Properties</span></span>


| <span data-ttu-id="aec69-107">属性</span><span class="sxs-lookup"><span data-stu-id="aec69-107">Property</span></span>       | <span data-ttu-id="aec69-108">类型</span><span class="sxs-lookup"><span data-stu-id="aec69-108">Type</span></span>              |<span data-ttu-id="aec69-109">说明</span><span class="sxs-lookup"><span data-stu-id="aec69-109">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="aec69-110">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="aec69-110">expirationDateTime</span></span> | <span data-ttu-id="aec69-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aec69-111">DateTimeOffset</span></span>    | <span data-ttu-id="aec69-p101">以 UTC 表示的上载会话过期的日期和时间。在此过期时间之前必须上载完整的文件文件。</span><span class="sxs-lookup"><span data-stu-id="aec69-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="aec69-114">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="aec69-114">nextExpectedRanges</span></span> | <span data-ttu-id="aec69-115">String collection</span><span class="sxs-lookup"><span data-stu-id="aec69-115">String collection</span></span> | <span data-ttu-id="aec69-p102">字节范围集合，文件服务器缺失。这些区域索引均从零开始，格式为“开始-结束”（例如，“0-26”指示该文件的前 27 个字节)。</span><span class="sxs-lookup"><span data-stu-id="aec69-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="aec69-118">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="aec69-118">uploadUrl</span></span>          | <span data-ttu-id="aec69-119">String</span><span class="sxs-lookup"><span data-stu-id="aec69-119">String</span></span>            | <span data-ttu-id="aec69-120">接受文件字节范围的 PUT 请求的 URL 端点。</span><span class="sxs-lookup"><span data-stu-id="aec69-120">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="aec69-121">另请参阅</span><span class="sxs-lookup"><span data-stu-id="aec69-121">See also</span></span>

- [<span data-ttu-id="aec69-122">通过上传会话上传大文件</span><span class="sxs-lookup"><span data-stu-id="aec69-122">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

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
