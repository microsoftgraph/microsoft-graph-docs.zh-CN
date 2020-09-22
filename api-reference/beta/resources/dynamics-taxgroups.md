---
title: taxGroups 资源类型
description: Dynamics 365 Business Central 中的税务组对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 373e4785d19a7983f890ee3c3574533323829954
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027039"
---
# <a name="taxgroups-resource-type"></a><span data-ttu-id="ac651-103">taxGroups 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac651-103">taxGroups resource type</span></span>

<span data-ttu-id="ac651-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac651-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac651-105">代表 Dynamics 365 Business Central 中的 taxGroups 资源类型。</span><span class="sxs-lookup"><span data-stu-id="ac651-105">Represents a taxGroups resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="ac651-106">方法</span><span class="sxs-lookup"><span data-stu-id="ac651-106">Methods</span></span>
| <span data-ttu-id="ac651-107">方法</span><span class="sxs-lookup"><span data-stu-id="ac651-107">Method</span></span>       | <span data-ttu-id="ac651-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ac651-108">Return Type</span></span>  |<span data-ttu-id="ac651-109">说明</span><span class="sxs-lookup"><span data-stu-id="ac651-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ac651-110">获取 taxGroups</span><span class="sxs-lookup"><span data-stu-id="ac651-110">Get taxGroups</span></span>](../api/dynamics-taxgroups-get.md)|<span data-ttu-id="ac651-111">taxGroups</span><span class="sxs-lookup"><span data-stu-id="ac651-111">taxGroups</span></span>|<span data-ttu-id="ac651-112">获取税务组对象。</span><span class="sxs-lookup"><span data-stu-id="ac651-112">Gets a tax group object.</span></span>|
|[<span data-ttu-id="ac651-113">Post taxGroups</span><span class="sxs-lookup"><span data-stu-id="ac651-113">Post taxGroups</span></span>](../api/dynamics-create-taxgroups.md)|<span data-ttu-id="ac651-114">taxGroups</span><span class="sxs-lookup"><span data-stu-id="ac651-114">taxGroups</span></span>|<span data-ttu-id="ac651-115">创建税务组对象。</span><span class="sxs-lookup"><span data-stu-id="ac651-115">Creates a tax group object.</span></span>|
|[<span data-ttu-id="ac651-116">修补程序 taxGroups</span><span class="sxs-lookup"><span data-stu-id="ac651-116">Patch taxGroups</span></span>](../api/dynamics-taxgroups-update.md)|<span data-ttu-id="ac651-117">taxGroups</span><span class="sxs-lookup"><span data-stu-id="ac651-117">taxGroups</span></span>|<span data-ttu-id="ac651-118">更新税务组对象。</span><span class="sxs-lookup"><span data-stu-id="ac651-118">Updates a tax group object.</span></span>|
|[<span data-ttu-id="ac651-119">删除 taxGroups</span><span class="sxs-lookup"><span data-stu-id="ac651-119">Delete taxGroups</span></span>](../api/dynamics-taxgroups-delete.md)|<span data-ttu-id="ac651-120">无</span><span class="sxs-lookup"><span data-stu-id="ac651-120">none</span></span>|<span data-ttu-id="ac651-121">删除税务组对象。</span><span class="sxs-lookup"><span data-stu-id="ac651-121">Deletes a tax group object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac651-122">属性</span><span class="sxs-lookup"><span data-stu-id="ac651-122">Properties</span></span>
| <span data-ttu-id="ac651-123">属性</span><span class="sxs-lookup"><span data-stu-id="ac651-123">Property</span></span>     | <span data-ttu-id="ac651-124">类型</span><span class="sxs-lookup"><span data-stu-id="ac651-124">Type</span></span>   |<span data-ttu-id="ac651-125">说明</span><span class="sxs-lookup"><span data-stu-id="ac651-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac651-126">id</span><span class="sxs-lookup"><span data-stu-id="ac651-126">id</span></span>|<span data-ttu-id="ac651-127">GUID</span><span class="sxs-lookup"><span data-stu-id="ac651-127">GUID</span></span>|<span data-ttu-id="ac651-128">TaxGroup 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="ac651-128">The unique ID of the taxGroup.</span></span> <span data-ttu-id="ac651-129">只读。</span><span class="sxs-lookup"><span data-stu-id="ac651-129">Read-Only.</span></span>|
|<span data-ttu-id="ac651-130">code</span><span class="sxs-lookup"><span data-stu-id="ac651-130">code</span></span>|<span data-ttu-id="ac651-131">string</span><span class="sxs-lookup"><span data-stu-id="ac651-131">string</span></span>|<span data-ttu-id="ac651-132">指定税务组。</span><span class="sxs-lookup"><span data-stu-id="ac651-132">Specifies the tax group.</span></span>|
|<span data-ttu-id="ac651-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ac651-133">displayName</span></span>|<span data-ttu-id="ac651-134">string</span><span class="sxs-lookup"><span data-stu-id="ac651-134">string</span></span>|<span data-ttu-id="ac651-135">指定税务组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ac651-135">Specifies the tax group display name.</span></span>|
|<span data-ttu-id="ac651-136">taxType</span><span class="sxs-lookup"><span data-stu-id="ac651-136">taxType</span></span>|<span data-ttu-id="ac651-137">string</span><span class="sxs-lookup"><span data-stu-id="ac651-137">string</span></span>|<span data-ttu-id="ac651-138">指定组的税金类型。</span><span class="sxs-lookup"><span data-stu-id="ac651-138">Specifies the tax type for the group.</span></span>|
|<span data-ttu-id="ac651-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac651-139">lastModifiedDateTime</span></span>|<span data-ttu-id="ac651-140">datetime</span><span class="sxs-lookup"><span data-stu-id="ac651-140">datetime</span></span>|<span data-ttu-id="ac651-141">税组的最后修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="ac651-141">The last datetime the tax group was modified.</span></span> <span data-ttu-id="ac651-142">只读。</span><span class="sxs-lookup"><span data-stu-id="ac651-142">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="ac651-143">关系</span><span class="sxs-lookup"><span data-stu-id="ac651-143">Relationships</span></span>
<span data-ttu-id="ac651-144">无</span><span class="sxs-lookup"><span data-stu-id="ac651-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac651-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac651-145">JSON representation</span></span>

<span data-ttu-id="ac651-146">下面是 taxGroup 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac651-146">Here is a JSON representation of the taxGroup.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```




