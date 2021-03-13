---
title: directoryObjectPartnerReference 资源类型
description: 表示对合作伙伴租户中的目录对象的引用。 继承自 directoryObject。
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8b9d6a8826c38171dc7b32c281c371e841906f82
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761555"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="6244a-104">directoryObjectPartnerReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="6244a-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="6244a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6244a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6244a-106">表示对合作伙伴组织中目录对象的引用。</span><span class="sxs-lookup"><span data-stu-id="6244a-106">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="6244a-107">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="6244a-107">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6244a-108">属性</span><span class="sxs-lookup"><span data-stu-id="6244a-108">Properties</span></span>

| <span data-ttu-id="6244a-109">属性</span><span class="sxs-lookup"><span data-stu-id="6244a-109">Property</span></span> | <span data-ttu-id="6244a-110">类型</span><span class="sxs-lookup"><span data-stu-id="6244a-110">Type</span></span> | <span data-ttu-id="6244a-111">说明</span><span class="sxs-lookup"><span data-stu-id="6244a-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6244a-112">说明</span><span class="sxs-lookup"><span data-stu-id="6244a-112">description</span></span>|<span data-ttu-id="6244a-113">String</span><span class="sxs-lookup"><span data-stu-id="6244a-113">String</span></span>| <span data-ttu-id="6244a-114">返回的对象的说明。</span><span class="sxs-lookup"><span data-stu-id="6244a-114">Description of the object returned.</span></span> <span data-ttu-id="6244a-115">只读。</span><span class="sxs-lookup"><span data-stu-id="6244a-115">Read-only.</span></span> |
|<span data-ttu-id="6244a-116">displayName</span><span class="sxs-lookup"><span data-stu-id="6244a-116">displayName</span></span>|<span data-ttu-id="6244a-117">String</span><span class="sxs-lookup"><span data-stu-id="6244a-117">String</span></span>| <span data-ttu-id="6244a-118">要返回的目录对象的名称，如组或应用程序。</span><span class="sxs-lookup"><span data-stu-id="6244a-118">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="6244a-119">只读。</span><span class="sxs-lookup"><span data-stu-id="6244a-119">Read-only.</span></span> |
|<span data-ttu-id="6244a-120">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="6244a-120">externalPartnerTenantId</span></span>|<span data-ttu-id="6244a-121">Guid</span><span class="sxs-lookup"><span data-stu-id="6244a-121">Guid</span></span>| <span data-ttu-id="6244a-122">合作伙伴租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="6244a-122">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="6244a-123">只读。</span><span class="sxs-lookup"><span data-stu-id="6244a-123">Read-only.</span></span> |
|<span data-ttu-id="6244a-124">id</span><span class="sxs-lookup"><span data-stu-id="6244a-124">id</span></span>|<span data-ttu-id="6244a-125">String</span><span class="sxs-lookup"><span data-stu-id="6244a-125">String</span></span>| <span data-ttu-id="6244a-126">资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6244a-126">The unique identifier for the resource.</span></span> <span data-ttu-id="6244a-127">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="6244a-127">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="6244a-128">只读。</span><span class="sxs-lookup"><span data-stu-id="6244a-128">Read-only.</span></span> |
|<span data-ttu-id="6244a-129">objectType</span><span class="sxs-lookup"><span data-stu-id="6244a-129">objectType</span></span>|<span data-ttu-id="6244a-130">String</span><span class="sxs-lookup"><span data-stu-id="6244a-130">String</span></span>| <span data-ttu-id="6244a-131">合作伙伴租户中引用的对象的类型。</span><span class="sxs-lookup"><span data-stu-id="6244a-131">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="6244a-132">只读。</span><span class="sxs-lookup"><span data-stu-id="6244a-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6244a-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6244a-133">JSON representation</span></span>

<span data-ttu-id="6244a-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6244a-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="6244a-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6244a-135">See also</span></span>

- [<span data-ttu-id="6244a-136">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="6244a-136">Get directory objects from a list of ids</span></span>](../api/directoryobject-getbyids.md)

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
