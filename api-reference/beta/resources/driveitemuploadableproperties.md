---
title: driveItemUploadableProperties 资源类型
description: DriveItemUploadableProperties 资源表示在创建上载会话时要上载的项。
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a68180476910051dc3633ee5dce7363c77eb60ae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505558"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="2b64a-103">driveItemUploadableProperties 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b64a-103">driveItemUploadableProperties resource type</span></span>

<span data-ttu-id="2b64a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b64a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b64a-105">**DriveItemUploadableProperties**资源表示在[创建上载会话](../api/driveitem-createuploadsession.md)时要上载的项。</span><span class="sxs-lookup"><span data-stu-id="2b64a-105">The **driveItemUploadableProperties** resource represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2b64a-106">属性</span><span class="sxs-lookup"><span data-stu-id="2b64a-106">Properties</span></span>

| <span data-ttu-id="2b64a-107">属性</span><span class="sxs-lookup"><span data-stu-id="2b64a-107">Property</span></span>     | <span data-ttu-id="2b64a-108">类型</span><span class="sxs-lookup"><span data-stu-id="2b64a-108">Type</span></span>                              | <span data-ttu-id="2b64a-109">说明</span><span class="sxs-lookup"><span data-stu-id="2b64a-109">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="2b64a-110">说明</span><span class="sxs-lookup"><span data-stu-id="2b64a-110">description</span></span>   |<span data-ttu-id="2b64a-111">String</span><span class="sxs-lookup"><span data-stu-id="2b64a-111">String</span></span>                             | <span data-ttu-id="2b64a-112">提供项的用户可见的说明。</span><span class="sxs-lookup"><span data-stu-id="2b64a-112">Provides a user-visible description of the item.</span></span> <span data-ttu-id="2b64a-113">读写。</span><span class="sxs-lookup"><span data-stu-id="2b64a-113">Read-write.</span></span> <span data-ttu-id="2b64a-114">仅适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="2b64a-114">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="2b64a-115">fileSize</span><span class="sxs-lookup"><span data-stu-id="2b64a-115">fileSize</span></span>      |<span data-ttu-id="2b64a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2b64a-116">Int64</span></span>                              | <span data-ttu-id="2b64a-117">提供在上载前执行配额检查所需的文件大小。</span><span class="sxs-lookup"><span data-stu-id="2b64a-117">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="2b64a-118">仅适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="2b64a-118">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="2b64a-119">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="2b64a-119">fileSystemInfo</span></span>|[<span data-ttu-id="2b64a-120">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="2b64a-120">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="2b64a-p103">客户端上的文件系统信息。读写。</span><span class="sxs-lookup"><span data-stu-id="2b64a-p103">File system information on client. Read-write.</span></span>                                                      |
|<span data-ttu-id="2b64a-123">name</span><span class="sxs-lookup"><span data-stu-id="2b64a-123">name</span></span>          |<span data-ttu-id="2b64a-124">String</span><span class="sxs-lookup"><span data-stu-id="2b64a-124">String</span></span>                             | <span data-ttu-id="2b64a-p104">项目名称（文件名和扩展名）。读写。</span><span class="sxs-lookup"><span data-stu-id="2b64a-p104">The name of the item (filename and extension). Read-write.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="2b64a-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b64a-127">JSON representation</span></span>

<span data-ttu-id="2b64a-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b64a-128">The following is a JSON representation of the resource.</span></span>

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