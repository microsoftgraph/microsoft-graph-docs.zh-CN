---
title: securityResource 资源类型
description: 代表与警报相关的资源。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ce0398ba134f7537420a99ccaed84f2ff209f883
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682017"
---
# <a name="securityresource-resource-type"></a><span data-ttu-id="c9815-103">securityResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9815-103">securityResource resource type</span></span>

<span data-ttu-id="c9815-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9815-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c9815-105">代表与警报相关的资源。</span><span class="sxs-lookup"><span data-stu-id="c9815-105">Represents the resources related to an alert.</span></span>

## <a name="properties"></a><span data-ttu-id="c9815-106">属性</span><span class="sxs-lookup"><span data-stu-id="c9815-106">Properties</span></span>

| <span data-ttu-id="c9815-107">属性</span><span class="sxs-lookup"><span data-stu-id="c9815-107">Property</span></span>   | <span data-ttu-id="c9815-108">类型</span><span class="sxs-lookup"><span data-stu-id="c9815-108">Type</span></span>|<span data-ttu-id="c9815-109">Description</span><span class="sxs-lookup"><span data-stu-id="c9815-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9815-110">资源</span><span class="sxs-lookup"><span data-stu-id="c9815-110">resource</span></span>|<span data-ttu-id="c9815-111">String</span><span class="sxs-lookup"><span data-stu-id="c9815-111">String</span></span>|<span data-ttu-id="c9815-112">与当前警报相关的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="c9815-112">Name of the resource that is related to current alert.</span></span> <span data-ttu-id="c9815-113">\*\*\*\* 必需。</span><span class="sxs-lookup"><span data-stu-id="c9815-113">**Required**.</span></span>|
|<span data-ttu-id="c9815-114">resourceType</span><span class="sxs-lookup"><span data-stu-id="c9815-114">resourceType</span></span>|[<span data-ttu-id="c9815-115">securityResourceType</span><span class="sxs-lookup"><span data-stu-id="c9815-115">securityResourceType</span></span>](#securityresourcetype-values)|<span data-ttu-id="c9815-116">表示与警报相关的安全资源的类型。</span><span class="sxs-lookup"><span data-stu-id="c9815-116">Represents type of security resources related to an alert.</span></span> <span data-ttu-id="c9815-117">可取值为：`attacked`、`related`。</span><span class="sxs-lookup"><span data-stu-id="c9815-117">Possible values are: `attacked`, `related`.</span></span>|

### <a name="securityresourcetype-values"></a><span data-ttu-id="c9815-118">securityResourceType 值</span><span class="sxs-lookup"><span data-stu-id="c9815-118">securityResourceType values</span></span>

|<span data-ttu-id="c9815-119">成员</span><span class="sxs-lookup"><span data-stu-id="c9815-119">Member</span></span>|<span data-ttu-id="c9815-120">值</span><span class="sxs-lookup"><span data-stu-id="c9815-120">Value</span></span>|<span data-ttu-id="c9815-121">说明</span><span class="sxs-lookup"><span data-stu-id="c9815-121">Description</span></span>|
|-|-|-|
|<span data-ttu-id="c9815-122">遭受</span><span class="sxs-lookup"><span data-stu-id="c9815-122">attacked</span></span>|<span data-ttu-id="c9815-123">1 </span><span class="sxs-lookup"><span data-stu-id="c9815-123">1</span></span>|<span data-ttu-id="c9815-124">警报中的资源受到攻击。</span><span class="sxs-lookup"><span data-stu-id="c9815-124">The resource was attacked in the alert.</span></span>|
|<span data-ttu-id="c9815-125">关联方</span><span class="sxs-lookup"><span data-stu-id="c9815-125">related</span></span>|<span data-ttu-id="c9815-126">双面</span><span class="sxs-lookup"><span data-stu-id="c9815-126">2</span></span>|<span data-ttu-id="c9815-127">该资源与警报相关，但不直接受到攻击。</span><span class="sxs-lookup"><span data-stu-id="c9815-127">The resource is related to the alert, though not directly attacked.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9815-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9815-128">JSON representation</span></span>

<span data-ttu-id="c9815-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9815-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.securityResource"
}-->

```json
{
  "resource": "String",
  "resourceType": "@odata.type: microsoft.graph.securityResourceType"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
