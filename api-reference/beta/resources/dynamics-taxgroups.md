---
title: taxGroups 资源类型
description: Dynamics 365 Business Central 中的税务组对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 378d8c1d773eacb3339eba35d5d60cc7ef5f2400
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006603"
---
# <a name="taxgroups-resource-type"></a><span data-ttu-id="9df5b-103">taxGroups 资源类型</span><span class="sxs-lookup"><span data-stu-id="9df5b-103">taxGroups resource type</span></span>
<span data-ttu-id="9df5b-104">代表 Dynamics 365 Business Central 中的 taxGroups 资源类型。</span><span class="sxs-lookup"><span data-stu-id="9df5b-104">Represents a taxGroups resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="9df5b-105">方法</span><span class="sxs-lookup"><span data-stu-id="9df5b-105">Methods</span></span>
| <span data-ttu-id="9df5b-106">方法</span><span class="sxs-lookup"><span data-stu-id="9df5b-106">Method</span></span>       | <span data-ttu-id="9df5b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="9df5b-107">Return Type</span></span>  |<span data-ttu-id="9df5b-108">说明</span><span class="sxs-lookup"><span data-stu-id="9df5b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9df5b-109">获取 taxGroups</span><span class="sxs-lookup"><span data-stu-id="9df5b-109">Get taxGroups</span></span>](../api/dynamics-taxgroups-get.md)|<span data-ttu-id="9df5b-110">taxGroups</span><span class="sxs-lookup"><span data-stu-id="9df5b-110">taxGroups</span></span>|<span data-ttu-id="9df5b-111">获取税务组对象。</span><span class="sxs-lookup"><span data-stu-id="9df5b-111">Gets a tax group object.</span></span>|
|[<span data-ttu-id="9df5b-112">Post taxGroups</span><span class="sxs-lookup"><span data-stu-id="9df5b-112">Post taxGroups</span></span>](../api/dynamics-create-taxgroups.md)|<span data-ttu-id="9df5b-113">taxGroups</span><span class="sxs-lookup"><span data-stu-id="9df5b-113">taxGroups</span></span>|<span data-ttu-id="9df5b-114">创建税务组对象。</span><span class="sxs-lookup"><span data-stu-id="9df5b-114">Creates a tax group object.</span></span>|
|[<span data-ttu-id="9df5b-115">修补程序 taxGroups</span><span class="sxs-lookup"><span data-stu-id="9df5b-115">Patch taxGroups</span></span>](../api/dynamics-taxgroups-update.md)|<span data-ttu-id="9df5b-116">taxGroups</span><span class="sxs-lookup"><span data-stu-id="9df5b-116">taxGroups</span></span>|<span data-ttu-id="9df5b-117">更新税务组对象。</span><span class="sxs-lookup"><span data-stu-id="9df5b-117">Updates a tax group object.</span></span>|
|[<span data-ttu-id="9df5b-118">删除 taxGroups</span><span class="sxs-lookup"><span data-stu-id="9df5b-118">Delete taxGroups</span></span>](../api/dynamics-taxgroups-delete.md)|<span data-ttu-id="9df5b-119">无</span><span class="sxs-lookup"><span data-stu-id="9df5b-119">none</span></span>|<span data-ttu-id="9df5b-120">删除税务组对象。</span><span class="sxs-lookup"><span data-stu-id="9df5b-120">Deletes a tax group object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9df5b-121">属性</span><span class="sxs-lookup"><span data-stu-id="9df5b-121">Properties</span></span>
| <span data-ttu-id="9df5b-122">属性</span><span class="sxs-lookup"><span data-stu-id="9df5b-122">Property</span></span>     | <span data-ttu-id="9df5b-123">类型</span><span class="sxs-lookup"><span data-stu-id="9df5b-123">Type</span></span>   |<span data-ttu-id="9df5b-124">说明</span><span class="sxs-lookup"><span data-stu-id="9df5b-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9df5b-125">id</span><span class="sxs-lookup"><span data-stu-id="9df5b-125">id</span></span>|<span data-ttu-id="9df5b-126">GUID</span><span class="sxs-lookup"><span data-stu-id="9df5b-126">GUID</span></span>|<span data-ttu-id="9df5b-127">TaxGroup 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="9df5b-127">The unique ID of the taxGroup.</span></span> <span data-ttu-id="9df5b-128">只读。</span><span class="sxs-lookup"><span data-stu-id="9df5b-128">Read-Only.</span></span>|
|<span data-ttu-id="9df5b-129">code</span><span class="sxs-lookup"><span data-stu-id="9df5b-129">code</span></span>|<span data-ttu-id="9df5b-130">string</span><span class="sxs-lookup"><span data-stu-id="9df5b-130">string</span></span>|<span data-ttu-id="9df5b-131">指定税务组。</span><span class="sxs-lookup"><span data-stu-id="9df5b-131">Specifies the tax group.</span></span>|
|<span data-ttu-id="9df5b-132">displayName</span><span class="sxs-lookup"><span data-stu-id="9df5b-132">displayName</span></span>|<span data-ttu-id="9df5b-133">string</span><span class="sxs-lookup"><span data-stu-id="9df5b-133">string</span></span>|<span data-ttu-id="9df5b-134">指定税务组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9df5b-134">Specifies the tax group display name.</span></span>|
|<span data-ttu-id="9df5b-135">taxType</span><span class="sxs-lookup"><span data-stu-id="9df5b-135">taxType</span></span>|<span data-ttu-id="9df5b-136">string</span><span class="sxs-lookup"><span data-stu-id="9df5b-136">string</span></span>|<span data-ttu-id="9df5b-137">指定组的税金类型。</span><span class="sxs-lookup"><span data-stu-id="9df5b-137">Specifies the tax type for the group.</span></span>|
|<span data-ttu-id="9df5b-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9df5b-138">lastModifiedDateTime</span></span>|<span data-ttu-id="9df5b-139">datetime</span><span class="sxs-lookup"><span data-stu-id="9df5b-139">datetime</span></span>|<span data-ttu-id="9df5b-140">税组的最后修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="9df5b-140">The last datetime the tax group was modified.</span></span> <span data-ttu-id="9df5b-141">只读。</span><span class="sxs-lookup"><span data-stu-id="9df5b-141">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="9df5b-142">关系</span><span class="sxs-lookup"><span data-stu-id="9df5b-142">Relationships</span></span>
<span data-ttu-id="9df5b-143">无</span><span class="sxs-lookup"><span data-stu-id="9df5b-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9df5b-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9df5b-144">JSON representation</span></span>

<span data-ttu-id="9df5b-145">下面是 taxGroup 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9df5b-145">Here is a JSON representation of the taxGroup.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```


