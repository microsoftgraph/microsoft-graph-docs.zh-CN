---
title: managedAppPolicy 资源类型
description: ManagedAppPolicy 资源表示特定于平台的策略的基类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2615d1331c024c1a04bc7db618e36966cc5bcdff
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251165"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="c95f4-103">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="c95f4-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="c95f4-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c95f4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c95f4-105">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="c95f4-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="c95f4-106">方法</span><span class="sxs-lookup"><span data-stu-id="c95f4-106">Methods</span></span>
|<span data-ttu-id="c95f4-107">方法</span><span class="sxs-lookup"><span data-stu-id="c95f4-107">Method</span></span>|<span data-ttu-id="c95f4-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c95f4-108">Return Type</span></span>|<span data-ttu-id="c95f4-109">说明</span><span class="sxs-lookup"><span data-stu-id="c95f4-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c95f4-110">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="c95f4-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="c95f4-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c95f4-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="c95f4-112">列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c95f4-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="c95f4-113">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="c95f4-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="c95f4-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="c95f4-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="c95f4-115">读取 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c95f4-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="c95f4-116">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="c95f4-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="c95f4-117">无</span><span class="sxs-lookup"><span data-stu-id="c95f4-117">None</span></span>|<span data-ttu-id="c95f4-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c95f4-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c95f4-119">属性</span><span class="sxs-lookup"><span data-stu-id="c95f4-119">Properties</span></span>
|<span data-ttu-id="c95f4-120">属性</span><span class="sxs-lookup"><span data-stu-id="c95f4-120">Property</span></span>|<span data-ttu-id="c95f4-121">类型</span><span class="sxs-lookup"><span data-stu-id="c95f4-121">Type</span></span>|<span data-ttu-id="c95f4-122">说明</span><span class="sxs-lookup"><span data-stu-id="c95f4-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c95f4-123">displayName</span><span class="sxs-lookup"><span data-stu-id="c95f4-123">displayName</span></span>|<span data-ttu-id="c95f4-124">String</span><span class="sxs-lookup"><span data-stu-id="c95f4-124">String</span></span>|<span data-ttu-id="c95f4-125">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="c95f4-125">Policy display name.</span></span>|
|<span data-ttu-id="c95f4-126">description</span><span class="sxs-lookup"><span data-stu-id="c95f4-126">description</span></span>|<span data-ttu-id="c95f4-127">String</span><span class="sxs-lookup"><span data-stu-id="c95f4-127">String</span></span>|<span data-ttu-id="c95f4-128">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="c95f4-128">The policy's description.</span></span>|
|<span data-ttu-id="c95f4-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c95f4-129">createdDateTime</span></span>|<span data-ttu-id="c95f4-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c95f4-130">DateTimeOffset</span></span>|<span data-ttu-id="c95f4-131">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c95f4-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="c95f4-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c95f4-132">lastModifiedDateTime</span></span>|<span data-ttu-id="c95f4-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c95f4-133">DateTimeOffset</span></span>|<span data-ttu-id="c95f4-134">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="c95f4-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="c95f4-135">id</span><span class="sxs-lookup"><span data-stu-id="c95f4-135">id</span></span>|<span data-ttu-id="c95f4-136">字符串</span><span class="sxs-lookup"><span data-stu-id="c95f4-136">String</span></span>|<span data-ttu-id="c95f4-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c95f4-137">Key of the entity.</span></span>|
|<span data-ttu-id="c95f4-138">version</span><span class="sxs-lookup"><span data-stu-id="c95f4-138">version</span></span>|<span data-ttu-id="c95f4-139">String</span><span class="sxs-lookup"><span data-stu-id="c95f4-139">String</span></span>|<span data-ttu-id="c95f4-140">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="c95f4-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c95f4-141">关系</span><span class="sxs-lookup"><span data-stu-id="c95f4-141">Relationships</span></span>
<span data-ttu-id="c95f4-142">无</span><span class="sxs-lookup"><span data-stu-id="c95f4-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c95f4-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c95f4-143">JSON Representation</span></span>
<span data-ttu-id="c95f4-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c95f4-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String"
}
```



