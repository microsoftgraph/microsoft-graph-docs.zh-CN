---
title: managedAppPolicy 资源类型
description: ManagedAppPolicy 资源表示特定于平台的策略的基类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5766e3a467a157bac0d876fd0178dc3ba1cb94e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888079"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="6ce26-103">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ce26-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="6ce26-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6ce26-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ce26-105">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="6ce26-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="6ce26-106">方法</span><span class="sxs-lookup"><span data-stu-id="6ce26-106">Methods</span></span>
|<span data-ttu-id="6ce26-107">方法</span><span class="sxs-lookup"><span data-stu-id="6ce26-107">Method</span></span>|<span data-ttu-id="6ce26-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6ce26-108">Return Type</span></span>|<span data-ttu-id="6ce26-109">说明</span><span class="sxs-lookup"><span data-stu-id="6ce26-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6ce26-110">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="6ce26-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="6ce26-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6ce26-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="6ce26-112">列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6ce26-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="6ce26-113">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="6ce26-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="6ce26-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="6ce26-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="6ce26-115">读取 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6ce26-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="6ce26-116">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="6ce26-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="6ce26-117">无</span><span class="sxs-lookup"><span data-stu-id="6ce26-117">None</span></span>|<span data-ttu-id="6ce26-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6ce26-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6ce26-119">属性</span><span class="sxs-lookup"><span data-stu-id="6ce26-119">Properties</span></span>
|<span data-ttu-id="6ce26-120">属性</span><span class="sxs-lookup"><span data-stu-id="6ce26-120">Property</span></span>|<span data-ttu-id="6ce26-121">类型</span><span class="sxs-lookup"><span data-stu-id="6ce26-121">Type</span></span>|<span data-ttu-id="6ce26-122">说明</span><span class="sxs-lookup"><span data-stu-id="6ce26-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ce26-123">displayName</span><span class="sxs-lookup"><span data-stu-id="6ce26-123">displayName</span></span>|<span data-ttu-id="6ce26-124">String</span><span class="sxs-lookup"><span data-stu-id="6ce26-124">String</span></span>|<span data-ttu-id="6ce26-125">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="6ce26-125">Policy display name.</span></span>|
|<span data-ttu-id="6ce26-126">description</span><span class="sxs-lookup"><span data-stu-id="6ce26-126">description</span></span>|<span data-ttu-id="6ce26-127">String</span><span class="sxs-lookup"><span data-stu-id="6ce26-127">String</span></span>|<span data-ttu-id="6ce26-128">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="6ce26-128">The policy's description.</span></span>|
|<span data-ttu-id="6ce26-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ce26-129">createdDateTime</span></span>|<span data-ttu-id="6ce26-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ce26-130">DateTimeOffset</span></span>|<span data-ttu-id="6ce26-131">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6ce26-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="6ce26-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ce26-132">lastModifiedDateTime</span></span>|<span data-ttu-id="6ce26-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ce26-133">DateTimeOffset</span></span>|<span data-ttu-id="6ce26-134">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="6ce26-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="6ce26-135">id</span><span class="sxs-lookup"><span data-stu-id="6ce26-135">id</span></span>|<span data-ttu-id="6ce26-136">String</span><span class="sxs-lookup"><span data-stu-id="6ce26-136">String</span></span>|<span data-ttu-id="6ce26-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6ce26-137">Key of the entity.</span></span>|
|<span data-ttu-id="6ce26-138">version</span><span class="sxs-lookup"><span data-stu-id="6ce26-138">version</span></span>|<span data-ttu-id="6ce26-139">String</span><span class="sxs-lookup"><span data-stu-id="6ce26-139">String</span></span>|<span data-ttu-id="6ce26-140">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="6ce26-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ce26-141">关系</span><span class="sxs-lookup"><span data-stu-id="6ce26-141">Relationships</span></span>
<span data-ttu-id="6ce26-142">无</span><span class="sxs-lookup"><span data-stu-id="6ce26-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6ce26-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ce26-143">JSON Representation</span></span>
<span data-ttu-id="6ce26-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ce26-144">Here is a JSON representation of the resource.</span></span>
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



