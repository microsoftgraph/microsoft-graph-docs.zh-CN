---
title: managedAppPolicy 资源类型
description: ManagedAppPolicy 资源表示特定于平台的策略的基类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3cea81d492e708c1d21039c6286fe01e70a590b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840731"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="d10d6-103">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="d10d6-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="d10d6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d10d6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d10d6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d10d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d10d6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d10d6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d10d6-107">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="d10d6-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="d10d6-108">方法</span><span class="sxs-lookup"><span data-stu-id="d10d6-108">Methods</span></span>
|<span data-ttu-id="d10d6-109">方法</span><span class="sxs-lookup"><span data-stu-id="d10d6-109">Method</span></span>|<span data-ttu-id="d10d6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d10d6-110">Return Type</span></span>|<span data-ttu-id="d10d6-111">说明</span><span class="sxs-lookup"><span data-stu-id="d10d6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d10d6-112">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="d10d6-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="d10d6-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d10d6-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d10d6-114">列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d10d6-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="d10d6-115">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="d10d6-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="d10d6-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="d10d6-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="d10d6-117">读取 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d10d6-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="d10d6-118">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="d10d6-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="d10d6-119">无</span><span class="sxs-lookup"><span data-stu-id="d10d6-119">None</span></span>|<span data-ttu-id="d10d6-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d10d6-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d10d6-121">属性</span><span class="sxs-lookup"><span data-stu-id="d10d6-121">Properties</span></span>
|<span data-ttu-id="d10d6-122">属性</span><span class="sxs-lookup"><span data-stu-id="d10d6-122">Property</span></span>|<span data-ttu-id="d10d6-123">类型</span><span class="sxs-lookup"><span data-stu-id="d10d6-123">Type</span></span>|<span data-ttu-id="d10d6-124">说明</span><span class="sxs-lookup"><span data-stu-id="d10d6-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d10d6-125">displayName</span><span class="sxs-lookup"><span data-stu-id="d10d6-125">displayName</span></span>|<span data-ttu-id="d10d6-126">String</span><span class="sxs-lookup"><span data-stu-id="d10d6-126">String</span></span>|<span data-ttu-id="d10d6-127">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="d10d6-127">Policy display name.</span></span>|
|<span data-ttu-id="d10d6-128">description</span><span class="sxs-lookup"><span data-stu-id="d10d6-128">description</span></span>|<span data-ttu-id="d10d6-129">String</span><span class="sxs-lookup"><span data-stu-id="d10d6-129">String</span></span>|<span data-ttu-id="d10d6-130">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="d10d6-130">The policy's description.</span></span>|
|<span data-ttu-id="d10d6-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d10d6-131">createdDateTime</span></span>|<span data-ttu-id="d10d6-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d10d6-132">DateTimeOffset</span></span>|<span data-ttu-id="d10d6-133">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d10d6-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="d10d6-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d10d6-134">lastModifiedDateTime</span></span>|<span data-ttu-id="d10d6-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d10d6-135">DateTimeOffset</span></span>|<span data-ttu-id="d10d6-136">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="d10d6-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="d10d6-137">id</span><span class="sxs-lookup"><span data-stu-id="d10d6-137">id</span></span>|<span data-ttu-id="d10d6-138">String</span><span class="sxs-lookup"><span data-stu-id="d10d6-138">String</span></span>|<span data-ttu-id="d10d6-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d10d6-139">Key of the entity.</span></span>|
|<span data-ttu-id="d10d6-140">version</span><span class="sxs-lookup"><span data-stu-id="d10d6-140">version</span></span>|<span data-ttu-id="d10d6-141">String</span><span class="sxs-lookup"><span data-stu-id="d10d6-141">String</span></span>|<span data-ttu-id="d10d6-142">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="d10d6-142">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d10d6-143">关系</span><span class="sxs-lookup"><span data-stu-id="d10d6-143">Relationships</span></span>
<span data-ttu-id="d10d6-144">无</span><span class="sxs-lookup"><span data-stu-id="d10d6-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d10d6-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d10d6-145">JSON Representation</span></span>
<span data-ttu-id="d10d6-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d10d6-146">Here is a JSON representation of the resource.</span></span>
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





