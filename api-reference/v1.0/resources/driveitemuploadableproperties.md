---
title: driveItemUploadableProperties 资源类型
description: DriveItemUploadableProperties 资源表示在创建上载会话时要上载的项。
localization_priority: Normal
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: c05c69f0cf72f74913882ddbf75355dc37592584
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032717"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="6f95e-103">driveItemUploadableProperties 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f95e-103">driveItemUploadableProperties resource type</span></span>

<span data-ttu-id="6f95e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f95e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f95e-105">表示在 [创建上载会话](../api/driveitem-createuploadsession.md)时要上载的项。</span><span class="sxs-lookup"><span data-stu-id="6f95e-105">Represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f95e-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f95e-106">JSON representation</span></span>

<span data-ttu-id="6f95e-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f95e-107">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6f95e-108">属性</span><span class="sxs-lookup"><span data-stu-id="6f95e-108">Properties</span></span>

| <span data-ttu-id="6f95e-109">属性</span><span class="sxs-lookup"><span data-stu-id="6f95e-109">Property</span></span>     | <span data-ttu-id="6f95e-110">类型</span><span class="sxs-lookup"><span data-stu-id="6f95e-110">Type</span></span>                              | <span data-ttu-id="6f95e-111">说明</span><span class="sxs-lookup"><span data-stu-id="6f95e-111">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="6f95e-112">**description**</span><span class="sxs-lookup"><span data-stu-id="6f95e-112">**description**</span></span>   |<span data-ttu-id="6f95e-113">String</span><span class="sxs-lookup"><span data-stu-id="6f95e-113">String</span></span>                             | <span data-ttu-id="6f95e-114">提供项的用户可见的说明。</span><span class="sxs-lookup"><span data-stu-id="6f95e-114">Provides a user-visible description of the item.</span></span> <span data-ttu-id="6f95e-115">读写。</span><span class="sxs-lookup"><span data-stu-id="6f95e-115">Read-write.</span></span> <span data-ttu-id="6f95e-116">仅适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="6f95e-116">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="6f95e-117">**fileSize**</span><span class="sxs-lookup"><span data-stu-id="6f95e-117">**fileSize**</span></span>      |<span data-ttu-id="6f95e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6f95e-118">Int64</span></span>                              | <span data-ttu-id="6f95e-119">提供在上载前执行配额检查所需的文件大小。</span><span class="sxs-lookup"><span data-stu-id="6f95e-119">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="6f95e-120">仅适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="6f95e-120">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="6f95e-121">**fileSystemInfo**</span><span class="sxs-lookup"><span data-stu-id="6f95e-121">**fileSystemInfo**</span></span>|[<span data-ttu-id="6f95e-122">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="6f95e-122">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="6f95e-p103">客户端上的文件系统信息。读写。</span><span class="sxs-lookup"><span data-stu-id="6f95e-p103">File system information on client. Read-write.</span></span>                                                      |
|<span data-ttu-id="6f95e-125">**name**</span><span class="sxs-lookup"><span data-stu-id="6f95e-125">**name**</span></span>          |<span data-ttu-id="6f95e-126">String</span><span class="sxs-lookup"><span data-stu-id="6f95e-126">String</span></span>                             | <span data-ttu-id="6f95e-p104">项目名称（文件名和扩展名）。读写。</span><span class="sxs-lookup"><span data-stu-id="6f95e-p104">The name of the item (filename and extension). Read-write.</span></span>                                          |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->

