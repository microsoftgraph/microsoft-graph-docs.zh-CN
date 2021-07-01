---
title: driveItemUploadableProperties 资源类型
description: driveItemUploadableProperties 资源表示创建上载会话时要上载的项目。
localization_priority: Normal
author: JeremyKelley
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 6c00270f1e86e2bb8f44af36c6c514c9b80a647d
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236206"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="98455-103">driveItemUploadableProperties 资源类型</span><span class="sxs-lookup"><span data-stu-id="98455-103">driveItemUploadableProperties resource type</span></span>

<span data-ttu-id="98455-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98455-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98455-105">**driveItemUploadableProperties** 资源表示创建上传会话时 [上传的项](../api/driveitem-createuploadsession.md)。</span><span class="sxs-lookup"><span data-stu-id="98455-105">The **driveItemUploadableProperties** resource represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="properties"></a><span data-ttu-id="98455-106">属性</span><span class="sxs-lookup"><span data-stu-id="98455-106">Properties</span></span>

| <span data-ttu-id="98455-107">属性</span><span class="sxs-lookup"><span data-stu-id="98455-107">Property</span></span>     | <span data-ttu-id="98455-108">类型</span><span class="sxs-lookup"><span data-stu-id="98455-108">Type</span></span>                              | <span data-ttu-id="98455-109">说明</span><span class="sxs-lookup"><span data-stu-id="98455-109">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="98455-110">说明</span><span class="sxs-lookup"><span data-stu-id="98455-110">description</span></span>   |<span data-ttu-id="98455-111">String</span><span class="sxs-lookup"><span data-stu-id="98455-111">String</span></span>                             | <span data-ttu-id="98455-112">提供项的用户可见的说明。</span><span class="sxs-lookup"><span data-stu-id="98455-112">Provides a user-visible description of the item.</span></span> <span data-ttu-id="98455-113">读写。</span><span class="sxs-lookup"><span data-stu-id="98455-113">Read-write.</span></span> <span data-ttu-id="98455-114">仅在个人OneDrive上。</span><span class="sxs-lookup"><span data-stu-id="98455-114">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="98455-115">driveItemSource</span><span class="sxs-lookup"><span data-stu-id="98455-115">driveItemSource</span></span>| [<span data-ttu-id="98455-116">driveItemSource</span><span class="sxs-lookup"><span data-stu-id="98455-116">driveItemSource</span></span>](driveItemSource.md)              | <span data-ttu-id="98455-117">有关驱动器项源的信息。</span><span class="sxs-lookup"><span data-stu-id="98455-117">Information about the drive item source.</span></span> <span data-ttu-id="98455-118">读写。</span><span class="sxs-lookup"><span data-stu-id="98455-118">Read-write.</span></span> <span data-ttu-id="98455-119">仅在 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="98455-119">Only on OneDrive for Business and SharePoint.</span></span>  |
|<span data-ttu-id="98455-120">fileSize</span><span class="sxs-lookup"><span data-stu-id="98455-120">fileSize</span></span>      |<span data-ttu-id="98455-121">Int64</span><span class="sxs-lookup"><span data-stu-id="98455-121">Int64</span></span>                              | <span data-ttu-id="98455-122">提供在上载之前执行配额检查的预期文件大小。</span><span class="sxs-lookup"><span data-stu-id="98455-122">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="98455-123">仅在个人OneDrive上。</span><span class="sxs-lookup"><span data-stu-id="98455-123">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="98455-124">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="98455-124">fileSystemInfo</span></span>|[<span data-ttu-id="98455-125">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="98455-125">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="98455-p104">客户端上的文件系统信息。读写。</span><span class="sxs-lookup"><span data-stu-id="98455-p104">File system information on client. Read-write.</span></span>                                                      |
|<span data-ttu-id="98455-128">mediaSource</span><span class="sxs-lookup"><span data-stu-id="98455-128">mediaSource</span></span>  | [<span data-ttu-id="98455-129">mediaSource</span><span class="sxs-lookup"><span data-stu-id="98455-129">mediaSource</span></span>](mediaSource.md)                    | <span data-ttu-id="98455-130">媒体源信息。</span><span class="sxs-lookup"><span data-stu-id="98455-130">Media source information.</span></span> <span data-ttu-id="98455-131">读写。</span><span class="sxs-lookup"><span data-stu-id="98455-131">Read-write.</span></span> <span data-ttu-id="98455-132">仅在 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="98455-132">Only on OneDrive for Business and SharePoint.</span></span>                 |
|<span data-ttu-id="98455-133">name</span><span class="sxs-lookup"><span data-stu-id="98455-133">name</span></span>          |<span data-ttu-id="98455-134">String</span><span class="sxs-lookup"><span data-stu-id="98455-134">String</span></span>                             | <span data-ttu-id="98455-p106">项目名称（文件名和扩展名）。读写。</span><span class="sxs-lookup"><span data-stu-id="98455-p106">The name of the item (filename and extension). Read-write.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="98455-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98455-137">JSON representation</span></span>

<span data-ttu-id="98455-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98455-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.driveItemUploadableProperties",
  "baseType": null
}-->

```json
{
  "description": "String",
  "fileSize": 1024,
  "fileSystemInfo": {"@odata.type": "microsoft.graph.fileSystemInfo"},
  "name": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->

