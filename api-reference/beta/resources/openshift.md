---
title: openShift 资源类型
description: 代表计划中未分配的打开班次。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 534756fd26fcac13d150e9cbd1782a8f334e5a2f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998563"
---
# <a name="openshift-resource-type"></a><span data-ttu-id="bba31-103">openShift 资源类型</span><span class="sxs-lookup"><span data-stu-id="bba31-103">openShift resource type</span></span>

<span data-ttu-id="bba31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bba31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bba31-105">代表 [计划](../resources/schedule.md)中未分配的打开班次。</span><span class="sxs-lookup"><span data-stu-id="bba31-105">Represents an unassigned, open shift in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="bba31-106">方法</span><span class="sxs-lookup"><span data-stu-id="bba31-106">Methods</span></span>

| <span data-ttu-id="bba31-107">方法</span><span class="sxs-lookup"><span data-stu-id="bba31-107">Method</span></span>       | <span data-ttu-id="bba31-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="bba31-108">Return Type</span></span> | <span data-ttu-id="bba31-109">说明</span><span class="sxs-lookup"><span data-stu-id="bba31-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bba31-110">创建</span><span class="sxs-lookup"><span data-stu-id="bba31-110">Create</span></span>](../api/openshift-post.md) | [<span data-ttu-id="bba31-111">openShift</span><span class="sxs-lookup"><span data-stu-id="bba31-111">openShift</span></span>](openshift.md) | <span data-ttu-id="bba31-112">创建 **openShift** 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="bba31-112">Create an instance of an **openShift** object.</span></span> |
| [<span data-ttu-id="bba31-113">List</span><span class="sxs-lookup"><span data-stu-id="bba31-113">List</span></span>](../api/openshift-list.md) | <span data-ttu-id="bba31-114">[OpenShift](openshift.md)的集合</span><span class="sxs-lookup"><span data-stu-id="bba31-114">Collection of [openShift](openshift.md)</span></span> | <span data-ttu-id="bba31-115">列出团队中的 **openShift** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bba31-115">List the properties and relationships of **openShift** objects in a team.</span></span>|
| [<span data-ttu-id="bba31-116">获取</span><span class="sxs-lookup"><span data-stu-id="bba31-116">Get</span></span>](../api/openshift-get.md) | [<span data-ttu-id="bba31-117">openShift</span><span class="sxs-lookup"><span data-stu-id="bba31-117">openShift</span></span>](openshift.md) | <span data-ttu-id="bba31-118">读取 **openShift** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bba31-118">Read the properties and relationships of an **openShift** object.</span></span> |
| [<span data-ttu-id="bba31-119">更新</span><span class="sxs-lookup"><span data-stu-id="bba31-119">Update</span></span>](../api/openshift-update.md) | [<span data-ttu-id="bba31-120">openShift</span><span class="sxs-lookup"><span data-stu-id="bba31-120">openShift</span></span>](openshift.md) | <span data-ttu-id="bba31-121">更新 **openShift** 对象。</span><span class="sxs-lookup"><span data-stu-id="bba31-121">Update an **openShift** object.</span></span> |
| [<span data-ttu-id="bba31-122">删除</span><span class="sxs-lookup"><span data-stu-id="bba31-122">Delete</span></span>](../api/openshift-delete.md) | <span data-ttu-id="bba31-123">无</span><span class="sxs-lookup"><span data-stu-id="bba31-123">None</span></span> | <span data-ttu-id="bba31-124">删除 **openShift** 对象。</span><span class="sxs-lookup"><span data-stu-id="bba31-124">Delete an **openShift** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bba31-125">属性</span><span class="sxs-lookup"><span data-stu-id="bba31-125">Properties</span></span>

| <span data-ttu-id="bba31-126">属性</span><span class="sxs-lookup"><span data-stu-id="bba31-126">Property</span></span>     | <span data-ttu-id="bba31-127">类型</span><span class="sxs-lookup"><span data-stu-id="bba31-127">Type</span></span>        | <span data-ttu-id="bba31-128">说明</span><span class="sxs-lookup"><span data-stu-id="bba31-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bba31-129">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="bba31-129">draftOpenShift</span></span>|[<span data-ttu-id="bba31-130">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="bba31-130">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="bba31-131">未发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="bba31-131">An unpublished open shift.</span></span>|
|<span data-ttu-id="bba31-132">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="bba31-132">schedulingGroupId</span></span>|<span data-ttu-id="bba31-133">String</span><span class="sxs-lookup"><span data-stu-id="bba31-133">String</span></span>|<span data-ttu-id="bba31-134">打开的班次所属的计划组的 ID。</span><span class="sxs-lookup"><span data-stu-id="bba31-134">ID for the scheduling group that the open shift belongs to.</span></span>|
|<span data-ttu-id="bba31-135">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="bba31-135">sharedOpenShift</span></span>|[<span data-ttu-id="bba31-136">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="bba31-136">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="bba31-137">已发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="bba31-137">A published open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bba31-138">关系</span><span class="sxs-lookup"><span data-stu-id="bba31-138">Relationships</span></span>

<span data-ttu-id="bba31-139">无。</span><span class="sxs-lookup"><span data-stu-id="bba31-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bba31-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bba31-140">JSON representation</span></span>

<span data-ttu-id="bba31-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bba31-141">The following is a JSON representation of the resource.</span></span>

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


