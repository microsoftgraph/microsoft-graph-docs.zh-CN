---
title: openShiftChangeRequest 资源类型
description: 表示用于声明计划中打开的班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e141dcb6657c9efc7d751b1713aa8b53d79c9264
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161416"
---
# <a name="openshiftchangerequest-resource-type"></a><span data-ttu-id="497e1-103">openShiftChangeRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="497e1-103">openShiftChangeRequest resource type</span></span>

<span data-ttu-id="497e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="497e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="497e1-105">表示一种班次请求，以声明 [在](../resources/openshift.md) 计划中的开放 [临时](../resources/schedule.md)。</span><span class="sxs-lookup"><span data-stu-id="497e1-105">Represents a type of shift request to claim an [openshift](../resources/openshift.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="497e1-106">方法</span><span class="sxs-lookup"><span data-stu-id="497e1-106">Methods</span></span>

| <span data-ttu-id="497e1-107">方法</span><span class="sxs-lookup"><span data-stu-id="497e1-107">Method</span></span>       | <span data-ttu-id="497e1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="497e1-108">Return Type</span></span> | <span data-ttu-id="497e1-109">说明</span><span class="sxs-lookup"><span data-stu-id="497e1-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="497e1-110">创建</span><span class="sxs-lookup"><span data-stu-id="497e1-110">Create</span></span>](../api/openshiftchangerequest-post.md) | [<span data-ttu-id="497e1-111">openshiftchangerequest</span><span class="sxs-lookup"><span data-stu-id="497e1-111">openshiftchangerequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="497e1-112">创建 openshiftchangerequest 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="497e1-112">Create an instance of an openshiftchangerequest object.</span></span> |
| [<span data-ttu-id="497e1-113">列表</span><span class="sxs-lookup"><span data-stu-id="497e1-113">List</span></span>](../api/openshiftchangerequest-list.md) | <span data-ttu-id="497e1-114">[openshiftchangerequest 的集合](openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="497e1-114">Collection of [openshiftchangerequest](openshiftchangerequest.md)</span></span> | <span data-ttu-id="497e1-115">列出团队 **中 openShiftChangeRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="497e1-115">List the properties and relationships of **openShiftChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="497e1-116">Get</span><span class="sxs-lookup"><span data-stu-id="497e1-116">Get</span></span>](../api/openshiftchangerequest-get.md) | [<span data-ttu-id="497e1-117">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="497e1-117">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="497e1-118">读取 **openShiftChangeRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="497e1-118">Read the properties and relationships of an **openShiftChangeRequest** object.</span></span> |
|[<span data-ttu-id="497e1-119">批准</span><span class="sxs-lookup"><span data-stu-id="497e1-119">Approve</span></span>](../api/openshiftchangerequest-approve.md)|<span data-ttu-id="497e1-120">无</span><span class="sxs-lookup"><span data-stu-id="497e1-120">None</span></span>|<span data-ttu-id="497e1-121">批准打开的班次更改请求。</span><span class="sxs-lookup"><span data-stu-id="497e1-121">Approve an open shift change request.</span></span>|
|[<span data-ttu-id="497e1-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="497e1-122">Decline</span></span>](../api/openshiftchangerequest-decline.md)|<span data-ttu-id="497e1-123">无</span><span class="sxs-lookup"><span data-stu-id="497e1-123">None</span></span>| <span data-ttu-id="497e1-124">拒绝打开的班次更改请求。</span><span class="sxs-lookup"><span data-stu-id="497e1-124">Decline an open shift change request.</span></span>|

## <a name="properties"></a><span data-ttu-id="497e1-125">属性</span><span class="sxs-lookup"><span data-stu-id="497e1-125">Properties</span></span>

| <span data-ttu-id="497e1-126">属性</span><span class="sxs-lookup"><span data-stu-id="497e1-126">Property</span></span>     | <span data-ttu-id="497e1-127">类型</span><span class="sxs-lookup"><span data-stu-id="497e1-127">Type</span></span>        | <span data-ttu-id="497e1-128">说明</span><span class="sxs-lookup"><span data-stu-id="497e1-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="497e1-129">openShiftId</span><span class="sxs-lookup"><span data-stu-id="497e1-129">openShiftId</span></span>|<span data-ttu-id="497e1-130">String</span><span class="sxs-lookup"><span data-stu-id="497e1-130">String</span></span>| <span data-ttu-id="497e1-131">打开的班次的 ID。</span><span class="sxs-lookup"><span data-stu-id="497e1-131">ID for the open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="497e1-132">关系</span><span class="sxs-lookup"><span data-stu-id="497e1-132">Relationships</span></span>

<span data-ttu-id="497e1-133">无。</span><span class="sxs-lookup"><span data-stu-id="497e1-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="497e1-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="497e1-134">JSON representation</span></span>

<span data-ttu-id="497e1-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="497e1-135">The following is a JSON representation of the resource.</span></span>

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


