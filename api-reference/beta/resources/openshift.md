---
title: openShift 资源类型
description: 代表计划中未分配的打开班次。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa87acd2065a3a56f15016bb7708e73cebe63a31
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870157"
---
# <a name="openshift-resource-type"></a><span data-ttu-id="7f41c-103">openShift 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f41c-103">openShift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f41c-104">代表[计划](../resources/schedule.md)中未分配的打开班次。</span><span class="sxs-lookup"><span data-stu-id="7f41c-104">Represents an unassigned, open shift in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7f41c-105">方法</span><span class="sxs-lookup"><span data-stu-id="7f41c-105">Methods</span></span>

| <span data-ttu-id="7f41c-106">方法</span><span class="sxs-lookup"><span data-stu-id="7f41c-106">Method</span></span>       | <span data-ttu-id="7f41c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="7f41c-107">Return Type</span></span> | <span data-ttu-id="7f41c-108">说明</span><span class="sxs-lookup"><span data-stu-id="7f41c-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7f41c-109">获取</span><span class="sxs-lookup"><span data-stu-id="7f41c-109">Get</span></span>](../api/openshift-get.md) | [<span data-ttu-id="7f41c-110">openShift</span><span class="sxs-lookup"><span data-stu-id="7f41c-110">openShift</span></span>](openshift.md) | <span data-ttu-id="7f41c-111">读取**openShift**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7f41c-111">Read the properties and relationships of an **openShift** object.</span></span> |
| [<span data-ttu-id="7f41c-112">更新</span><span class="sxs-lookup"><span data-stu-id="7f41c-112">Update</span></span>](../api/openshift-update.md) | [<span data-ttu-id="7f41c-113">openShift</span><span class="sxs-lookup"><span data-stu-id="7f41c-113">openShift</span></span>](openshift.md) | <span data-ttu-id="7f41c-114">更新**openShift**对象。</span><span class="sxs-lookup"><span data-stu-id="7f41c-114">Update an **openShift** object.</span></span> |
| [<span data-ttu-id="7f41c-115">删除</span><span class="sxs-lookup"><span data-stu-id="7f41c-115">Delete</span></span>](../api/openshift-delete.md) | <span data-ttu-id="7f41c-116">无</span><span class="sxs-lookup"><span data-stu-id="7f41c-116">None</span></span> | <span data-ttu-id="7f41c-117">删除**openShift**对象。</span><span class="sxs-lookup"><span data-stu-id="7f41c-117">Delete an **openShift** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7f41c-118">属性</span><span class="sxs-lookup"><span data-stu-id="7f41c-118">Properties</span></span>

| <span data-ttu-id="7f41c-119">属性</span><span class="sxs-lookup"><span data-stu-id="7f41c-119">Property</span></span>     | <span data-ttu-id="7f41c-120">类型</span><span class="sxs-lookup"><span data-stu-id="7f41c-120">Type</span></span>        | <span data-ttu-id="7f41c-121">说明</span><span class="sxs-lookup"><span data-stu-id="7f41c-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7f41c-122">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="7f41c-122">draftOpenShift</span></span>|[<span data-ttu-id="7f41c-123">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="7f41c-123">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="7f41c-124">未发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="7f41c-124">An unpublished open shift.</span></span>|
|<span data-ttu-id="7f41c-125">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="7f41c-125">schedulingGroupId</span></span>|<span data-ttu-id="7f41c-126">String</span><span class="sxs-lookup"><span data-stu-id="7f41c-126">String</span></span>|<span data-ttu-id="7f41c-127">打开的班次所属的计划组的 ID。</span><span class="sxs-lookup"><span data-stu-id="7f41c-127">ID for the scheduling group that the open shift belongs to.</span></span>|
|<span data-ttu-id="7f41c-128">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="7f41c-128">sharedOpenShift</span></span>|[<span data-ttu-id="7f41c-129">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="7f41c-129">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="7f41c-130">已发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="7f41c-130">A published open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f41c-131">关系</span><span class="sxs-lookup"><span data-stu-id="7f41c-131">Relationships</span></span>

<span data-ttu-id="7f41c-132">无。</span><span class="sxs-lookup"><span data-stu-id="7f41c-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f41c-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f41c-133">JSON representation</span></span>

<span data-ttu-id="7f41c-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f41c-134">The following is a JSON representation of the resource.</span></span>

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
