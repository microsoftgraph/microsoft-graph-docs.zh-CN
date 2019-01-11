---
title: directoryObjectPartnerReference 资源类型
description: 表示对合作伙伴租户中的目录对象的引用。 继承自 directoryObject。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 46d0f749ac77e7d51e03314e78cfccf494dcc6fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884859"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="7d488-104">directoryObjectPartnerReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d488-104">directoryObjectPartnerReference resource type</span></span>

> <span data-ttu-id="7d488-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7d488-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d488-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7d488-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d488-107">表示对合作伙伴组织中的目录对象的引用。</span><span class="sxs-lookup"><span data-stu-id="7d488-107">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="7d488-108">继承自 [directoryObject](directoryobject.md?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="7d488-108">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="7d488-109">属性</span><span class="sxs-lookup"><span data-stu-id="7d488-109">Properties</span></span>

| <span data-ttu-id="7d488-110">属性</span><span class="sxs-lookup"><span data-stu-id="7d488-110">Property</span></span> | <span data-ttu-id="7d488-111">类型</span><span class="sxs-lookup"><span data-stu-id="7d488-111">Type</span></span> | <span data-ttu-id="7d488-112">说明</span><span class="sxs-lookup"><span data-stu-id="7d488-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7d488-113">说明</span><span class="sxs-lookup"><span data-stu-id="7d488-113">description</span></span>|<span data-ttu-id="7d488-114">字符串</span><span class="sxs-lookup"><span data-stu-id="7d488-114">String</span></span>| <span data-ttu-id="7d488-115">返回的对象的说明。</span><span class="sxs-lookup"><span data-stu-id="7d488-115">Description of the object returned.</span></span> <span data-ttu-id="7d488-116">只读。</span><span class="sxs-lookup"><span data-stu-id="7d488-116">Read-only.</span></span> |
|<span data-ttu-id="7d488-117">displayName</span><span class="sxs-lookup"><span data-stu-id="7d488-117">displayName</span></span>|<span data-ttu-id="7d488-118">字符串</span><span class="sxs-lookup"><span data-stu-id="7d488-118">String</span></span>| <span data-ttu-id="7d488-119">目录对象返回，如组或应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="7d488-119">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="7d488-120">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="7d488-120">Read-only.</span></span> |
|<span data-ttu-id="7d488-121">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="7d488-121">externalPartnerTenantId</span></span>|<span data-ttu-id="7d488-122">Guid</span><span class="sxs-lookup"><span data-stu-id="7d488-122">Guid</span></span>| <span data-ttu-id="7d488-123">合作伙伴租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="7d488-123">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="7d488-124">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="7d488-124">Read-only.</span></span> |
|<span data-ttu-id="7d488-125">id</span><span class="sxs-lookup"><span data-stu-id="7d488-125">id</span></span>|<span data-ttu-id="7d488-126">字符串</span><span class="sxs-lookup"><span data-stu-id="7d488-126">String</span></span>| <span data-ttu-id="7d488-127">资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7d488-127">The unique identifier for the resource.</span></span> <span data-ttu-id="7d488-128">继承自 [directoryObject](directoryobject.md?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="7d488-128">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="7d488-129">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="7d488-129">Read-only.</span></span> |
|<span data-ttu-id="7d488-130">objectType</span><span class="sxs-lookup"><span data-stu-id="7d488-130">objectType</span></span>|<span data-ttu-id="7d488-131">String</span><span class="sxs-lookup"><span data-stu-id="7d488-131">String</span></span>| <span data-ttu-id="7d488-132">合作伙伴租户中引用的对象的类型。</span><span class="sxs-lookup"><span data-stu-id="7d488-132">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="7d488-133">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="7d488-133">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7d488-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d488-134">JSON representation</span></span>

<span data-ttu-id="7d488-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d488-135">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7d488-136">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7d488-136">See also</span></span>

- [<span data-ttu-id="7d488-137">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="7d488-137">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
