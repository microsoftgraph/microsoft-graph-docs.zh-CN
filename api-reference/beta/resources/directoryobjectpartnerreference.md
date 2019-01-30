---
title: directoryObjectPartnerReference 资源类型
description: 表示对合作伙伴租户中的目录对象的引用。 继承自 directoryObject。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a031586d1f92bf2b8b331e9b71058211b4617382
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640306"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="4a423-104">directoryObjectPartnerReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a423-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a423-105">表示对合作伙伴组织中的目录对象的引用。</span><span class="sxs-lookup"><span data-stu-id="4a423-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="4a423-106">继承自 [directoryObject](directoryobject.md?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="4a423-106">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="4a423-107">属性</span><span class="sxs-lookup"><span data-stu-id="4a423-107">Properties</span></span>

| <span data-ttu-id="4a423-108">属性</span><span class="sxs-lookup"><span data-stu-id="4a423-108">Property</span></span> | <span data-ttu-id="4a423-109">类型</span><span class="sxs-lookup"><span data-stu-id="4a423-109">Type</span></span> | <span data-ttu-id="4a423-110">说明</span><span class="sxs-lookup"><span data-stu-id="4a423-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4a423-111">description</span><span class="sxs-lookup"><span data-stu-id="4a423-111">description</span></span>|<span data-ttu-id="4a423-112">String</span><span class="sxs-lookup"><span data-stu-id="4a423-112">String</span></span>| <span data-ttu-id="4a423-113">返回的对象的说明。</span><span class="sxs-lookup"><span data-stu-id="4a423-113">Description of the object returned.</span></span> <span data-ttu-id="4a423-114">只读。</span><span class="sxs-lookup"><span data-stu-id="4a423-114">Read-only.</span></span> |
|<span data-ttu-id="4a423-115">displayName</span><span class="sxs-lookup"><span data-stu-id="4a423-115">displayName</span></span>|<span data-ttu-id="4a423-116">String</span><span class="sxs-lookup"><span data-stu-id="4a423-116">String</span></span>| <span data-ttu-id="4a423-117">目录对象返回，如组或应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="4a423-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="4a423-118">只读。</span><span class="sxs-lookup"><span data-stu-id="4a423-118">Read-only.</span></span> |
|<span data-ttu-id="4a423-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="4a423-119">externalPartnerTenantId</span></span>|<span data-ttu-id="4a423-120">Guid</span><span class="sxs-lookup"><span data-stu-id="4a423-120">Guid</span></span>| <span data-ttu-id="4a423-121">合作伙伴租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="4a423-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="4a423-122">只读。</span><span class="sxs-lookup"><span data-stu-id="4a423-122">Read-only.</span></span> |
|<span data-ttu-id="4a423-123">id</span><span class="sxs-lookup"><span data-stu-id="4a423-123">id</span></span>|<span data-ttu-id="4a423-124">String</span><span class="sxs-lookup"><span data-stu-id="4a423-124">String</span></span>| <span data-ttu-id="4a423-125">资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4a423-125">The unique identifier for the resource.</span></span> <span data-ttu-id="4a423-126">继承自 [directoryObject](directoryobject.md?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="4a423-126">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="4a423-127">只读。</span><span class="sxs-lookup"><span data-stu-id="4a423-127">Read-only.</span></span> |
|<span data-ttu-id="4a423-128">objectType</span><span class="sxs-lookup"><span data-stu-id="4a423-128">objectType</span></span>|<span data-ttu-id="4a423-129">String</span><span class="sxs-lookup"><span data-stu-id="4a423-129">String</span></span>| <span data-ttu-id="4a423-130">合作伙伴租户中引用的对象的类型。</span><span class="sxs-lookup"><span data-stu-id="4a423-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="4a423-131">只读。</span><span class="sxs-lookup"><span data-stu-id="4a423-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4a423-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a423-132">JSON representation</span></span>

<span data-ttu-id="4a423-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a423-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference"
}-->

```json
{
  "description": "string ",
  "displayName": "string",
  "externalPartnerTenantId": "string (identifier)",
  "id": "string (identifier)",
  "objectType": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="4a423-134">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4a423-134">See also</span></span>

- [<span data-ttu-id="4a423-135">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="4a423-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobjectpartnerreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
