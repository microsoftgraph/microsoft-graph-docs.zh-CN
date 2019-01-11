---
title: targetResource 资源类型
description: 指示与审核活动关联的目标资源类型的集合。 每个目标资源类型将继承此资源从下面概括的属性。
localization_priority: Normal
ms.openlocfilehash: f86cfe45870292dae93327859c32d38aa2b252fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828677"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="f1f2a-104">targetResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1f2a-104">targetResource resource type</span></span>
<span data-ttu-id="f1f2a-105">指示与审核活动关联的目标资源类型的集合。</span><span class="sxs-lookup"><span data-stu-id="f1f2a-105">Indicates a collection of  target resource types associated with the audit activity.</span></span> <span data-ttu-id="f1f2a-106">每个目标资源类型将继承此资源从下面概括的属性。</span><span class="sxs-lookup"><span data-stu-id="f1f2a-106">Each target resource type will inherit the properties outlined below from this resource.</span></span>


## <a name="properties"></a><span data-ttu-id="f1f2a-107">属性</span><span class="sxs-lookup"><span data-stu-id="f1f2a-107">Properties</span></span>
| <span data-ttu-id="f1f2a-108">属性</span><span class="sxs-lookup"><span data-stu-id="f1f2a-108">Property</span></span>     | <span data-ttu-id="f1f2a-109">类型</span><span class="sxs-lookup"><span data-stu-id="f1f2a-109">Type</span></span>   |<span data-ttu-id="f1f2a-110">说明</span><span class="sxs-lookup"><span data-stu-id="f1f2a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1f2a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f1f2a-111">displayName</span></span>|<span data-ttu-id="f1f2a-112">字符串</span><span class="sxs-lookup"><span data-stu-id="f1f2a-112">String</span></span>|<span data-ttu-id="f1f2a-113">指示下以下目标资源类型列出的资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f1f2a-113">Indicates the display name of the resources outlined under Target Resource Types below.</span></span>|
|<span data-ttu-id="f1f2a-114">id</span><span class="sxs-lookup"><span data-stu-id="f1f2a-114">id</span></span>|<span data-ttu-id="f1f2a-115">字符串</span><span class="sxs-lookup"><span data-stu-id="f1f2a-115">String</span></span>|<span data-ttu-id="f1f2a-116">指示的资源的唯一 Id (例如： UserId，AppId，RoleId。)。</span><span class="sxs-lookup"><span data-stu-id="f1f2a-116">Indicates the Unique Id of the resource (For example: UserId, AppId, RoleId.).</span></span>|
|<span data-ttu-id="f1f2a-117">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="f1f2a-117">modifiedProperties</span></span>|<span data-ttu-id="f1f2a-118">[modifiedProperty](modifiedproperty.md)集合</span><span class="sxs-lookup"><span data-stu-id="f1f2a-118">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="f1f2a-119">指示名称、 旧值和更改每个属性的新值。</span><span class="sxs-lookup"><span data-stu-id="f1f2a-119">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="f1f2a-120">这仅适用于任何"更新"活动</span><span class="sxs-lookup"><span data-stu-id="f1f2a-120">This is applicable for any "Update" activities</span></span>|

### <a name="target-resource-types"></a><span data-ttu-id="f1f2a-121">目标资源类型</span><span class="sxs-lookup"><span data-stu-id="f1f2a-121">Target Resource Types</span></span>

<span data-ttu-id="f1f2a-122">目标资源类型会有所不同，根据基础资源：</span><span class="sxs-lookup"><span data-stu-id="f1f2a-122">The target resource type varies according to the underlying resource:</span></span>

|<span data-ttu-id="f1f2a-123">资源名称</span><span class="sxs-lookup"><span data-stu-id="f1f2a-123">Resource Name</span></span>| <span data-ttu-id="f1f2a-124">参考</span><span class="sxs-lookup"><span data-stu-id="f1f2a-124">Reference</span></span>|
|-------------|----------|
<span data-ttu-id="f1f2a-125">Device</span><span class="sxs-lookup"><span data-stu-id="f1f2a-125">Device</span></span>|[<span data-ttu-id="f1f2a-126">targetResourceDevice</span><span class="sxs-lookup"><span data-stu-id="f1f2a-126">targetResourceDevice</span></span>](targetresourcedevice.md)
<span data-ttu-id="f1f2a-127">目录</span><span class="sxs-lookup"><span data-stu-id="f1f2a-127">Directory</span></span>|<span data-ttu-id="f1f2a-128">[targetResourceDirectory](targetresourcedirectory.md]</span><span class="sxs-lookup"><span data-stu-id="f1f2a-128">[targetResourceDirectory](targetresourcedirectory.md]</span></span>
<span data-ttu-id="f1f2a-129">Group</span><span class="sxs-lookup"><span data-stu-id="f1f2a-129">Group</span></span>|[<span data-ttu-id="f1f2a-130">targetResourceGroup</span><span class="sxs-lookup"><span data-stu-id="f1f2a-130">targetResourceGroup</span></span>](targetresourcegroup.md)
<span data-ttu-id="f1f2a-131">策略</span><span class="sxs-lookup"><span data-stu-id="f1f2a-131">Policy</span></span>|[<span data-ttu-id="f1f2a-132">targetResourcePolicy</span><span class="sxs-lookup"><span data-stu-id="f1f2a-132">targetResourcePolicy</span></span>](targetresourcepolicy.md)
<span data-ttu-id="f1f2a-133">Role</span><span class="sxs-lookup"><span data-stu-id="f1f2a-133">Role</span></span>|[<span data-ttu-id="f1f2a-134">targetResourceRole</span><span class="sxs-lookup"><span data-stu-id="f1f2a-134">targetResourceRole</span></span>](targetresourcerole.md)
<span data-ttu-id="f1f2a-135">服务主体</span><span class="sxs-lookup"><span data-stu-id="f1f2a-135">Service Principal</span></span>|[<span data-ttu-id="f1f2a-136">targetResourceServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="f1f2a-136">targetResourceServicePrincipal</span></span>](targetresourceserviceprincipal.md)
<span data-ttu-id="f1f2a-137">用户</span><span class="sxs-lookup"><span data-stu-id="f1f2a-137">User</span></span>|[<span data-ttu-id="f1f2a-138">targetResourceUser</span><span class="sxs-lookup"><span data-stu-id="f1f2a-138">targetResourceUser</span></span>](targetresourceuser.md)
<span data-ttu-id="f1f2a-139">其他</span><span class="sxs-lookup"><span data-stu-id="f1f2a-139">Other</span></span>|[<span data-ttu-id="f1f2a-140">targetResourceOther</span><span class="sxs-lookup"><span data-stu-id="f1f2a-140">targetResourceOther</span></span>](targetresourceother.md)

## <a name="json-representation"></a><span data-ttu-id="f1f2a-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1f2a-141">JSON representation</span></span>

<span data-ttu-id="f1f2a-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1f2a-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
