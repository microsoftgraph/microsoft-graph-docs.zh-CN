---
title: openShiftChangeRequest 资源类型
description: 表示在计划中声明打开的班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 400444ccccc13d103420cc95c522a6ed0aa1afa6
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895625"
---
# <a name="openshiftchangerequest-resource-type"></a><span data-ttu-id="8959b-103">openShiftChangeRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="8959b-103">openShiftChangeRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8959b-104">表示在[计划](../resources/schedule.md)中对[openshift](../resources/openshift.md)进行声明的班次请求的类型。</span><span class="sxs-lookup"><span data-stu-id="8959b-104">Represents a type of shift request to claim an [openshift](../resources/openshift.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8959b-105">方法</span><span class="sxs-lookup"><span data-stu-id="8959b-105">Methods</span></span>

| <span data-ttu-id="8959b-106">方法</span><span class="sxs-lookup"><span data-stu-id="8959b-106">Method</span></span>       | <span data-ttu-id="8959b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="8959b-107">Return Type</span></span> | <span data-ttu-id="8959b-108">说明</span><span class="sxs-lookup"><span data-stu-id="8959b-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8959b-109">获取</span><span class="sxs-lookup"><span data-stu-id="8959b-109">Get</span></span>](../api/openshiftchangerequest-get.md) | [<span data-ttu-id="8959b-110">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="8959b-110">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="8959b-111">读取**openShiftChangeRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8959b-111">Read the properties and relationships of an **openShiftChangeRequest** object.</span></span> |
| [<span data-ttu-id="8959b-112">更新</span><span class="sxs-lookup"><span data-stu-id="8959b-112">Update</span></span>](../api/openshiftchangerequest-update.md) | [<span data-ttu-id="8959b-113">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="8959b-113">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="8959b-114">更新**openShiftChangeRequest**对象。</span><span class="sxs-lookup"><span data-stu-id="8959b-114">Update an **openShiftChangeRequest** object.</span></span> |
| [<span data-ttu-id="8959b-115">删除</span><span class="sxs-lookup"><span data-stu-id="8959b-115">Delete</span></span>](../api/openshiftchangerequest-delete.md) | <span data-ttu-id="8959b-116">None</span><span class="sxs-lookup"><span data-stu-id="8959b-116">None</span></span> | <span data-ttu-id="8959b-117">删除**openShiftChangeRequest**对象。</span><span class="sxs-lookup"><span data-stu-id="8959b-117">Delete an **openShiftChangeRequest** object.</span></span> |
|[<span data-ttu-id="8959b-118">批准</span><span class="sxs-lookup"><span data-stu-id="8959b-118">Approve</span></span>](../api/openshiftchangerequest-approve.md)|<span data-ttu-id="8959b-119">None</span><span class="sxs-lookup"><span data-stu-id="8959b-119">None</span></span>|<span data-ttu-id="8959b-120">批准打开的班次更改请求。</span><span class="sxs-lookup"><span data-stu-id="8959b-120">Approve an open shift change request.</span></span>|
|[<span data-ttu-id="8959b-121">拒绝</span><span class="sxs-lookup"><span data-stu-id="8959b-121">Decline</span></span>](../api/openshiftchangerequest-decline.md)|<span data-ttu-id="8959b-122">None</span><span class="sxs-lookup"><span data-stu-id="8959b-122">None</span></span>| <span data-ttu-id="8959b-123">拒绝打开的班次更改请求。</span><span class="sxs-lookup"><span data-stu-id="8959b-123">Decline an open shift change request.</span></span>|

## <a name="properties"></a><span data-ttu-id="8959b-124">属性</span><span class="sxs-lookup"><span data-stu-id="8959b-124">Properties</span></span>

| <span data-ttu-id="8959b-125">属性</span><span class="sxs-lookup"><span data-stu-id="8959b-125">Property</span></span>     | <span data-ttu-id="8959b-126">类型</span><span class="sxs-lookup"><span data-stu-id="8959b-126">Type</span></span>        | <span data-ttu-id="8959b-127">说明</span><span class="sxs-lookup"><span data-stu-id="8959b-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8959b-128">openShiftId</span><span class="sxs-lookup"><span data-stu-id="8959b-128">openShiftId</span></span>|<span data-ttu-id="8959b-129">字符串</span><span class="sxs-lookup"><span data-stu-id="8959b-129">String</span></span>| <span data-ttu-id="8959b-130">打开的班次的 ID。</span><span class="sxs-lookup"><span data-stu-id="8959b-130">ID for the open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8959b-131">关系</span><span class="sxs-lookup"><span data-stu-id="8959b-131">Relationships</span></span>

<span data-ttu-id="8959b-132">无。</span><span class="sxs-lookup"><span data-stu-id="8959b-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8959b-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8959b-133">JSON representation</span></span>

<span data-ttu-id="8959b-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8959b-134">The following is a JSON representation of the resource.</span></span>

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
