---
title: managedAppPolicy 资源类型
description: ManagedAppPolicy 资源表示特定于平台的策略的基类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 610012b216a0fe924af3cd4f08fb3928e504454b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573814"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="eed2a-103">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="eed2a-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="eed2a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eed2a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eed2a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eed2a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eed2a-106">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="eed2a-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="eed2a-107">方法</span><span class="sxs-lookup"><span data-stu-id="eed2a-107">Methods</span></span>
|<span data-ttu-id="eed2a-108">方法</span><span class="sxs-lookup"><span data-stu-id="eed2a-108">Method</span></span>|<span data-ttu-id="eed2a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="eed2a-109">Return Type</span></span>|<span data-ttu-id="eed2a-110">说明</span><span class="sxs-lookup"><span data-stu-id="eed2a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eed2a-111">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="eed2a-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="eed2a-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eed2a-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="eed2a-113">列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eed2a-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="eed2a-114">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="eed2a-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="eed2a-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="eed2a-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="eed2a-116">读取 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eed2a-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="eed2a-117">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="eed2a-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="eed2a-118">无</span><span class="sxs-lookup"><span data-stu-id="eed2a-118">None</span></span>|<span data-ttu-id="eed2a-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="eed2a-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="eed2a-120">属性</span><span class="sxs-lookup"><span data-stu-id="eed2a-120">Properties</span></span>
|<span data-ttu-id="eed2a-121">属性</span><span class="sxs-lookup"><span data-stu-id="eed2a-121">Property</span></span>|<span data-ttu-id="eed2a-122">类型</span><span class="sxs-lookup"><span data-stu-id="eed2a-122">Type</span></span>|<span data-ttu-id="eed2a-123">说明</span><span class="sxs-lookup"><span data-stu-id="eed2a-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eed2a-124">displayName</span><span class="sxs-lookup"><span data-stu-id="eed2a-124">displayName</span></span>|<span data-ttu-id="eed2a-125">字符串</span><span class="sxs-lookup"><span data-stu-id="eed2a-125">String</span></span>|<span data-ttu-id="eed2a-126">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="eed2a-126">Policy display name.</span></span>|
|<span data-ttu-id="eed2a-127">说明</span><span class="sxs-lookup"><span data-stu-id="eed2a-127">description</span></span>|<span data-ttu-id="eed2a-128">String</span><span class="sxs-lookup"><span data-stu-id="eed2a-128">String</span></span>|<span data-ttu-id="eed2a-129">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="eed2a-129">The policy's description.</span></span>|
|<span data-ttu-id="eed2a-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eed2a-130">createdDateTime</span></span>|<span data-ttu-id="eed2a-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eed2a-131">DateTimeOffset</span></span>|<span data-ttu-id="eed2a-132">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="eed2a-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="eed2a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eed2a-133">lastModifiedDateTime</span></span>|<span data-ttu-id="eed2a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eed2a-134">DateTimeOffset</span></span>|<span data-ttu-id="eed2a-135">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="eed2a-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="eed2a-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eed2a-136">roleScopeTagIds</span></span>|<span data-ttu-id="eed2a-137">String collection</span><span class="sxs-lookup"><span data-stu-id="eed2a-137">String collection</span></span>|<span data-ttu-id="eed2a-138">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="eed2a-138">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="eed2a-139">id</span><span class="sxs-lookup"><span data-stu-id="eed2a-139">id</span></span>|<span data-ttu-id="eed2a-140">字符串</span><span class="sxs-lookup"><span data-stu-id="eed2a-140">String</span></span>|<span data-ttu-id="eed2a-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="eed2a-141">Key of the entity.</span></span>|
|<span data-ttu-id="eed2a-142">version</span><span class="sxs-lookup"><span data-stu-id="eed2a-142">version</span></span>|<span data-ttu-id="eed2a-143">String</span><span class="sxs-lookup"><span data-stu-id="eed2a-143">String</span></span>|<span data-ttu-id="eed2a-144">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="eed2a-144">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eed2a-145">关系</span><span class="sxs-lookup"><span data-stu-id="eed2a-145">Relationships</span></span>
<span data-ttu-id="eed2a-146">无</span><span class="sxs-lookup"><span data-stu-id="eed2a-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eed2a-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eed2a-147">JSON Representation</span></span>
<span data-ttu-id="eed2a-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eed2a-148">Here is a JSON representation of the resource.</span></span>
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





