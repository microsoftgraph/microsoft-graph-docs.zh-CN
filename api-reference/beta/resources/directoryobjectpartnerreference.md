---
title: directoryObjectPartnerReference 资源类型
description: 表示对合作伙伴租户中的目录对象的引用。 继承自 directoryObject。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 17bab72fad3e03b843975ae62261fac9c09af791
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918537"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="5e3ec-104">directoryObjectPartnerReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e3ec-104">directoryObjectPartnerReference resource type</span></span>

> <span data-ttu-id="5e3ec-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e3ec-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e3ec-107">表示对合作伙伴组织中的目录对象的引用。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-107">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="5e3ec-108">继承自 [directoryObject](directoryobject.md?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-108">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="5e3ec-109">属性</span><span class="sxs-lookup"><span data-stu-id="5e3ec-109">Properties</span></span>

| <span data-ttu-id="5e3ec-110">属性</span><span class="sxs-lookup"><span data-stu-id="5e3ec-110">Property</span></span> | <span data-ttu-id="5e3ec-111">类型</span><span class="sxs-lookup"><span data-stu-id="5e3ec-111">Type</span></span> | <span data-ttu-id="5e3ec-112">说明</span><span class="sxs-lookup"><span data-stu-id="5e3ec-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5e3ec-113">说明</span><span class="sxs-lookup"><span data-stu-id="5e3ec-113">description</span></span>|<span data-ttu-id="5e3ec-114">字符串</span><span class="sxs-lookup"><span data-stu-id="5e3ec-114">String</span></span>| <span data-ttu-id="5e3ec-115">返回的对象的说明。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-115">Description of the object returned.</span></span> <span data-ttu-id="5e3ec-116">只读。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-116">Read-only.</span></span> |
|<span data-ttu-id="5e3ec-117">displayName</span><span class="sxs-lookup"><span data-stu-id="5e3ec-117">displayName</span></span>|<span data-ttu-id="5e3ec-118">字符串</span><span class="sxs-lookup"><span data-stu-id="5e3ec-118">String</span></span>| <span data-ttu-id="5e3ec-119">目录对象返回，如组或应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-119">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="5e3ec-120">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-120">Read-only.</span></span> |
|<span data-ttu-id="5e3ec-121">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="5e3ec-121">externalPartnerTenantId</span></span>|<span data-ttu-id="5e3ec-122">Guid</span><span class="sxs-lookup"><span data-stu-id="5e3ec-122">Guid</span></span>| <span data-ttu-id="5e3ec-123">合作伙伴租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-123">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="5e3ec-124">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-124">Read-only.</span></span> |
|<span data-ttu-id="5e3ec-125">id</span><span class="sxs-lookup"><span data-stu-id="5e3ec-125">id</span></span>|<span data-ttu-id="5e3ec-126">字符串</span><span class="sxs-lookup"><span data-stu-id="5e3ec-126">String</span></span>| <span data-ttu-id="5e3ec-127">资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-127">The unique identifier for the resource.</span></span> <span data-ttu-id="5e3ec-128">继承自 [directoryObject](directoryobject.md?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-128">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="5e3ec-129">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-129">Read-only.</span></span> |
|<span data-ttu-id="5e3ec-130">objectType</span><span class="sxs-lookup"><span data-stu-id="5e3ec-130">objectType</span></span>|<span data-ttu-id="5e3ec-131">String</span><span class="sxs-lookup"><span data-stu-id="5e3ec-131">String</span></span>| <span data-ttu-id="5e3ec-132">合作伙伴租户中引用的对象的类型。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-132">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="5e3ec-133">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-133">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5e3ec-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e3ec-134">JSON representation</span></span>

<span data-ttu-id="5e3ec-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e3ec-135">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="5e3ec-136">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5e3ec-136">See also</span></span>

- [<span data-ttu-id="5e3ec-137">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="5e3ec-137">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
