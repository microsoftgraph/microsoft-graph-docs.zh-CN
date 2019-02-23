---
title: directoryObjectPartnerReference 资源类型
description: 表示对合作伙伴租户中的 directory 对象的引用。 继承自 directoryObject。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b84b7447d689759444e9cfd99982857eafa71eb
ms.sourcegitcommit: 7412dd2f2d5ed66afa2b0759c861ad23b4c6ecdf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/23/2019
ms.locfileid: "30224125"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="99c8e-104">directoryObjectPartnerReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="99c8e-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="99c8e-105">表示对合作伙伴组织中的目录对象的引用。</span><span class="sxs-lookup"><span data-stu-id="99c8e-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="99c8e-106">继承自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)。</span><span class="sxs-lookup"><span data-stu-id="99c8e-106">Inherits from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span>

## <a name="properties"></a><span data-ttu-id="99c8e-107">属性</span><span class="sxs-lookup"><span data-stu-id="99c8e-107">Properties</span></span>

| <span data-ttu-id="99c8e-108">属性</span><span class="sxs-lookup"><span data-stu-id="99c8e-108">Property</span></span> | <span data-ttu-id="99c8e-109">类型</span><span class="sxs-lookup"><span data-stu-id="99c8e-109">Type</span></span> | <span data-ttu-id="99c8e-110">说明</span><span class="sxs-lookup"><span data-stu-id="99c8e-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="99c8e-111">说明</span><span class="sxs-lookup"><span data-stu-id="99c8e-111">description</span></span>|<span data-ttu-id="99c8e-112">字符串</span><span class="sxs-lookup"><span data-stu-id="99c8e-112">String</span></span>| <span data-ttu-id="99c8e-113">返回的对象的说明。</span><span class="sxs-lookup"><span data-stu-id="99c8e-113">Description of the object returned.</span></span> <span data-ttu-id="99c8e-114">只读。</span><span class="sxs-lookup"><span data-stu-id="99c8e-114">Read-only.</span></span> |
|<span data-ttu-id="99c8e-115">displayName</span><span class="sxs-lookup"><span data-stu-id="99c8e-115">displayName</span></span>|<span data-ttu-id="99c8e-116">字符串</span><span class="sxs-lookup"><span data-stu-id="99c8e-116">String</span></span>| <span data-ttu-id="99c8e-117">返回的目录对象的名称, 如 group 或 application。</span><span class="sxs-lookup"><span data-stu-id="99c8e-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="99c8e-118">只读。</span><span class="sxs-lookup"><span data-stu-id="99c8e-118">Read-only.</span></span> |
|<span data-ttu-id="99c8e-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="99c8e-119">externalPartnerTenantId</span></span>|<span data-ttu-id="99c8e-120">Guid</span><span class="sxs-lookup"><span data-stu-id="99c8e-120">Guid</span></span>| <span data-ttu-id="99c8e-121">合作伙伴租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="99c8e-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="99c8e-122">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="99c8e-122">Read-only.</span></span> |
|<span data-ttu-id="99c8e-123">id</span><span class="sxs-lookup"><span data-stu-id="99c8e-123">id</span></span>|<span data-ttu-id="99c8e-124">String</span><span class="sxs-lookup"><span data-stu-id="99c8e-124">String</span></span>| <span data-ttu-id="99c8e-125">资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="99c8e-125">The unique identifier for the resource.</span></span> <span data-ttu-id="99c8e-126">继承自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)。</span><span class="sxs-lookup"><span data-stu-id="99c8e-126">Inherited from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span> <span data-ttu-id="99c8e-127">只读。</span><span class="sxs-lookup"><span data-stu-id="99c8e-127">Read-only.</span></span> |
|<span data-ttu-id="99c8e-128">objectType</span><span class="sxs-lookup"><span data-stu-id="99c8e-128">objectType</span></span>|<span data-ttu-id="99c8e-129">字符串</span><span class="sxs-lookup"><span data-stu-id="99c8e-129">String</span></span>| <span data-ttu-id="99c8e-130">合作伙伴租户中被引用对象的类型。</span><span class="sxs-lookup"><span data-stu-id="99c8e-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="99c8e-131">只读。</span><span class="sxs-lookup"><span data-stu-id="99c8e-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="99c8e-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99c8e-132">JSON representation</span></span>

<span data-ttu-id="99c8e-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99c8e-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="99c8e-134">另请参阅</span><span class="sxs-lookup"><span data-stu-id="99c8e-134">See also</span></span>

- [<span data-ttu-id="99c8e-135">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="99c8e-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-v1.0)

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
