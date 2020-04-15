---
title: managedAppPolicy 资源类型
description: ManagedAppPolicy 资源表示特定于平台的策略的基类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f0e26ea51641bf2a291802d391bfaace18da31f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468516"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="894b3-103">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="894b3-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="894b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="894b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="894b3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="894b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="894b3-106">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="894b3-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="894b3-107">方法</span><span class="sxs-lookup"><span data-stu-id="894b3-107">Methods</span></span>
|<span data-ttu-id="894b3-108">方法</span><span class="sxs-lookup"><span data-stu-id="894b3-108">Method</span></span>|<span data-ttu-id="894b3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="894b3-109">Return Type</span></span>|<span data-ttu-id="894b3-110">说明</span><span class="sxs-lookup"><span data-stu-id="894b3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="894b3-111">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="894b3-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="894b3-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="894b3-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="894b3-113">列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="894b3-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="894b3-114">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="894b3-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="894b3-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="894b3-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="894b3-116">读取 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="894b3-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="894b3-117">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="894b3-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="894b3-118">无</span><span class="sxs-lookup"><span data-stu-id="894b3-118">None</span></span>|<span data-ttu-id="894b3-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="894b3-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="894b3-120">属性</span><span class="sxs-lookup"><span data-stu-id="894b3-120">Properties</span></span>
|<span data-ttu-id="894b3-121">属性</span><span class="sxs-lookup"><span data-stu-id="894b3-121">Property</span></span>|<span data-ttu-id="894b3-122">类型</span><span class="sxs-lookup"><span data-stu-id="894b3-122">Type</span></span>|<span data-ttu-id="894b3-123">说明</span><span class="sxs-lookup"><span data-stu-id="894b3-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="894b3-124">displayName</span><span class="sxs-lookup"><span data-stu-id="894b3-124">displayName</span></span>|<span data-ttu-id="894b3-125">字符串</span><span class="sxs-lookup"><span data-stu-id="894b3-125">String</span></span>|<span data-ttu-id="894b3-126">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="894b3-126">Policy display name.</span></span>|
|<span data-ttu-id="894b3-127">description</span><span class="sxs-lookup"><span data-stu-id="894b3-127">description</span></span>|<span data-ttu-id="894b3-128">String</span><span class="sxs-lookup"><span data-stu-id="894b3-128">String</span></span>|<span data-ttu-id="894b3-129">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="894b3-129">The policy's description.</span></span>|
|<span data-ttu-id="894b3-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="894b3-130">createdDateTime</span></span>|<span data-ttu-id="894b3-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="894b3-131">DateTimeOffset</span></span>|<span data-ttu-id="894b3-132">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="894b3-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="894b3-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="894b3-133">lastModifiedDateTime</span></span>|<span data-ttu-id="894b3-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="894b3-134">DateTimeOffset</span></span>|<span data-ttu-id="894b3-135">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="894b3-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="894b3-136">id</span><span class="sxs-lookup"><span data-stu-id="894b3-136">id</span></span>|<span data-ttu-id="894b3-137">字符串</span><span class="sxs-lookup"><span data-stu-id="894b3-137">String</span></span>|<span data-ttu-id="894b3-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="894b3-138">Key of the entity.</span></span>|
|<span data-ttu-id="894b3-139">version</span><span class="sxs-lookup"><span data-stu-id="894b3-139">version</span></span>|<span data-ttu-id="894b3-140">String</span><span class="sxs-lookup"><span data-stu-id="894b3-140">String</span></span>|<span data-ttu-id="894b3-141">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="894b3-141">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="894b3-142">关系</span><span class="sxs-lookup"><span data-stu-id="894b3-142">Relationships</span></span>
<span data-ttu-id="894b3-143">无</span><span class="sxs-lookup"><span data-stu-id="894b3-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="894b3-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="894b3-144">JSON Representation</span></span>
<span data-ttu-id="894b3-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="894b3-145">Here is a JSON representation of the resource.</span></span>
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







