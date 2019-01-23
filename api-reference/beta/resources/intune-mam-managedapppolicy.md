---
title: managedAppPolicy 资源类型
description: ManagedAppPolicy 资源表示特定于平台的策略的基类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6bc4a7bbc4bc0dc85da8759ad95162712b1deb13
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422976"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="be106-103">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="be106-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="be106-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="be106-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="be106-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="be106-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be106-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be106-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be106-107">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="be106-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="be106-108">方法</span><span class="sxs-lookup"><span data-stu-id="be106-108">Methods</span></span>
|<span data-ttu-id="be106-109">方法</span><span class="sxs-lookup"><span data-stu-id="be106-109">Method</span></span>|<span data-ttu-id="be106-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="be106-110">Return Type</span></span>|<span data-ttu-id="be106-111">说明</span><span class="sxs-lookup"><span data-stu-id="be106-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be106-112">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="be106-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="be106-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be106-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="be106-114">列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be106-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="be106-115">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="be106-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="be106-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="be106-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="be106-117">读取 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be106-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="be106-118">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="be106-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="be106-119">无</span><span class="sxs-lookup"><span data-stu-id="be106-119">None</span></span>|<span data-ttu-id="be106-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="be106-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="be106-121">属性</span><span class="sxs-lookup"><span data-stu-id="be106-121">Properties</span></span>
|<span data-ttu-id="be106-122">属性</span><span class="sxs-lookup"><span data-stu-id="be106-122">Property</span></span>|<span data-ttu-id="be106-123">类型</span><span class="sxs-lookup"><span data-stu-id="be106-123">Type</span></span>|<span data-ttu-id="be106-124">说明</span><span class="sxs-lookup"><span data-stu-id="be106-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be106-125">displayName</span><span class="sxs-lookup"><span data-stu-id="be106-125">displayName</span></span>|<span data-ttu-id="be106-126">String</span><span class="sxs-lookup"><span data-stu-id="be106-126">String</span></span>|<span data-ttu-id="be106-127">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="be106-127">Policy display name.</span></span>|
|<span data-ttu-id="be106-128">description</span><span class="sxs-lookup"><span data-stu-id="be106-128">description</span></span>|<span data-ttu-id="be106-129">String</span><span class="sxs-lookup"><span data-stu-id="be106-129">String</span></span>|<span data-ttu-id="be106-130">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="be106-130">The policy's description.</span></span>|
|<span data-ttu-id="be106-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be106-131">createdDateTime</span></span>|<span data-ttu-id="be106-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be106-132">DateTimeOffset</span></span>|<span data-ttu-id="be106-133">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="be106-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="be106-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be106-134">lastModifiedDateTime</span></span>|<span data-ttu-id="be106-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be106-135">DateTimeOffset</span></span>|<span data-ttu-id="be106-136">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="be106-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="be106-137">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="be106-137">roleScopeTagIds</span></span>|<span data-ttu-id="be106-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="be106-138">String collection</span></span>|<span data-ttu-id="be106-139">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="be106-139">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="be106-140">id</span><span class="sxs-lookup"><span data-stu-id="be106-140">id</span></span>|<span data-ttu-id="be106-141">String</span><span class="sxs-lookup"><span data-stu-id="be106-141">String</span></span>|<span data-ttu-id="be106-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="be106-142">Key of the entity.</span></span>|
|<span data-ttu-id="be106-143">version</span><span class="sxs-lookup"><span data-stu-id="be106-143">version</span></span>|<span data-ttu-id="be106-144">String</span><span class="sxs-lookup"><span data-stu-id="be106-144">String</span></span>|<span data-ttu-id="be106-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="be106-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be106-146">关系</span><span class="sxs-lookup"><span data-stu-id="be106-146">Relationships</span></span>
<span data-ttu-id="be106-147">无</span><span class="sxs-lookup"><span data-stu-id="be106-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be106-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be106-148">JSON Representation</span></span>
<span data-ttu-id="be106-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be106-149">Here is a JSON representation of the resource.</span></span>
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




