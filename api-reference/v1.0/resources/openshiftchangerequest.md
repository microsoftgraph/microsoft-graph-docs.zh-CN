---
title: openShiftChangeRequest 资源类型
description: 代表在计划中声明打开的班次的请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ad13d42eb5c4617292be449e1a517d376a3bf8a7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028278"
---
# <a name="openshiftchangerequest-resource-type"></a><span data-ttu-id="0fe11-103">openShiftChangeRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fe11-103">openShiftChangeRequest resource type</span></span>

<span data-ttu-id="0fe11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fe11-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0fe11-105">表示在[计划](../resources/schedule.md)中声明[openShift](../resources/openshift.md)的请求。</span><span class="sxs-lookup"><span data-stu-id="0fe11-105">Represents request to claim an [openShift](../resources/openshift.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0fe11-106">方法</span><span class="sxs-lookup"><span data-stu-id="0fe11-106">Methods</span></span>

| <span data-ttu-id="0fe11-107">方法</span><span class="sxs-lookup"><span data-stu-id="0fe11-107">Method</span></span>       | <span data-ttu-id="0fe11-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0fe11-108">Return Type</span></span> | <span data-ttu-id="0fe11-109">Description</span><span class="sxs-lookup"><span data-stu-id="0fe11-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0fe11-110">List</span><span class="sxs-lookup"><span data-stu-id="0fe11-110">List</span></span>](../api/openshiftchangerequest-list.md) | <span data-ttu-id="0fe11-111">[OpenShiftChangeRequest](openshiftchangerequest.md)的集合</span><span class="sxs-lookup"><span data-stu-id="0fe11-111">Collection of [openShiftChangeRequest](openshiftchangerequest.md)</span></span> | <span data-ttu-id="0fe11-112">列出团队中的 **openShiftChangeRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fe11-112">List the properties and relationships of **openShiftChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="0fe11-113">创建</span><span class="sxs-lookup"><span data-stu-id="0fe11-113">Create</span></span>](../api/openshiftchangerequest-post.md) | [<span data-ttu-id="0fe11-114">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="0fe11-114">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="0fe11-115">创建 **openShiftChangeRequest** 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="0fe11-115">Create an instance of an **openShiftChangeRequest** object.</span></span> |
| [<span data-ttu-id="0fe11-116">获取</span><span class="sxs-lookup"><span data-stu-id="0fe11-116">Get</span></span>](../api/openshiftchangerequest-get.md) | [<span data-ttu-id="0fe11-117">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="0fe11-117">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="0fe11-118">读取 **openShiftChangeRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fe11-118">Read the properties and relationships of an **openShiftChangeRequest** object.</span></span> |
|[<span data-ttu-id="0fe11-119">批准</span><span class="sxs-lookup"><span data-stu-id="0fe11-119">Approve</span></span>](../api/openshiftchangerequest-approve.md)|<span data-ttu-id="0fe11-120">无</span><span class="sxs-lookup"><span data-stu-id="0fe11-120">None</span></span>|<span data-ttu-id="0fe11-121">批准打开的班次更改请求。</span><span class="sxs-lookup"><span data-stu-id="0fe11-121">Approve an open shift change request.</span></span>|
|[<span data-ttu-id="0fe11-122">拒绝</span><span class="sxs-lookup"><span data-stu-id="0fe11-122">Decline</span></span>](../api/openshiftchangerequest-decline.md)|<span data-ttu-id="0fe11-123">无</span><span class="sxs-lookup"><span data-stu-id="0fe11-123">None</span></span>| <span data-ttu-id="0fe11-124">拒绝打开的班次更改请求。</span><span class="sxs-lookup"><span data-stu-id="0fe11-124">Decline an open shift change request.</span></span>|

## <a name="properties"></a><span data-ttu-id="0fe11-125">属性</span><span class="sxs-lookup"><span data-stu-id="0fe11-125">Properties</span></span>

| <span data-ttu-id="0fe11-126">属性</span><span class="sxs-lookup"><span data-stu-id="0fe11-126">Property</span></span>     | <span data-ttu-id="0fe11-127">类型</span><span class="sxs-lookup"><span data-stu-id="0fe11-127">Type</span></span>        | <span data-ttu-id="0fe11-128">说明</span><span class="sxs-lookup"><span data-stu-id="0fe11-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0fe11-129">openShiftId</span><span class="sxs-lookup"><span data-stu-id="0fe11-129">openShiftId</span></span>|<span data-ttu-id="0fe11-130">String</span><span class="sxs-lookup"><span data-stu-id="0fe11-130">String</span></span>| <span data-ttu-id="0fe11-131">打开的班次的 ID。</span><span class="sxs-lookup"><span data-stu-id="0fe11-131">ID for the open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fe11-132">关系</span><span class="sxs-lookup"><span data-stu-id="0fe11-132">Relationships</span></span>

<span data-ttu-id="0fe11-133">无。</span><span class="sxs-lookup"><span data-stu-id="0fe11-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fe11-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fe11-134">JSON representation</span></span>

<span data-ttu-id="0fe11-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fe11-135">The following is a JSON representation of the resource.</span></span>

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

