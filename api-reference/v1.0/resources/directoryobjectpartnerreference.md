---
title: directoryObjectPartnerReference 资源类型
description: 表示对合作伙伴租户中的 directory 对象的引用。 继承自 directoryObject。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bcd26b80ba133ec2f4fa81c9ffb74fc7aac56b17
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34658020"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="517d2-104">directoryObjectPartnerReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="517d2-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="517d2-105">表示对合作伙伴组织中的目录对象的引用。</span><span class="sxs-lookup"><span data-stu-id="517d2-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="517d2-106">继承自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)。</span><span class="sxs-lookup"><span data-stu-id="517d2-106">Inherits from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span>

## <a name="properties"></a><span data-ttu-id="517d2-107">属性</span><span class="sxs-lookup"><span data-stu-id="517d2-107">Properties</span></span>

| <span data-ttu-id="517d2-108">属性</span><span class="sxs-lookup"><span data-stu-id="517d2-108">Property</span></span> | <span data-ttu-id="517d2-109">类型</span><span class="sxs-lookup"><span data-stu-id="517d2-109">Type</span></span> | <span data-ttu-id="517d2-110">说明</span><span class="sxs-lookup"><span data-stu-id="517d2-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="517d2-111">说明</span><span class="sxs-lookup"><span data-stu-id="517d2-111">description</span></span>|<span data-ttu-id="517d2-112">String</span><span class="sxs-lookup"><span data-stu-id="517d2-112">String</span></span>| <span data-ttu-id="517d2-113">返回的对象的说明。</span><span class="sxs-lookup"><span data-stu-id="517d2-113">Description of the object returned.</span></span> <span data-ttu-id="517d2-114">只读。</span><span class="sxs-lookup"><span data-stu-id="517d2-114">Read-only.</span></span> |
|<span data-ttu-id="517d2-115">displayName</span><span class="sxs-lookup"><span data-stu-id="517d2-115">displayName</span></span>|<span data-ttu-id="517d2-116">字符串</span><span class="sxs-lookup"><span data-stu-id="517d2-116">String</span></span>| <span data-ttu-id="517d2-117">返回的目录对象的名称, 如 group 或 application。</span><span class="sxs-lookup"><span data-stu-id="517d2-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="517d2-118">只读。</span><span class="sxs-lookup"><span data-stu-id="517d2-118">Read-only.</span></span> |
|<span data-ttu-id="517d2-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="517d2-119">externalPartnerTenantId</span></span>|<span data-ttu-id="517d2-120">Guid</span><span class="sxs-lookup"><span data-stu-id="517d2-120">Guid</span></span>| <span data-ttu-id="517d2-121">合作伙伴租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="517d2-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="517d2-122">只读。</span><span class="sxs-lookup"><span data-stu-id="517d2-122">Read-only.</span></span> |
|<span data-ttu-id="517d2-123">id</span><span class="sxs-lookup"><span data-stu-id="517d2-123">id</span></span>|<span data-ttu-id="517d2-124">字符串</span><span class="sxs-lookup"><span data-stu-id="517d2-124">String</span></span>| <span data-ttu-id="517d2-125">资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="517d2-125">The unique identifier for the resource.</span></span> <span data-ttu-id="517d2-126">继承自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)。</span><span class="sxs-lookup"><span data-stu-id="517d2-126">Inherited from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span> <span data-ttu-id="517d2-127">只读。</span><span class="sxs-lookup"><span data-stu-id="517d2-127">Read-only.</span></span> |
|<span data-ttu-id="517d2-128">objectType</span><span class="sxs-lookup"><span data-stu-id="517d2-128">objectType</span></span>|<span data-ttu-id="517d2-129">String</span><span class="sxs-lookup"><span data-stu-id="517d2-129">String</span></span>| <span data-ttu-id="517d2-130">合作伙伴租户中被引用对象的类型。</span><span class="sxs-lookup"><span data-stu-id="517d2-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="517d2-131">只读。</span><span class="sxs-lookup"><span data-stu-id="517d2-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="517d2-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="517d2-132">JSON representation</span></span>

<span data-ttu-id="517d2-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="517d2-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="517d2-134">另请参阅</span><span class="sxs-lookup"><span data-stu-id="517d2-134">See also</span></span>

- [<span data-ttu-id="517d2-135">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="517d2-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-v1.0)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
