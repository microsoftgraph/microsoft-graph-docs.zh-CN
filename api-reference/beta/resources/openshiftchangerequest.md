---
title: openShiftChangeRequest 资源类型
description: 表示在计划中声明打开的班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 69663b876e98bfe9f5c633890d02a6abd3b72f32
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951928"
---
# <a name="openshiftchangerequest-resource-type"></a><span data-ttu-id="f37aa-103">openShiftChangeRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="f37aa-103">openShiftChangeRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f37aa-104">表示在[计划](../resources/schedule.md)中对[openshift](../resources/openshift.md)进行声明的班次请求的类型。</span><span class="sxs-lookup"><span data-stu-id="f37aa-104">Represents a type of shift request to claim an [openshift](../resources/openshift.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f37aa-105">Methods</span><span class="sxs-lookup"><span data-stu-id="f37aa-105">Methods</span></span>

| <span data-ttu-id="f37aa-106">方法</span><span class="sxs-lookup"><span data-stu-id="f37aa-106">Method</span></span>       | <span data-ttu-id="f37aa-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f37aa-107">Return Type</span></span> | <span data-ttu-id="f37aa-108">说明</span><span class="sxs-lookup"><span data-stu-id="f37aa-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f37aa-109">Create</span><span class="sxs-lookup"><span data-stu-id="f37aa-109">Create</span></span>](../api/openshiftchangerequest-post.md) | [<span data-ttu-id="f37aa-110">openshiftchangerequest</span><span class="sxs-lookup"><span data-stu-id="f37aa-110">openshiftchangerequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="f37aa-111">创建 openshiftchangerequest 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="f37aa-111">Create an instance of an openshiftchangerequest object.</span></span> |
| [<span data-ttu-id="f37aa-112">List</span><span class="sxs-lookup"><span data-stu-id="f37aa-112">List</span></span>](../api/openshiftchangerequest-list.md) | <span data-ttu-id="f37aa-113">[Openshiftchangerequest](openshiftchangerequest.md)的集合</span><span class="sxs-lookup"><span data-stu-id="f37aa-113">Collection of [openshiftchangerequest](openshiftchangerequest.md)</span></span> | <span data-ttu-id="f37aa-114">列出团队中的**openShiftChangeRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f37aa-114">List the properties and relationships of **openShiftChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="f37aa-115">Get</span><span class="sxs-lookup"><span data-stu-id="f37aa-115">Get</span></span>](../api/openshiftchangerequest-get.md) | [<span data-ttu-id="f37aa-116">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="f37aa-116">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="f37aa-117">读取**openShiftChangeRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f37aa-117">Read the properties and relationships of an **openShiftChangeRequest** object.</span></span> |
|[<span data-ttu-id="f37aa-118">批准</span><span class="sxs-lookup"><span data-stu-id="f37aa-118">Approve</span></span>](../api/openshiftchangerequest-approve.md)|<span data-ttu-id="f37aa-119">无</span><span class="sxs-lookup"><span data-stu-id="f37aa-119">None</span></span>|<span data-ttu-id="f37aa-120">批准打开的班次更改请求。</span><span class="sxs-lookup"><span data-stu-id="f37aa-120">Approve an open shift change request.</span></span>|
|[<span data-ttu-id="f37aa-121">拒绝</span><span class="sxs-lookup"><span data-stu-id="f37aa-121">Decline</span></span>](../api/openshiftchangerequest-decline.md)|<span data-ttu-id="f37aa-122">无</span><span class="sxs-lookup"><span data-stu-id="f37aa-122">None</span></span>| <span data-ttu-id="f37aa-123">拒绝打开的班次更改请求。</span><span class="sxs-lookup"><span data-stu-id="f37aa-123">Decline an open shift change request.</span></span>|

## <a name="properties"></a><span data-ttu-id="f37aa-124">属性</span><span class="sxs-lookup"><span data-stu-id="f37aa-124">Properties</span></span>

| <span data-ttu-id="f37aa-125">属性</span><span class="sxs-lookup"><span data-stu-id="f37aa-125">Property</span></span>     | <span data-ttu-id="f37aa-126">类型</span><span class="sxs-lookup"><span data-stu-id="f37aa-126">Type</span></span>        | <span data-ttu-id="f37aa-127">Description</span><span class="sxs-lookup"><span data-stu-id="f37aa-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f37aa-128">openShiftId</span><span class="sxs-lookup"><span data-stu-id="f37aa-128">openShiftId</span></span>|<span data-ttu-id="f37aa-129">String</span><span class="sxs-lookup"><span data-stu-id="f37aa-129">String</span></span>| <span data-ttu-id="f37aa-130">打开的班次的 ID。</span><span class="sxs-lookup"><span data-stu-id="f37aa-130">ID for the open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f37aa-131">关系</span><span class="sxs-lookup"><span data-stu-id="f37aa-131">Relationships</span></span>

<span data-ttu-id="f37aa-132">无。</span><span class="sxs-lookup"><span data-stu-id="f37aa-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f37aa-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f37aa-133">JSON representation</span></span>

<span data-ttu-id="f37aa-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f37aa-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftChangeRequest",
  "baseType": ""
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
