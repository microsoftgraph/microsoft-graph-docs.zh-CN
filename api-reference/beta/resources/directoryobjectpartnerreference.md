---
title: directoryObjectPartnerReference 资源类型
description: 表示对合作伙伴租户中的 directory 对象的引用。 继承自 directoryObject。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3158e081586cbcb822d385cbb357b017ac7239ba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507021"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="68f5d-104">directoryObjectPartnerReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="68f5d-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="68f5d-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="68f5d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68f5d-106">表示对合作伙伴组织中的目录对象的引用。</span><span class="sxs-lookup"><span data-stu-id="68f5d-106">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="68f5d-107">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="68f5d-107">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="68f5d-108">属性</span><span class="sxs-lookup"><span data-stu-id="68f5d-108">Properties</span></span>

| <span data-ttu-id="68f5d-109">属性</span><span class="sxs-lookup"><span data-stu-id="68f5d-109">Property</span></span> | <span data-ttu-id="68f5d-110">类型</span><span class="sxs-lookup"><span data-stu-id="68f5d-110">Type</span></span> | <span data-ttu-id="68f5d-111">说明</span><span class="sxs-lookup"><span data-stu-id="68f5d-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="68f5d-112">说明</span><span class="sxs-lookup"><span data-stu-id="68f5d-112">description</span></span>|<span data-ttu-id="68f5d-113">String</span><span class="sxs-lookup"><span data-stu-id="68f5d-113">String</span></span>| <span data-ttu-id="68f5d-114">返回的对象的说明。</span><span class="sxs-lookup"><span data-stu-id="68f5d-114">Description of the object returned.</span></span> <span data-ttu-id="68f5d-115">只读。</span><span class="sxs-lookup"><span data-stu-id="68f5d-115">Read-only.</span></span> |
|<span data-ttu-id="68f5d-116">displayName</span><span class="sxs-lookup"><span data-stu-id="68f5d-116">displayName</span></span>|<span data-ttu-id="68f5d-117">字符串</span><span class="sxs-lookup"><span data-stu-id="68f5d-117">String</span></span>| <span data-ttu-id="68f5d-118">返回的目录对象的名称，如 group 或 application。</span><span class="sxs-lookup"><span data-stu-id="68f5d-118">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="68f5d-119">只读。</span><span class="sxs-lookup"><span data-stu-id="68f5d-119">Read-only.</span></span> |
|<span data-ttu-id="68f5d-120">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="68f5d-120">externalPartnerTenantId</span></span>|<span data-ttu-id="68f5d-121">Guid</span><span class="sxs-lookup"><span data-stu-id="68f5d-121">Guid</span></span>| <span data-ttu-id="68f5d-122">合作伙伴租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="68f5d-122">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="68f5d-123">只读。</span><span class="sxs-lookup"><span data-stu-id="68f5d-123">Read-only.</span></span> |
|<span data-ttu-id="68f5d-124">id</span><span class="sxs-lookup"><span data-stu-id="68f5d-124">id</span></span>|<span data-ttu-id="68f5d-125">字符串</span><span class="sxs-lookup"><span data-stu-id="68f5d-125">String</span></span>| <span data-ttu-id="68f5d-126">资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="68f5d-126">The unique identifier for the resource.</span></span> <span data-ttu-id="68f5d-127">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="68f5d-127">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="68f5d-128">只读。</span><span class="sxs-lookup"><span data-stu-id="68f5d-128">Read-only.</span></span> |
|<span data-ttu-id="68f5d-129">objectType</span><span class="sxs-lookup"><span data-stu-id="68f5d-129">objectType</span></span>|<span data-ttu-id="68f5d-130">String</span><span class="sxs-lookup"><span data-stu-id="68f5d-130">String</span></span>| <span data-ttu-id="68f5d-131">合作伙伴租户中被引用对象的类型。</span><span class="sxs-lookup"><span data-stu-id="68f5d-131">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="68f5d-132">只读。</span><span class="sxs-lookup"><span data-stu-id="68f5d-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="68f5d-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68f5d-133">JSON representation</span></span>

<span data-ttu-id="68f5d-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68f5d-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="68f5d-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="68f5d-135">See also</span></span>

- [<span data-ttu-id="68f5d-136">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="68f5d-136">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

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
