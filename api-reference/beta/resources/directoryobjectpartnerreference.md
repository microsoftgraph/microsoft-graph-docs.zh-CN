---
title: directoryObjectPartnerReference 资源类型
description: 表示对合作伙伴租户中的目录对象的引用。 继承自 directoryObject。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a031586d1f92bf2b8b331e9b71058211b4617382
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511049"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="f0fe7-104">directoryObjectPartnerReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0fe7-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0fe7-105">表示对合作伙伴组织中的目录对象的引用。</span><span class="sxs-lookup"><span data-stu-id="f0fe7-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="f0fe7-106">继承自 [directoryObject](directoryobject.md?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="f0fe7-106">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="f0fe7-107">属性</span><span class="sxs-lookup"><span data-stu-id="f0fe7-107">Properties</span></span>

| <span data-ttu-id="f0fe7-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0fe7-108">Property</span></span> | <span data-ttu-id="f0fe7-109">类型</span><span class="sxs-lookup"><span data-stu-id="f0fe7-109">Type</span></span> | <span data-ttu-id="f0fe7-110">说明</span><span class="sxs-lookup"><span data-stu-id="f0fe7-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f0fe7-111">说明</span><span class="sxs-lookup"><span data-stu-id="f0fe7-111">description</span></span>|<span data-ttu-id="f0fe7-112">String</span><span class="sxs-lookup"><span data-stu-id="f0fe7-112">String</span></span>| <span data-ttu-id="f0fe7-113">返回的对象的说明。</span><span class="sxs-lookup"><span data-stu-id="f0fe7-113">Description of the object returned.</span></span> <span data-ttu-id="f0fe7-114">只读。</span><span class="sxs-lookup"><span data-stu-id="f0fe7-114">Read-only.</span></span> |
|<span data-ttu-id="f0fe7-115">displayName</span><span class="sxs-lookup"><span data-stu-id="f0fe7-115">displayName</span></span>|<span data-ttu-id="f0fe7-116">String</span><span class="sxs-lookup"><span data-stu-id="f0fe7-116">String</span></span>| <span data-ttu-id="f0fe7-117">目录对象返回，如组或应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="f0fe7-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="f0fe7-118">只读。</span><span class="sxs-lookup"><span data-stu-id="f0fe7-118">Read-only.</span></span> |
|<span data-ttu-id="f0fe7-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="f0fe7-119">externalPartnerTenantId</span></span>|<span data-ttu-id="f0fe7-120">Guid</span><span class="sxs-lookup"><span data-stu-id="f0fe7-120">Guid</span></span>| <span data-ttu-id="f0fe7-121">合作伙伴租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="f0fe7-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="f0fe7-122">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="f0fe7-122">Read-only.</span></span> |
|<span data-ttu-id="f0fe7-123">id</span><span class="sxs-lookup"><span data-stu-id="f0fe7-123">id</span></span>|<span data-ttu-id="f0fe7-124">String</span><span class="sxs-lookup"><span data-stu-id="f0fe7-124">String</span></span>| <span data-ttu-id="f0fe7-125">资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f0fe7-125">The unique identifier for the resource.</span></span> <span data-ttu-id="f0fe7-126">继承自 [directoryObject](directoryobject.md?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="f0fe7-126">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="f0fe7-127">只读。</span><span class="sxs-lookup"><span data-stu-id="f0fe7-127">Read-only.</span></span> |
|<span data-ttu-id="f0fe7-128">objectType</span><span class="sxs-lookup"><span data-stu-id="f0fe7-128">objectType</span></span>|<span data-ttu-id="f0fe7-129">String</span><span class="sxs-lookup"><span data-stu-id="f0fe7-129">String</span></span>| <span data-ttu-id="f0fe7-130">合作伙伴租户中引用的对象的类型。</span><span class="sxs-lookup"><span data-stu-id="f0fe7-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="f0fe7-131">只读。</span><span class="sxs-lookup"><span data-stu-id="f0fe7-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f0fe7-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0fe7-132">JSON representation</span></span>

<span data-ttu-id="f0fe7-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0fe7-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="f0fe7-134">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f0fe7-134">See also</span></span>

- <span data-ttu-id="f0fe7-135">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="f0fe7-135">[Get directory objects from a list of ids](/graph/api/directoryobject-getbyids?view=graph-rest-beta)</span></span>

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
