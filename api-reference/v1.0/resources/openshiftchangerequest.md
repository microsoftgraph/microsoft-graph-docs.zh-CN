---
title: openShiftChangeRequest 资源类型
description: 表示请求在日程安排中声明打开的班次。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b427d7914d95aaed794734bbbb39fa3eb139d06a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158679"
---
# <a name="openshiftchangerequest-resource-type"></a><span data-ttu-id="33cfa-103">openShiftChangeRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="33cfa-103">openShiftChangeRequest resource type</span></span>

<span data-ttu-id="33cfa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33cfa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33cfa-105">表示按计划声明 [openShift](../resources/openshift.md) [的请求](../resources/schedule.md)。</span><span class="sxs-lookup"><span data-stu-id="33cfa-105">Represents request to claim an [openShift](../resources/openshift.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="33cfa-106">方法</span><span class="sxs-lookup"><span data-stu-id="33cfa-106">Methods</span></span>

| <span data-ttu-id="33cfa-107">方法</span><span class="sxs-lookup"><span data-stu-id="33cfa-107">Method</span></span>       | <span data-ttu-id="33cfa-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="33cfa-108">Return Type</span></span> | <span data-ttu-id="33cfa-109">Description</span><span class="sxs-lookup"><span data-stu-id="33cfa-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="33cfa-110">List</span><span class="sxs-lookup"><span data-stu-id="33cfa-110">List</span></span>](../api/openshiftchangerequest-list.md) | <span data-ttu-id="33cfa-111">[openShiftChangeRequest 集合](openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="33cfa-111">Collection of [openShiftChangeRequest](openshiftchangerequest.md)</span></span> | <span data-ttu-id="33cfa-112">列出团队 **中 openShiftChangeRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="33cfa-112">List the properties and relationships of **openShiftChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="33cfa-113">创建</span><span class="sxs-lookup"><span data-stu-id="33cfa-113">Create</span></span>](../api/openshiftchangerequest-post.md) | [<span data-ttu-id="33cfa-114">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="33cfa-114">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="33cfa-115">创建 **openShiftChangeRequest 对象** 的实例。</span><span class="sxs-lookup"><span data-stu-id="33cfa-115">Create an instance of an **openShiftChangeRequest** object.</span></span> |
| [<span data-ttu-id="33cfa-116">Get</span><span class="sxs-lookup"><span data-stu-id="33cfa-116">Get</span></span>](../api/openshiftchangerequest-get.md) | [<span data-ttu-id="33cfa-117">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="33cfa-117">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="33cfa-118">读取 **openShiftChangeRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="33cfa-118">Read the properties and relationships of an **openShiftChangeRequest** object.</span></span> |
|[<span data-ttu-id="33cfa-119">批准</span><span class="sxs-lookup"><span data-stu-id="33cfa-119">Approve</span></span>](../api/openshiftchangerequest-approve.md)|<span data-ttu-id="33cfa-120">无</span><span class="sxs-lookup"><span data-stu-id="33cfa-120">None</span></span>|<span data-ttu-id="33cfa-121">批准打开的班次更改请求。</span><span class="sxs-lookup"><span data-stu-id="33cfa-121">Approve an open shift change request.</span></span>|
|[<span data-ttu-id="33cfa-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="33cfa-122">Decline</span></span>](../api/openshiftchangerequest-decline.md)|<span data-ttu-id="33cfa-123">无</span><span class="sxs-lookup"><span data-stu-id="33cfa-123">None</span></span>| <span data-ttu-id="33cfa-124">拒绝打开的班次更改请求。</span><span class="sxs-lookup"><span data-stu-id="33cfa-124">Decline an open shift change request.</span></span>|

## <a name="properties"></a><span data-ttu-id="33cfa-125">属性</span><span class="sxs-lookup"><span data-stu-id="33cfa-125">Properties</span></span>

| <span data-ttu-id="33cfa-126">属性</span><span class="sxs-lookup"><span data-stu-id="33cfa-126">Property</span></span>     | <span data-ttu-id="33cfa-127">类型</span><span class="sxs-lookup"><span data-stu-id="33cfa-127">Type</span></span>        | <span data-ttu-id="33cfa-128">说明</span><span class="sxs-lookup"><span data-stu-id="33cfa-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="33cfa-129">openShiftId</span><span class="sxs-lookup"><span data-stu-id="33cfa-129">openShiftId</span></span>|<span data-ttu-id="33cfa-130">String</span><span class="sxs-lookup"><span data-stu-id="33cfa-130">String</span></span>| <span data-ttu-id="33cfa-131">打开的班次的 ID。</span><span class="sxs-lookup"><span data-stu-id="33cfa-131">ID for the open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33cfa-132">关系</span><span class="sxs-lookup"><span data-stu-id="33cfa-132">Relationships</span></span>

<span data-ttu-id="33cfa-133">无。</span><span class="sxs-lookup"><span data-stu-id="33cfa-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="33cfa-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33cfa-134">JSON representation</span></span>

<span data-ttu-id="33cfa-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33cfa-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
}-->

```json
{
  "openShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftChangeRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

