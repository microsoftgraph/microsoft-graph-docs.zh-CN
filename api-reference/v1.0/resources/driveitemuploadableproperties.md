---
title: driveItemUploadableProperties 资源类型
description: DriveItemUploadableProperties 资源表示在创建上载会话时要上载的项。
localization_priority: Normal
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 1f3ef83f36af70aa2efd3cce8d0215d705114e50
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863871"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="335da-103">driveItemUploadableProperties 资源类型</span><span class="sxs-lookup"><span data-stu-id="335da-103">driveItemUploadableProperties resource type</span></span>

<span data-ttu-id="335da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="335da-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="335da-105">表示在[创建上载会话](../api/driveitem-createuploadsession.md)时要上载的项。</span><span class="sxs-lookup"><span data-stu-id="335da-105">Represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="335da-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="335da-106">JSON representation</span></span>

<span data-ttu-id="335da-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="335da-107">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="335da-108">属性</span><span class="sxs-lookup"><span data-stu-id="335da-108">Properties</span></span>

| <span data-ttu-id="335da-109">属性</span><span class="sxs-lookup"><span data-stu-id="335da-109">Property</span></span>     | <span data-ttu-id="335da-110">类型</span><span class="sxs-lookup"><span data-stu-id="335da-110">Type</span></span>                              | <span data-ttu-id="335da-111">说明</span><span class="sxs-lookup"><span data-stu-id="335da-111">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="335da-112">**description**</span><span class="sxs-lookup"><span data-stu-id="335da-112">**description**</span></span>   |<span data-ttu-id="335da-113">String</span><span class="sxs-lookup"><span data-stu-id="335da-113">String</span></span>                             | <span data-ttu-id="335da-114">提供项的用户可见的说明。</span><span class="sxs-lookup"><span data-stu-id="335da-114">Provides a user-visible description of the item.</span></span> <span data-ttu-id="335da-115">读写。</span><span class="sxs-lookup"><span data-stu-id="335da-115">Read-write.</span></span> <span data-ttu-id="335da-116">仅适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="335da-116">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="335da-117">**fileSize**</span><span class="sxs-lookup"><span data-stu-id="335da-117">**fileSize**</span></span>      |<span data-ttu-id="335da-118">Int64</span><span class="sxs-lookup"><span data-stu-id="335da-118">Int64</span></span>                              | <span data-ttu-id="335da-119">提供在上载前执行配额检查所需的文件大小。</span><span class="sxs-lookup"><span data-stu-id="335da-119">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="335da-120">仅适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="335da-120">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="335da-121">**fileSystemInfo**</span><span class="sxs-lookup"><span data-stu-id="335da-121">**fileSystemInfo**</span></span>|[<span data-ttu-id="335da-122">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="335da-122">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="335da-123">File system information on client.</span><span class="sxs-lookup"><span data-stu-id="335da-123">File system information on client.</span></span> <span data-ttu-id="335da-124">Read-write.</span><span class="sxs-lookup"><span data-stu-id="335da-124">Read-write.</span></span>                                                      |
|<span data-ttu-id="335da-125">**name**</span><span class="sxs-lookup"><span data-stu-id="335da-125">**name**</span></span>          |<span data-ttu-id="335da-126">String</span><span class="sxs-lookup"><span data-stu-id="335da-126">String</span></span>                             | <span data-ttu-id="335da-127">The name of the item (filename and extension).</span><span class="sxs-lookup"><span data-stu-id="335da-127">The name of the item (filename and extension).</span></span> <span data-ttu-id="335da-128">Read-write.</span><span class="sxs-lookup"><span data-stu-id="335da-128">Read-write.</span></span>                                          |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->
