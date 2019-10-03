---
title: managedAppPolicy 资源类型
description: ManagedAppPolicy 资源表示特定于平台的策略的基类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d791126a5e059c80d4bc6da76597dd563e1c723a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367824"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="70cf0-103">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="70cf0-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="70cf0-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="70cf0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70cf0-105">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="70cf0-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="70cf0-106">方法</span><span class="sxs-lookup"><span data-stu-id="70cf0-106">Methods</span></span>
|<span data-ttu-id="70cf0-107">方法</span><span class="sxs-lookup"><span data-stu-id="70cf0-107">Method</span></span>|<span data-ttu-id="70cf0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="70cf0-108">Return Type</span></span>|<span data-ttu-id="70cf0-109">说明</span><span class="sxs-lookup"><span data-stu-id="70cf0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="70cf0-110">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="70cf0-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="70cf0-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="70cf0-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="70cf0-112">列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="70cf0-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="70cf0-113">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="70cf0-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="70cf0-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="70cf0-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="70cf0-115">读取 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="70cf0-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="70cf0-116">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="70cf0-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="70cf0-117">无</span><span class="sxs-lookup"><span data-stu-id="70cf0-117">None</span></span>|<span data-ttu-id="70cf0-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="70cf0-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="70cf0-119">属性</span><span class="sxs-lookup"><span data-stu-id="70cf0-119">Properties</span></span>
|<span data-ttu-id="70cf0-120">属性</span><span class="sxs-lookup"><span data-stu-id="70cf0-120">Property</span></span>|<span data-ttu-id="70cf0-121">类型</span><span class="sxs-lookup"><span data-stu-id="70cf0-121">Type</span></span>|<span data-ttu-id="70cf0-122">说明</span><span class="sxs-lookup"><span data-stu-id="70cf0-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70cf0-123">displayName</span><span class="sxs-lookup"><span data-stu-id="70cf0-123">displayName</span></span>|<span data-ttu-id="70cf0-124">字符串</span><span class="sxs-lookup"><span data-stu-id="70cf0-124">String</span></span>|<span data-ttu-id="70cf0-125">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="70cf0-125">Policy display name.</span></span>|
|<span data-ttu-id="70cf0-126">说明</span><span class="sxs-lookup"><span data-stu-id="70cf0-126">description</span></span>|<span data-ttu-id="70cf0-127">String</span><span class="sxs-lookup"><span data-stu-id="70cf0-127">String</span></span>|<span data-ttu-id="70cf0-128">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="70cf0-128">The policy's description.</span></span>|
|<span data-ttu-id="70cf0-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70cf0-129">createdDateTime</span></span>|<span data-ttu-id="70cf0-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70cf0-130">DateTimeOffset</span></span>|<span data-ttu-id="70cf0-131">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="70cf0-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="70cf0-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70cf0-132">lastModifiedDateTime</span></span>|<span data-ttu-id="70cf0-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70cf0-133">DateTimeOffset</span></span>|<span data-ttu-id="70cf0-134">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="70cf0-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="70cf0-135">id</span><span class="sxs-lookup"><span data-stu-id="70cf0-135">id</span></span>|<span data-ttu-id="70cf0-136">字符串</span><span class="sxs-lookup"><span data-stu-id="70cf0-136">String</span></span>|<span data-ttu-id="70cf0-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="70cf0-137">Key of the entity.</span></span>|
|<span data-ttu-id="70cf0-138">version</span><span class="sxs-lookup"><span data-stu-id="70cf0-138">version</span></span>|<span data-ttu-id="70cf0-139">String</span><span class="sxs-lookup"><span data-stu-id="70cf0-139">String</span></span>|<span data-ttu-id="70cf0-140">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="70cf0-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70cf0-141">关系</span><span class="sxs-lookup"><span data-stu-id="70cf0-141">Relationships</span></span>
<span data-ttu-id="70cf0-142">无</span><span class="sxs-lookup"><span data-stu-id="70cf0-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="70cf0-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70cf0-143">JSON Representation</span></span>
<span data-ttu-id="70cf0-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70cf0-144">Here is a JSON representation of the resource.</span></span>
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




