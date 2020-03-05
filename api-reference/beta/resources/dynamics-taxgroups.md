---
title: taxGroups 资源类型
description: Dynamics 365 Business Central 中的税务组对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 3c8f244b9c3601aaeb315b09bb51d21275a63f6f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503255"
---
# <a name="taxgroups-resource-type"></a><span data-ttu-id="b8dd6-103">taxGroups 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8dd6-103">taxGroups resource type</span></span>

<span data-ttu-id="b8dd6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b8dd6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8dd6-105">代表 Dynamics 365 Business Central 中的 taxGroups 资源类型。</span><span class="sxs-lookup"><span data-stu-id="b8dd6-105">Represents a taxGroups resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="b8dd6-106">方法</span><span class="sxs-lookup"><span data-stu-id="b8dd6-106">Methods</span></span>
| <span data-ttu-id="b8dd6-107">方法</span><span class="sxs-lookup"><span data-stu-id="b8dd6-107">Method</span></span>       | <span data-ttu-id="b8dd6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b8dd6-108">Return Type</span></span>  |<span data-ttu-id="b8dd6-109">说明</span><span class="sxs-lookup"><span data-stu-id="b8dd6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b8dd6-110">获取 taxGroups</span><span class="sxs-lookup"><span data-stu-id="b8dd6-110">Get taxGroups</span></span>](../api/dynamics-taxgroups-get.md)|<span data-ttu-id="b8dd6-111">taxGroups</span><span class="sxs-lookup"><span data-stu-id="b8dd6-111">taxGroups</span></span>|<span data-ttu-id="b8dd6-112">获取税务组对象。</span><span class="sxs-lookup"><span data-stu-id="b8dd6-112">Gets a tax group object.</span></span>|
|[<span data-ttu-id="b8dd6-113">Post taxGroups</span><span class="sxs-lookup"><span data-stu-id="b8dd6-113">Post taxGroups</span></span>](../api/dynamics-create-taxgroups.md)|<span data-ttu-id="b8dd6-114">taxGroups</span><span class="sxs-lookup"><span data-stu-id="b8dd6-114">taxGroups</span></span>|<span data-ttu-id="b8dd6-115">创建税务组对象。</span><span class="sxs-lookup"><span data-stu-id="b8dd6-115">Creates a tax group object.</span></span>|
|[<span data-ttu-id="b8dd6-116">修补程序 taxGroups</span><span class="sxs-lookup"><span data-stu-id="b8dd6-116">Patch taxGroups</span></span>](../api/dynamics-taxgroups-update.md)|<span data-ttu-id="b8dd6-117">taxGroups</span><span class="sxs-lookup"><span data-stu-id="b8dd6-117">taxGroups</span></span>|<span data-ttu-id="b8dd6-118">更新税务组对象。</span><span class="sxs-lookup"><span data-stu-id="b8dd6-118">Updates a tax group object.</span></span>|
|[<span data-ttu-id="b8dd6-119">删除 taxGroups</span><span class="sxs-lookup"><span data-stu-id="b8dd6-119">Delete taxGroups</span></span>](../api/dynamics-taxgroups-delete.md)|<span data-ttu-id="b8dd6-120">无</span><span class="sxs-lookup"><span data-stu-id="b8dd6-120">none</span></span>|<span data-ttu-id="b8dd6-121">删除税务组对象。</span><span class="sxs-lookup"><span data-stu-id="b8dd6-121">Deletes a tax group object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8dd6-122">属性</span><span class="sxs-lookup"><span data-stu-id="b8dd6-122">Properties</span></span>
| <span data-ttu-id="b8dd6-123">属性</span><span class="sxs-lookup"><span data-stu-id="b8dd6-123">Property</span></span>     | <span data-ttu-id="b8dd6-124">类型</span><span class="sxs-lookup"><span data-stu-id="b8dd6-124">Type</span></span>   |<span data-ttu-id="b8dd6-125">说明</span><span class="sxs-lookup"><span data-stu-id="b8dd6-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8dd6-126">id</span><span class="sxs-lookup"><span data-stu-id="b8dd6-126">id</span></span>|<span data-ttu-id="b8dd6-127">GUID</span><span class="sxs-lookup"><span data-stu-id="b8dd6-127">GUID</span></span>|<span data-ttu-id="b8dd6-128">TaxGroup 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="b8dd6-128">The unique ID of the taxGroup.</span></span> <span data-ttu-id="b8dd6-129">只读。</span><span class="sxs-lookup"><span data-stu-id="b8dd6-129">Read-Only.</span></span>|
|<span data-ttu-id="b8dd6-130">code</span><span class="sxs-lookup"><span data-stu-id="b8dd6-130">code</span></span>|<span data-ttu-id="b8dd6-131">string</span><span class="sxs-lookup"><span data-stu-id="b8dd6-131">string</span></span>|<span data-ttu-id="b8dd6-132">指定税务组。</span><span class="sxs-lookup"><span data-stu-id="b8dd6-132">Specifies the tax group.</span></span>|
|<span data-ttu-id="b8dd6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b8dd6-133">displayName</span></span>|<span data-ttu-id="b8dd6-134">string</span><span class="sxs-lookup"><span data-stu-id="b8dd6-134">string</span></span>|<span data-ttu-id="b8dd6-135">指定税务组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b8dd6-135">Specifies the tax group display name.</span></span>|
|<span data-ttu-id="b8dd6-136">taxType</span><span class="sxs-lookup"><span data-stu-id="b8dd6-136">taxType</span></span>|<span data-ttu-id="b8dd6-137">string</span><span class="sxs-lookup"><span data-stu-id="b8dd6-137">string</span></span>|<span data-ttu-id="b8dd6-138">指定组的税金类型。</span><span class="sxs-lookup"><span data-stu-id="b8dd6-138">Specifies the tax type for the group.</span></span>|
|<span data-ttu-id="b8dd6-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8dd6-139">lastModifiedDateTime</span></span>|<span data-ttu-id="b8dd6-140">datetime</span><span class="sxs-lookup"><span data-stu-id="b8dd6-140">datetime</span></span>|<span data-ttu-id="b8dd6-141">税组的最后修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="b8dd6-141">The last datetime the tax group was modified.</span></span> <span data-ttu-id="b8dd6-142">只读。</span><span class="sxs-lookup"><span data-stu-id="b8dd6-142">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="b8dd6-143">关系</span><span class="sxs-lookup"><span data-stu-id="b8dd6-143">Relationships</span></span>
<span data-ttu-id="b8dd6-144">无</span><span class="sxs-lookup"><span data-stu-id="b8dd6-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8dd6-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8dd6-145">JSON representation</span></span>

<span data-ttu-id="b8dd6-146">下面是 taxGroup 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8dd6-146">Here is a JSON representation of the taxGroup.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```


