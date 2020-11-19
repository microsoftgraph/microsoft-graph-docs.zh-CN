---
title: managedAppPolicy 资源类型
description: ManagedAppPolicy 资源表示特定于平台的策略的基类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6e19b62fe5b947487a71b5df359a567fe03dce21
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302521"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="e2e71-103">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2e71-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="e2e71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2e71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2e71-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e2e71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2e71-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2e71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2e71-107">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="e2e71-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="e2e71-108">Methods</span><span class="sxs-lookup"><span data-stu-id="e2e71-108">Methods</span></span>
|<span data-ttu-id="e2e71-109">方法</span><span class="sxs-lookup"><span data-stu-id="e2e71-109">Method</span></span>|<span data-ttu-id="e2e71-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e2e71-110">Return Type</span></span>|<span data-ttu-id="e2e71-111">Description</span><span class="sxs-lookup"><span data-stu-id="e2e71-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e2e71-112">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="e2e71-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="e2e71-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2e71-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="e2e71-114">列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2e71-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="e2e71-115">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="e2e71-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="e2e71-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="e2e71-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="e2e71-117">读取 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2e71-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="e2e71-118">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="e2e71-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="e2e71-119">无</span><span class="sxs-lookup"><span data-stu-id="e2e71-119">None</span></span>|<span data-ttu-id="e2e71-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e2e71-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e2e71-121">属性</span><span class="sxs-lookup"><span data-stu-id="e2e71-121">Properties</span></span>
|<span data-ttu-id="e2e71-122">属性</span><span class="sxs-lookup"><span data-stu-id="e2e71-122">Property</span></span>|<span data-ttu-id="e2e71-123">类型</span><span class="sxs-lookup"><span data-stu-id="e2e71-123">Type</span></span>|<span data-ttu-id="e2e71-124">说明</span><span class="sxs-lookup"><span data-stu-id="e2e71-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2e71-125">displayName</span><span class="sxs-lookup"><span data-stu-id="e2e71-125">displayName</span></span>|<span data-ttu-id="e2e71-126">字符串</span><span class="sxs-lookup"><span data-stu-id="e2e71-126">String</span></span>|<span data-ttu-id="e2e71-127">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="e2e71-127">Policy display name.</span></span>|
|<span data-ttu-id="e2e71-128">description</span><span class="sxs-lookup"><span data-stu-id="e2e71-128">description</span></span>|<span data-ttu-id="e2e71-129">字符串</span><span class="sxs-lookup"><span data-stu-id="e2e71-129">String</span></span>|<span data-ttu-id="e2e71-130">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="e2e71-130">The policy's description.</span></span>|
|<span data-ttu-id="e2e71-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2e71-131">createdDateTime</span></span>|<span data-ttu-id="e2e71-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2e71-132">DateTimeOffset</span></span>|<span data-ttu-id="e2e71-133">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e2e71-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="e2e71-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2e71-134">lastModifiedDateTime</span></span>|<span data-ttu-id="e2e71-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2e71-135">DateTimeOffset</span></span>|<span data-ttu-id="e2e71-136">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="e2e71-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="e2e71-137">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e2e71-137">roleScopeTagIds</span></span>|<span data-ttu-id="e2e71-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="e2e71-138">String collection</span></span>|<span data-ttu-id="e2e71-139">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e2e71-139">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="e2e71-140">id</span><span class="sxs-lookup"><span data-stu-id="e2e71-140">id</span></span>|<span data-ttu-id="e2e71-141">字符串</span><span class="sxs-lookup"><span data-stu-id="e2e71-141">String</span></span>|<span data-ttu-id="e2e71-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e2e71-142">Key of the entity.</span></span>|
|<span data-ttu-id="e2e71-143">version</span><span class="sxs-lookup"><span data-stu-id="e2e71-143">version</span></span>|<span data-ttu-id="e2e71-144">String</span><span class="sxs-lookup"><span data-stu-id="e2e71-144">String</span></span>|<span data-ttu-id="e2e71-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="e2e71-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2e71-146">关系</span><span class="sxs-lookup"><span data-stu-id="e2e71-146">Relationships</span></span>
<span data-ttu-id="e2e71-147">无</span><span class="sxs-lookup"><span data-stu-id="e2e71-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2e71-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2e71-148">JSON Representation</span></span>
<span data-ttu-id="e2e71-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2e71-149">Here is a JSON representation of the resource.</span></span>
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




