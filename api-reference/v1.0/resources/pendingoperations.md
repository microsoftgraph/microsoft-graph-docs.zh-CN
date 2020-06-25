---
title: pendingOperations
description: PendingOperations 资源指示可能影响 driveItem 状态的一个或多个操作正在等待完成。
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 381ecd3bf302a1e7d323211cac071e360340b5c6
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863682"
---
# <a name="pendingoperations-resource-type"></a><span data-ttu-id="82c21-103">pendingOperations 资源类型</span><span class="sxs-lookup"><span data-stu-id="82c21-103">pendingOperations resource type</span></span>

<span data-ttu-id="82c21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82c21-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="82c21-105">指示可能影响**driveItem**状态的一个或多个操作正在等待完成。</span><span class="sxs-lookup"><span data-stu-id="82c21-105">Indicates that one or more operations that might affect the state of the **driveItem** are pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="82c21-106">属性</span><span class="sxs-lookup"><span data-stu-id="82c21-106">Properties</span></span>

| <span data-ttu-id="82c21-107">属性</span><span class="sxs-lookup"><span data-stu-id="82c21-107">Property</span></span>                | <span data-ttu-id="82c21-108">类型</span><span class="sxs-lookup"><span data-stu-id="82c21-108">Type</span></span>        | <span data-ttu-id="82c21-109">说明</span><span class="sxs-lookup"><span data-stu-id="82c21-109">Description</span></span> |
|:------------------------|:------------|:------------|
|<span data-ttu-id="82c21-110">**pendingContentUpdate**</span><span class="sxs-lookup"><span data-stu-id="82c21-110">**pendingContentUpdate**</span></span> |[<span data-ttu-id="82c21-111">pendingContentUpdate</span><span class="sxs-lookup"><span data-stu-id="82c21-111">pendingContentUpdate</span></span>](pendingcontentupdate.md)|<span data-ttu-id="82c21-112">一个属性，指示可能更新文件二进制内容的操作正在等待完成。</span><span class="sxs-lookup"><span data-stu-id="82c21-112">A property that indicates that an operation that might update the binary content of a file is pending completion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="82c21-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82c21-113">JSON representation</span></span>

<span data-ttu-id="82c21-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82c21-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingOperations",
  "baseType": null
}-->

```json
{
  "pendingContentUpdate": {"@odata.type": "microsoft.graph.pendingContentUpdate"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingOperations resource indicates that an operation that may affect the state of the DriveItem is pending completion.",
  "keywords": "pendingoperations,pendingoperations,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->
