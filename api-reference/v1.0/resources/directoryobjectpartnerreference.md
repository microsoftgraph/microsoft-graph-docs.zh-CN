---
title: directoryObjectPartnerReference 资源类型
description: 表示对合作伙伴租户中的 directory 对象的引用。 继承自 directoryObject。
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cda40de50710c971970d64853b33eebbde8865a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091766"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="20b03-104">directoryObjectPartnerReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="20b03-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="20b03-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20b03-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20b03-106">表示对合作伙伴组织中的目录对象的引用。</span><span class="sxs-lookup"><span data-stu-id="20b03-106">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="20b03-107">继承自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)。</span><span class="sxs-lookup"><span data-stu-id="20b03-107">Inherits from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span>

## <a name="properties"></a><span data-ttu-id="20b03-108">属性</span><span class="sxs-lookup"><span data-stu-id="20b03-108">Properties</span></span>

| <span data-ttu-id="20b03-109">属性</span><span class="sxs-lookup"><span data-stu-id="20b03-109">Property</span></span> | <span data-ttu-id="20b03-110">类型</span><span class="sxs-lookup"><span data-stu-id="20b03-110">Type</span></span> | <span data-ttu-id="20b03-111">说明</span><span class="sxs-lookup"><span data-stu-id="20b03-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="20b03-112">说明</span><span class="sxs-lookup"><span data-stu-id="20b03-112">description</span></span>|<span data-ttu-id="20b03-113">String</span><span class="sxs-lookup"><span data-stu-id="20b03-113">String</span></span>| <span data-ttu-id="20b03-114">返回的对象的说明。</span><span class="sxs-lookup"><span data-stu-id="20b03-114">Description of the object returned.</span></span> <span data-ttu-id="20b03-115">只读。</span><span class="sxs-lookup"><span data-stu-id="20b03-115">Read-only.</span></span> |
|<span data-ttu-id="20b03-116">displayName</span><span class="sxs-lookup"><span data-stu-id="20b03-116">displayName</span></span>|<span data-ttu-id="20b03-117">String</span><span class="sxs-lookup"><span data-stu-id="20b03-117">String</span></span>| <span data-ttu-id="20b03-118">返回的目录对象的名称，如 group 或 application。</span><span class="sxs-lookup"><span data-stu-id="20b03-118">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="20b03-119">只读。</span><span class="sxs-lookup"><span data-stu-id="20b03-119">Read-only.</span></span> |
|<span data-ttu-id="20b03-120">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="20b03-120">externalPartnerTenantId</span></span>|<span data-ttu-id="20b03-121">Guid</span><span class="sxs-lookup"><span data-stu-id="20b03-121">Guid</span></span>| <span data-ttu-id="20b03-122">合作伙伴租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="20b03-122">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="20b03-123">只读。</span><span class="sxs-lookup"><span data-stu-id="20b03-123">Read-only.</span></span> |
|<span data-ttu-id="20b03-124">id</span><span class="sxs-lookup"><span data-stu-id="20b03-124">id</span></span>|<span data-ttu-id="20b03-125">String</span><span class="sxs-lookup"><span data-stu-id="20b03-125">String</span></span>| <span data-ttu-id="20b03-126">资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="20b03-126">The unique identifier for the resource.</span></span> <span data-ttu-id="20b03-127">继承自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)。</span><span class="sxs-lookup"><span data-stu-id="20b03-127">Inherited from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span> <span data-ttu-id="20b03-128">只读。</span><span class="sxs-lookup"><span data-stu-id="20b03-128">Read-only.</span></span> |
|<span data-ttu-id="20b03-129">objectType</span><span class="sxs-lookup"><span data-stu-id="20b03-129">objectType</span></span>|<span data-ttu-id="20b03-130">String</span><span class="sxs-lookup"><span data-stu-id="20b03-130">String</span></span>| <span data-ttu-id="20b03-131">合作伙伴租户中被引用对象的类型。</span><span class="sxs-lookup"><span data-stu-id="20b03-131">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="20b03-132">只读。</span><span class="sxs-lookup"><span data-stu-id="20b03-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="20b03-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20b03-133">JSON representation</span></span>

<span data-ttu-id="20b03-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20b03-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="20b03-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="20b03-135">See also</span></span>

- [<span data-ttu-id="20b03-136">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="20b03-136">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-v1.0)

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

