---
title: openShift 资源类型
description: 代表计划中未分配的打开班次。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f3ce94c12328e9c05f899c5d2176339bbed93432
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951935"
---
# <a name="openshift-resource-type"></a><span data-ttu-id="ed9d7-103">openShift 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed9d7-103">openShift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed9d7-104">代表[计划](../resources/schedule.md)中未分配的打开班次。</span><span class="sxs-lookup"><span data-stu-id="ed9d7-104">Represents an unassigned, open shift in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ed9d7-105">Methods</span><span class="sxs-lookup"><span data-stu-id="ed9d7-105">Methods</span></span>

| <span data-ttu-id="ed9d7-106">方法</span><span class="sxs-lookup"><span data-stu-id="ed9d7-106">Method</span></span>       | <span data-ttu-id="ed9d7-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="ed9d7-107">Return Type</span></span> | <span data-ttu-id="ed9d7-108">说明</span><span class="sxs-lookup"><span data-stu-id="ed9d7-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ed9d7-109">Create</span><span class="sxs-lookup"><span data-stu-id="ed9d7-109">Create</span></span>](../api/openshift-post.md) | [<span data-ttu-id="ed9d7-110">openShift</span><span class="sxs-lookup"><span data-stu-id="ed9d7-110">openShift</span></span>](openshift.md) | <span data-ttu-id="ed9d7-111">创建**openShift**对象的实例。</span><span class="sxs-lookup"><span data-stu-id="ed9d7-111">Create an instance of an **openShift** object.</span></span> |
| [<span data-ttu-id="ed9d7-112">List</span><span class="sxs-lookup"><span data-stu-id="ed9d7-112">List</span></span>](../api/openshift-list.md) | <span data-ttu-id="ed9d7-113">[OpenShift](openshift.md)的集合</span><span class="sxs-lookup"><span data-stu-id="ed9d7-113">Collection of [openShift](openshift.md)</span></span> | <span data-ttu-id="ed9d7-114">列出团队中的**openShift**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed9d7-114">List the properties and relationships of **openShift** objects in a team.</span></span>|
| [<span data-ttu-id="ed9d7-115">Get</span><span class="sxs-lookup"><span data-stu-id="ed9d7-115">Get</span></span>](../api/openshift-get.md) | [<span data-ttu-id="ed9d7-116">openShift</span><span class="sxs-lookup"><span data-stu-id="ed9d7-116">openShift</span></span>](openshift.md) | <span data-ttu-id="ed9d7-117">读取**openShift**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed9d7-117">Read the properties and relationships of an **openShift** object.</span></span> |
| [<span data-ttu-id="ed9d7-118">更新</span><span class="sxs-lookup"><span data-stu-id="ed9d7-118">Update</span></span>](../api/openshift-update.md) | [<span data-ttu-id="ed9d7-119">openShift</span><span class="sxs-lookup"><span data-stu-id="ed9d7-119">openShift</span></span>](openshift.md) | <span data-ttu-id="ed9d7-120">更新**openShift**对象。</span><span class="sxs-lookup"><span data-stu-id="ed9d7-120">Update an **openShift** object.</span></span> |
| [<span data-ttu-id="ed9d7-121">删除</span><span class="sxs-lookup"><span data-stu-id="ed9d7-121">Delete</span></span>](../api/openshift-delete.md) | <span data-ttu-id="ed9d7-122">无</span><span class="sxs-lookup"><span data-stu-id="ed9d7-122">None</span></span> | <span data-ttu-id="ed9d7-123">删除**openShift**对象。</span><span class="sxs-lookup"><span data-stu-id="ed9d7-123">Delete an **openShift** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ed9d7-124">属性</span><span class="sxs-lookup"><span data-stu-id="ed9d7-124">Properties</span></span>

| <span data-ttu-id="ed9d7-125">属性</span><span class="sxs-lookup"><span data-stu-id="ed9d7-125">Property</span></span>     | <span data-ttu-id="ed9d7-126">类型</span><span class="sxs-lookup"><span data-stu-id="ed9d7-126">Type</span></span>        | <span data-ttu-id="ed9d7-127">Description</span><span class="sxs-lookup"><span data-stu-id="ed9d7-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ed9d7-128">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="ed9d7-128">draftOpenShift</span></span>|[<span data-ttu-id="ed9d7-129">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="ed9d7-129">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="ed9d7-130">未发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="ed9d7-130">An unpublished open shift.</span></span>|
|<span data-ttu-id="ed9d7-131">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="ed9d7-131">schedulingGroupId</span></span>|<span data-ttu-id="ed9d7-132">String</span><span class="sxs-lookup"><span data-stu-id="ed9d7-132">String</span></span>|<span data-ttu-id="ed9d7-133">打开的班次所属的计划组的 ID。</span><span class="sxs-lookup"><span data-stu-id="ed9d7-133">ID for the scheduling group that the open shift belongs to.</span></span>|
|<span data-ttu-id="ed9d7-134">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="ed9d7-134">sharedOpenShift</span></span>|[<span data-ttu-id="ed9d7-135">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="ed9d7-135">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="ed9d7-136">已发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="ed9d7-136">A published open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed9d7-137">关系</span><span class="sxs-lookup"><span data-stu-id="ed9d7-137">Relationships</span></span>

<span data-ttu-id="ed9d7-138">无。</span><span class="sxs-lookup"><span data-stu-id="ed9d7-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed9d7-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed9d7-139">JSON representation</span></span>

<span data-ttu-id="ed9d7-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed9d7-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShift",
  "baseType": ""
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
