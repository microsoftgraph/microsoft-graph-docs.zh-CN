---
title: driveItemUploadableProperties 资源类型
description: DriveItemUploadableProperties 资源表示在创建上载会话时要上载的项。
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f8511bba850c1d165fe9b7082b7df51900b17962
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333396"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="0b803-103">driveItemUploadableProperties 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b803-103">driveItemUploadableProperties resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b803-104">**DriveItemUploadableProperties**资源表示在[创建上载会话](../api/driveitem-createuploadsession.md)时要上载的项。</span><span class="sxs-lookup"><span data-stu-id="0b803-104">The **driveItemUploadableProperties** resource represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0b803-105">属性</span><span class="sxs-lookup"><span data-stu-id="0b803-105">Properties</span></span>

| <span data-ttu-id="0b803-106">属性</span><span class="sxs-lookup"><span data-stu-id="0b803-106">Property</span></span>     | <span data-ttu-id="0b803-107">类型</span><span class="sxs-lookup"><span data-stu-id="0b803-107">Type</span></span>                              | <span data-ttu-id="0b803-108">说明</span><span class="sxs-lookup"><span data-stu-id="0b803-108">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="0b803-109">说明</span><span class="sxs-lookup"><span data-stu-id="0b803-109">description</span></span>   |<span data-ttu-id="0b803-110">String</span><span class="sxs-lookup"><span data-stu-id="0b803-110">String</span></span>                             | <span data-ttu-id="0b803-111">提供项的用户可见的说明。</span><span class="sxs-lookup"><span data-stu-id="0b803-111">Provides a user-visible description of the item.</span></span> <span data-ttu-id="0b803-112">读写。</span><span class="sxs-lookup"><span data-stu-id="0b803-112">Read-write.</span></span> <span data-ttu-id="0b803-113">仅适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="0b803-113">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="0b803-114">fileSize</span><span class="sxs-lookup"><span data-stu-id="0b803-114">fileSize</span></span>      |<span data-ttu-id="0b803-115">Int64</span><span class="sxs-lookup"><span data-stu-id="0b803-115">Int64</span></span>                              | <span data-ttu-id="0b803-116">提供在上载前执行配额检查所需的文件大小。</span><span class="sxs-lookup"><span data-stu-id="0b803-116">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="0b803-117">仅适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="0b803-117">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="0b803-118">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="0b803-118">fileSystemInfo</span></span>|[<span data-ttu-id="0b803-119">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="0b803-119">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="0b803-p103">客户端上的文件系统信息。读写。</span><span class="sxs-lookup"><span data-stu-id="0b803-p103">File system information on client. Read-write.</span></span>                                                      |
|<span data-ttu-id="0b803-122">name</span><span class="sxs-lookup"><span data-stu-id="0b803-122">name</span></span>          |<span data-ttu-id="0b803-123">String</span><span class="sxs-lookup"><span data-stu-id="0b803-123">String</span></span>                             | <span data-ttu-id="0b803-p104">项目名称（文件名和扩展名）。读写。</span><span class="sxs-lookup"><span data-stu-id="0b803-p104">The name of the item (filename and extension). Read-write.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="0b803-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b803-126">JSON representation</span></span>

<span data-ttu-id="0b803-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b803-127">The following is a JSON representation of the resource.</span></span>

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