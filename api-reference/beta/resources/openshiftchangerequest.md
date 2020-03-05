---
title: openShiftChangeRequest 资源类型
description: 表示在计划中声明打开的班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b4ca3b0904ffa0ec5bf06c36e710abdf3ba2a1dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522177"
---
# <a name="openshiftchangerequest-resource-type"></a><span data-ttu-id="48d82-103">openShiftChangeRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="48d82-103">openShiftChangeRequest resource type</span></span>

<span data-ttu-id="48d82-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="48d82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48d82-105">表示在[计划](../resources/schedule.md)中对[openshift](../resources/openshift.md)进行声明的班次请求的类型。</span><span class="sxs-lookup"><span data-stu-id="48d82-105">Represents a type of shift request to claim an [openshift](../resources/openshift.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="48d82-106">方法</span><span class="sxs-lookup"><span data-stu-id="48d82-106">Methods</span></span>

| <span data-ttu-id="48d82-107">方法</span><span class="sxs-lookup"><span data-stu-id="48d82-107">Method</span></span>       | <span data-ttu-id="48d82-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="48d82-108">Return Type</span></span> | <span data-ttu-id="48d82-109">说明</span><span class="sxs-lookup"><span data-stu-id="48d82-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="48d82-110">Create</span><span class="sxs-lookup"><span data-stu-id="48d82-110">Create</span></span>](../api/openshiftchangerequest-post.md) | [<span data-ttu-id="48d82-111">openshiftchangerequest</span><span class="sxs-lookup"><span data-stu-id="48d82-111">openshiftchangerequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="48d82-112">创建 openshiftchangerequest 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="48d82-112">Create an instance of an openshiftchangerequest object.</span></span> |
| [<span data-ttu-id="48d82-113">List</span><span class="sxs-lookup"><span data-stu-id="48d82-113">List</span></span>](../api/openshiftchangerequest-list.md) | <span data-ttu-id="48d82-114">[Openshiftchangerequest](openshiftchangerequest.md)的集合</span><span class="sxs-lookup"><span data-stu-id="48d82-114">Collection of [openshiftchangerequest](openshiftchangerequest.md)</span></span> | <span data-ttu-id="48d82-115">列出团队中的**openShiftChangeRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="48d82-115">List the properties and relationships of **openShiftChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="48d82-116">获取</span><span class="sxs-lookup"><span data-stu-id="48d82-116">Get</span></span>](../api/openshiftchangerequest-get.md) | [<span data-ttu-id="48d82-117">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="48d82-117">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="48d82-118">读取**openShiftChangeRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="48d82-118">Read the properties and relationships of an **openShiftChangeRequest** object.</span></span> |
|[<span data-ttu-id="48d82-119">批准</span><span class="sxs-lookup"><span data-stu-id="48d82-119">Approve</span></span>](../api/openshiftchangerequest-approve.md)|<span data-ttu-id="48d82-120">无</span><span class="sxs-lookup"><span data-stu-id="48d82-120">None</span></span>|<span data-ttu-id="48d82-121">批准打开的班次更改请求。</span><span class="sxs-lookup"><span data-stu-id="48d82-121">Approve an open shift change request.</span></span>|
|[<span data-ttu-id="48d82-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="48d82-122">Decline</span></span>](../api/openshiftchangerequest-decline.md)|<span data-ttu-id="48d82-123">无</span><span class="sxs-lookup"><span data-stu-id="48d82-123">None</span></span>| <span data-ttu-id="48d82-124">拒绝打开的班次更改请求。</span><span class="sxs-lookup"><span data-stu-id="48d82-124">Decline an open shift change request.</span></span>|

## <a name="properties"></a><span data-ttu-id="48d82-125">属性</span><span class="sxs-lookup"><span data-stu-id="48d82-125">Properties</span></span>

| <span data-ttu-id="48d82-126">属性</span><span class="sxs-lookup"><span data-stu-id="48d82-126">Property</span></span>     | <span data-ttu-id="48d82-127">类型</span><span class="sxs-lookup"><span data-stu-id="48d82-127">Type</span></span>        | <span data-ttu-id="48d82-128">说明</span><span class="sxs-lookup"><span data-stu-id="48d82-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="48d82-129">openShiftId</span><span class="sxs-lookup"><span data-stu-id="48d82-129">openShiftId</span></span>|<span data-ttu-id="48d82-130">String</span><span class="sxs-lookup"><span data-stu-id="48d82-130">String</span></span>| <span data-ttu-id="48d82-131">打开的班次的 ID。</span><span class="sxs-lookup"><span data-stu-id="48d82-131">ID for the open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48d82-132">关系</span><span class="sxs-lookup"><span data-stu-id="48d82-132">Relationships</span></span>

<span data-ttu-id="48d82-133">无。</span><span class="sxs-lookup"><span data-stu-id="48d82-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="48d82-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48d82-134">JSON representation</span></span>

<span data-ttu-id="48d82-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48d82-135">The following is a JSON representation of the resource.</span></span>

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
