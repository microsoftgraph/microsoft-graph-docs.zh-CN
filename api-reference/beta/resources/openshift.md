---
title: openShift 资源类型
description: 表示计划中的未分配开放班次。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a272d985a4aa71e1c1fdfc83baed51379010d7dc
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159463"
---
# <a name="openshift-resource-type"></a><span data-ttu-id="e64ba-103">openShift 资源类型</span><span class="sxs-lookup"><span data-stu-id="e64ba-103">openShift resource type</span></span>

<span data-ttu-id="e64ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e64ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e64ba-105">表示计划的未分配、打开的 [班次](../resources/schedule.md)。</span><span class="sxs-lookup"><span data-stu-id="e64ba-105">Represents an unassigned, open shift in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e64ba-106">方法</span><span class="sxs-lookup"><span data-stu-id="e64ba-106">Methods</span></span>

| <span data-ttu-id="e64ba-107">方法</span><span class="sxs-lookup"><span data-stu-id="e64ba-107">Method</span></span>       | <span data-ttu-id="e64ba-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e64ba-108">Return Type</span></span> | <span data-ttu-id="e64ba-109">说明</span><span class="sxs-lookup"><span data-stu-id="e64ba-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e64ba-110">创建</span><span class="sxs-lookup"><span data-stu-id="e64ba-110">Create</span></span>](../api/openshift-post.md) | [<span data-ttu-id="e64ba-111">openShift</span><span class="sxs-lookup"><span data-stu-id="e64ba-111">openShift</span></span>](openshift.md) | <span data-ttu-id="e64ba-112">创建 **openShift 对象** 的实例。</span><span class="sxs-lookup"><span data-stu-id="e64ba-112">Create an instance of an **openShift** object.</span></span> |
| [<span data-ttu-id="e64ba-113">列表</span><span class="sxs-lookup"><span data-stu-id="e64ba-113">List</span></span>](../api/openshift-list.md) | <span data-ttu-id="e64ba-114">[openShift 集合](openshift.md)</span><span class="sxs-lookup"><span data-stu-id="e64ba-114">Collection of [openShift](openshift.md)</span></span> | <span data-ttu-id="e64ba-115">列出团队 **中 openShift** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e64ba-115">List the properties and relationships of **openShift** objects in a team.</span></span>|
| [<span data-ttu-id="e64ba-116">Get</span><span class="sxs-lookup"><span data-stu-id="e64ba-116">Get</span></span>](../api/openshift-get.md) | [<span data-ttu-id="e64ba-117">openShift</span><span class="sxs-lookup"><span data-stu-id="e64ba-117">openShift</span></span>](openshift.md) | <span data-ttu-id="e64ba-118">读取 **openShift 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="e64ba-118">Read the properties and relationships of an **openShift** object.</span></span> |
| [<span data-ttu-id="e64ba-119">更新</span><span class="sxs-lookup"><span data-stu-id="e64ba-119">Update</span></span>](../api/openshift-update.md) | [<span data-ttu-id="e64ba-120">openShift</span><span class="sxs-lookup"><span data-stu-id="e64ba-120">openShift</span></span>](openshift.md) | <span data-ttu-id="e64ba-121">更新 **openShift** 对象。</span><span class="sxs-lookup"><span data-stu-id="e64ba-121">Update an **openShift** object.</span></span> |
| [<span data-ttu-id="e64ba-122">删除</span><span class="sxs-lookup"><span data-stu-id="e64ba-122">Delete</span></span>](../api/openshift-delete.md) | <span data-ttu-id="e64ba-123">无</span><span class="sxs-lookup"><span data-stu-id="e64ba-123">None</span></span> | <span data-ttu-id="e64ba-124">删除 **openShift** 对象。</span><span class="sxs-lookup"><span data-stu-id="e64ba-124">Delete an **openShift** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e64ba-125">属性</span><span class="sxs-lookup"><span data-stu-id="e64ba-125">Properties</span></span>

| <span data-ttu-id="e64ba-126">属性</span><span class="sxs-lookup"><span data-stu-id="e64ba-126">Property</span></span>     | <span data-ttu-id="e64ba-127">类型</span><span class="sxs-lookup"><span data-stu-id="e64ba-127">Type</span></span>        | <span data-ttu-id="e64ba-128">说明</span><span class="sxs-lookup"><span data-stu-id="e64ba-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e64ba-129">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="e64ba-129">draftOpenShift</span></span>|[<span data-ttu-id="e64ba-130">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="e64ba-130">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="e64ba-131">未发布的开放班次。</span><span class="sxs-lookup"><span data-stu-id="e64ba-131">An unpublished open shift.</span></span>|
|<span data-ttu-id="e64ba-132">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="e64ba-132">schedulingGroupId</span></span>|<span data-ttu-id="e64ba-133">String</span><span class="sxs-lookup"><span data-stu-id="e64ba-133">String</span></span>|<span data-ttu-id="e64ba-134">开放班次所属的计划组的 ID。</span><span class="sxs-lookup"><span data-stu-id="e64ba-134">ID for the scheduling group that the open shift belongs to.</span></span>|
|<span data-ttu-id="e64ba-135">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="e64ba-135">sharedOpenShift</span></span>|[<span data-ttu-id="e64ba-136">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="e64ba-136">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="e64ba-137">已发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="e64ba-137">A published open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e64ba-138">关系</span><span class="sxs-lookup"><span data-stu-id="e64ba-138">Relationships</span></span>

<span data-ttu-id="e64ba-139">无。</span><span class="sxs-lookup"><span data-stu-id="e64ba-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e64ba-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e64ba-140">JSON representation</span></span>

<span data-ttu-id="e64ba-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e64ba-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShift"
}-->

```json
{
  "draftOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"},
  "schedulingGroupId": "String",
  "sharedOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


