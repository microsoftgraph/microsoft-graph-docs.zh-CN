---
title: managedAppPolicy 资源类型
description: ManagedAppPolicy 资源表示特定于平台的策略的基类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b502364cdcc461601b8790955bb93710be336e24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030269"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="fd8bc-103">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd8bc-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="fd8bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd8bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd8bc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fd8bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd8bc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd8bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd8bc-107">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="fd8bc-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="fd8bc-108">方法</span><span class="sxs-lookup"><span data-stu-id="fd8bc-108">Methods</span></span>
|<span data-ttu-id="fd8bc-109">方法</span><span class="sxs-lookup"><span data-stu-id="fd8bc-109">Method</span></span>|<span data-ttu-id="fd8bc-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="fd8bc-110">Return Type</span></span>|<span data-ttu-id="fd8bc-111">说明</span><span class="sxs-lookup"><span data-stu-id="fd8bc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fd8bc-112">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="fd8bc-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="fd8bc-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd8bc-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="fd8bc-114">列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fd8bc-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="fd8bc-115">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="fd8bc-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="fd8bc-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="fd8bc-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="fd8bc-117">读取 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fd8bc-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="fd8bc-118">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="fd8bc-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="fd8bc-119">无</span><span class="sxs-lookup"><span data-stu-id="fd8bc-119">None</span></span>|<span data-ttu-id="fd8bc-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fd8bc-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fd8bc-121">属性</span><span class="sxs-lookup"><span data-stu-id="fd8bc-121">Properties</span></span>
|<span data-ttu-id="fd8bc-122">属性</span><span class="sxs-lookup"><span data-stu-id="fd8bc-122">Property</span></span>|<span data-ttu-id="fd8bc-123">类型</span><span class="sxs-lookup"><span data-stu-id="fd8bc-123">Type</span></span>|<span data-ttu-id="fd8bc-124">说明</span><span class="sxs-lookup"><span data-stu-id="fd8bc-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd8bc-125">displayName</span><span class="sxs-lookup"><span data-stu-id="fd8bc-125">displayName</span></span>|<span data-ttu-id="fd8bc-126">String</span><span class="sxs-lookup"><span data-stu-id="fd8bc-126">String</span></span>|<span data-ttu-id="fd8bc-127">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="fd8bc-127">Policy display name.</span></span>|
|<span data-ttu-id="fd8bc-128">description</span><span class="sxs-lookup"><span data-stu-id="fd8bc-128">description</span></span>|<span data-ttu-id="fd8bc-129">String</span><span class="sxs-lookup"><span data-stu-id="fd8bc-129">String</span></span>|<span data-ttu-id="fd8bc-130">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="fd8bc-130">The policy's description.</span></span>|
|<span data-ttu-id="fd8bc-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd8bc-131">createdDateTime</span></span>|<span data-ttu-id="fd8bc-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd8bc-132">DateTimeOffset</span></span>|<span data-ttu-id="fd8bc-133">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fd8bc-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="fd8bc-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd8bc-134">lastModifiedDateTime</span></span>|<span data-ttu-id="fd8bc-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd8bc-135">DateTimeOffset</span></span>|<span data-ttu-id="fd8bc-136">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="fd8bc-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="fd8bc-137">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fd8bc-137">roleScopeTagIds</span></span>|<span data-ttu-id="fd8bc-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="fd8bc-138">String collection</span></span>|<span data-ttu-id="fd8bc-139">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="fd8bc-139">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="fd8bc-140">id</span><span class="sxs-lookup"><span data-stu-id="fd8bc-140">id</span></span>|<span data-ttu-id="fd8bc-141">String</span><span class="sxs-lookup"><span data-stu-id="fd8bc-141">String</span></span>|<span data-ttu-id="fd8bc-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fd8bc-142">Key of the entity.</span></span>|
|<span data-ttu-id="fd8bc-143">version</span><span class="sxs-lookup"><span data-stu-id="fd8bc-143">version</span></span>|<span data-ttu-id="fd8bc-144">String</span><span class="sxs-lookup"><span data-stu-id="fd8bc-144">String</span></span>|<span data-ttu-id="fd8bc-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="fd8bc-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd8bc-146">关系</span><span class="sxs-lookup"><span data-stu-id="fd8bc-146">Relationships</span></span>
<span data-ttu-id="fd8bc-147">无</span><span class="sxs-lookup"><span data-stu-id="fd8bc-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd8bc-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd8bc-148">JSON Representation</span></span>
<span data-ttu-id="fd8bc-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd8bc-149">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String"
}
```






