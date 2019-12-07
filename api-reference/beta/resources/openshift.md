---
title: openShift 资源类型
description: 代表计划中未分配的打开班次。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3eff83475c4a36ec1c294c62b9e1b87673926d8d
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895626"
---
# <a name="openshift-resource-type"></a><span data-ttu-id="ff7f9-103">openShift 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff7f9-103">openShift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff7f9-104">代表[计划](../resources/schedule.md)中未分配的打开班次。</span><span class="sxs-lookup"><span data-stu-id="ff7f9-104">Represents an unassigned, open shift in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ff7f9-105">方法</span><span class="sxs-lookup"><span data-stu-id="ff7f9-105">Methods</span></span>

| <span data-ttu-id="ff7f9-106">方法</span><span class="sxs-lookup"><span data-stu-id="ff7f9-106">Method</span></span>       | <span data-ttu-id="ff7f9-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="ff7f9-107">Return Type</span></span> | <span data-ttu-id="ff7f9-108">说明</span><span class="sxs-lookup"><span data-stu-id="ff7f9-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ff7f9-109">获取</span><span class="sxs-lookup"><span data-stu-id="ff7f9-109">Get</span></span>](../api/openshift-get.md) | [<span data-ttu-id="ff7f9-110">openShift</span><span class="sxs-lookup"><span data-stu-id="ff7f9-110">openShift</span></span>](openshift.md) | <span data-ttu-id="ff7f9-111">读取 openShift 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff7f9-111">Read properties and relationships of openShift object.</span></span> |
| [<span data-ttu-id="ff7f9-112">更新</span><span class="sxs-lookup"><span data-stu-id="ff7f9-112">Update</span></span>](../api/openshift-update.md) | [<span data-ttu-id="ff7f9-113">openShift</span><span class="sxs-lookup"><span data-stu-id="ff7f9-113">openShift</span></span>](openshift.md) | <span data-ttu-id="ff7f9-114">更新 openShift 对象。</span><span class="sxs-lookup"><span data-stu-id="ff7f9-114">Update openShift object.</span></span> |
| [<span data-ttu-id="ff7f9-115">删除</span><span class="sxs-lookup"><span data-stu-id="ff7f9-115">Delete</span></span>](../api/openshift-delete.md) | <span data-ttu-id="ff7f9-116">None</span><span class="sxs-lookup"><span data-stu-id="ff7f9-116">None</span></span> | <span data-ttu-id="ff7f9-117">删除 openShift 对象。</span><span class="sxs-lookup"><span data-stu-id="ff7f9-117">Delete openShift object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ff7f9-118">属性</span><span class="sxs-lookup"><span data-stu-id="ff7f9-118">Properties</span></span>

| <span data-ttu-id="ff7f9-119">属性</span><span class="sxs-lookup"><span data-stu-id="ff7f9-119">Property</span></span>     | <span data-ttu-id="ff7f9-120">类型</span><span class="sxs-lookup"><span data-stu-id="ff7f9-120">Type</span></span>        | <span data-ttu-id="ff7f9-121">说明</span><span class="sxs-lookup"><span data-stu-id="ff7f9-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff7f9-122">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="ff7f9-122">draftOpenShift</span></span>|[<span data-ttu-id="ff7f9-123">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="ff7f9-123">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="ff7f9-124">未发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="ff7f9-124">An unpublished open shift.</span></span>|
|<span data-ttu-id="ff7f9-125">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="ff7f9-125">schedulingGroupId</span></span>|<span data-ttu-id="ff7f9-126">字符串</span><span class="sxs-lookup"><span data-stu-id="ff7f9-126">String</span></span>|<span data-ttu-id="ff7f9-127">打开的班次所属的计划组的 ID。</span><span class="sxs-lookup"><span data-stu-id="ff7f9-127">ID for the scheduling group that the open shift belongs to.</span></span>|
|<span data-ttu-id="ff7f9-128">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="ff7f9-128">sharedOpenShift</span></span>|[<span data-ttu-id="ff7f9-129">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="ff7f9-129">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="ff7f9-130">已发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="ff7f9-130">A published open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff7f9-131">关系</span><span class="sxs-lookup"><span data-stu-id="ff7f9-131">Relationships</span></span>

<span data-ttu-id="ff7f9-132">无。</span><span class="sxs-lookup"><span data-stu-id="ff7f9-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff7f9-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff7f9-133">JSON representation</span></span>

<span data-ttu-id="ff7f9-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff7f9-134">The following is a JSON representation of the resource.</span></span>

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
