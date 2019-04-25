---
title: taxGroups 资源类型
description: Dynamics 365 Business Central 中的税务组对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: bdfbec8f5373637924262388dab0e9c74c363af9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543124"
---
# <a name="taxgroups-resource-type"></a><span data-ttu-id="6ea69-103">taxGroups 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ea69-103">taxGroups resource type</span></span>
<span data-ttu-id="6ea69-104">代表 Dynamics 365 Business Central 中的 taxGroups 资源类型。</span><span class="sxs-lookup"><span data-stu-id="6ea69-104">Represents a taxGroups resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="6ea69-105">方法</span><span class="sxs-lookup"><span data-stu-id="6ea69-105">Methods</span></span>
| <span data-ttu-id="6ea69-106">方法</span><span class="sxs-lookup"><span data-stu-id="6ea69-106">Method</span></span>       | <span data-ttu-id="6ea69-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="6ea69-107">Return Type</span></span>  |<span data-ttu-id="6ea69-108">说明</span><span class="sxs-lookup"><span data-stu-id="6ea69-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6ea69-109">获取 taxGroups</span><span class="sxs-lookup"><span data-stu-id="6ea69-109">Get taxGroups</span></span>](../api/dynamics-taxgroups-get.md)|<span data-ttu-id="6ea69-110">taxGroups</span><span class="sxs-lookup"><span data-stu-id="6ea69-110">taxGroups</span></span>|<span data-ttu-id="6ea69-111">获取税务组对象。</span><span class="sxs-lookup"><span data-stu-id="6ea69-111">Gets a tax group object.</span></span>|
|[<span data-ttu-id="6ea69-112">Post taxGroups</span><span class="sxs-lookup"><span data-stu-id="6ea69-112">Post taxGroups</span></span>](../api/dynamics-create-taxgroups.md)|<span data-ttu-id="6ea69-113">taxGroups</span><span class="sxs-lookup"><span data-stu-id="6ea69-113">taxGroups</span></span>|<span data-ttu-id="6ea69-114">创建税务组对象。</span><span class="sxs-lookup"><span data-stu-id="6ea69-114">Creates a tax group object.</span></span>|
|[<span data-ttu-id="6ea69-115">修补程序 taxGroups</span><span class="sxs-lookup"><span data-stu-id="6ea69-115">Patch taxGroups</span></span>](../api/dynamics-taxgroups-update.md)|<span data-ttu-id="6ea69-116">taxGroups</span><span class="sxs-lookup"><span data-stu-id="6ea69-116">taxGroups</span></span>|<span data-ttu-id="6ea69-117">更新税务组对象。</span><span class="sxs-lookup"><span data-stu-id="6ea69-117">Updates a tax group object.</span></span>|
|[<span data-ttu-id="6ea69-118">删除 taxGroups</span><span class="sxs-lookup"><span data-stu-id="6ea69-118">Delete taxGroups</span></span>](../api/dynamics-taxgroups-delete.md)|<span data-ttu-id="6ea69-119">无</span><span class="sxs-lookup"><span data-stu-id="6ea69-119">none</span></span>|<span data-ttu-id="6ea69-120">删除税务组对象。</span><span class="sxs-lookup"><span data-stu-id="6ea69-120">Deletes a tax group object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6ea69-121">属性</span><span class="sxs-lookup"><span data-stu-id="6ea69-121">Properties</span></span>
| <span data-ttu-id="6ea69-122">属性</span><span class="sxs-lookup"><span data-stu-id="6ea69-122">Property</span></span>     | <span data-ttu-id="6ea69-123">类型</span><span class="sxs-lookup"><span data-stu-id="6ea69-123">Type</span></span>   |<span data-ttu-id="6ea69-124">说明</span><span class="sxs-lookup"><span data-stu-id="6ea69-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ea69-125">id</span><span class="sxs-lookup"><span data-stu-id="6ea69-125">id</span></span>|<span data-ttu-id="6ea69-126">GUID</span><span class="sxs-lookup"><span data-stu-id="6ea69-126">GUID</span></span>|<span data-ttu-id="6ea69-127">taxGroup 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="6ea69-127">The unique ID of the taxGroup.</span></span> <span data-ttu-id="6ea69-128">只读。</span><span class="sxs-lookup"><span data-stu-id="6ea69-128">Read-Only.</span></span>|
|<span data-ttu-id="6ea69-129">code</span><span class="sxs-lookup"><span data-stu-id="6ea69-129">code</span></span>|<span data-ttu-id="6ea69-130">string</span><span class="sxs-lookup"><span data-stu-id="6ea69-130">string</span></span>|<span data-ttu-id="6ea69-131">指定税务组。</span><span class="sxs-lookup"><span data-stu-id="6ea69-131">Specifies the tax group.</span></span>|
|<span data-ttu-id="6ea69-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6ea69-132">displayName</span></span>|<span data-ttu-id="6ea69-133">string</span><span class="sxs-lookup"><span data-stu-id="6ea69-133">string</span></span>|<span data-ttu-id="6ea69-134">指定税务组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6ea69-134">Specifies the tax group display name.</span></span>|
|<span data-ttu-id="6ea69-135">taxType</span><span class="sxs-lookup"><span data-stu-id="6ea69-135">taxType</span></span>|<span data-ttu-id="6ea69-136">string</span><span class="sxs-lookup"><span data-stu-id="6ea69-136">string</span></span>|<span data-ttu-id="6ea69-137">指定组的税金类型。</span><span class="sxs-lookup"><span data-stu-id="6ea69-137">Specifies the tax type for the group.</span></span>|
|<span data-ttu-id="6ea69-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ea69-138">lastModifiedDateTime</span></span>|<span data-ttu-id="6ea69-139">datetime</span><span class="sxs-lookup"><span data-stu-id="6ea69-139">datetime</span></span>|<span data-ttu-id="6ea69-140">税组的最后修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="6ea69-140">The last datetime the tax group was modified.</span></span> <span data-ttu-id="6ea69-141">只读。</span><span class="sxs-lookup"><span data-stu-id="6ea69-141">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="6ea69-142">关系</span><span class="sxs-lookup"><span data-stu-id="6ea69-142">Relationships</span></span>
<span data-ttu-id="6ea69-143">无</span><span class="sxs-lookup"><span data-stu-id="6ea69-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ea69-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ea69-144">JSON representation</span></span>

<span data-ttu-id="6ea69-145">下面是 taxGroup 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ea69-145">Here is a JSON representation of the taxGroup.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```


