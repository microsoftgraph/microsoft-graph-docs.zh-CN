---
title: managedAppPolicy 资源类型
description: ManagedAppPolicy 资源表示特定于平台的策略的基类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5054566f0ee80940165ba19f8f0da197b5e4f3c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981103"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="af0bd-103">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="af0bd-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="af0bd-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="af0bd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af0bd-105">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="af0bd-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="af0bd-106">方法</span><span class="sxs-lookup"><span data-stu-id="af0bd-106">Methods</span></span>
|<span data-ttu-id="af0bd-107">方法</span><span class="sxs-lookup"><span data-stu-id="af0bd-107">Method</span></span>|<span data-ttu-id="af0bd-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="af0bd-108">Return Type</span></span>|<span data-ttu-id="af0bd-109">说明</span><span class="sxs-lookup"><span data-stu-id="af0bd-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="af0bd-110">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="af0bd-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="af0bd-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af0bd-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="af0bd-112">列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="af0bd-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="af0bd-113">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="af0bd-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="af0bd-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="af0bd-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="af0bd-115">读取 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="af0bd-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="af0bd-116">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="af0bd-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="af0bd-117">无</span><span class="sxs-lookup"><span data-stu-id="af0bd-117">None</span></span>|<span data-ttu-id="af0bd-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="af0bd-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="af0bd-119">属性</span><span class="sxs-lookup"><span data-stu-id="af0bd-119">Properties</span></span>
|<span data-ttu-id="af0bd-120">属性</span><span class="sxs-lookup"><span data-stu-id="af0bd-120">Property</span></span>|<span data-ttu-id="af0bd-121">类型</span><span class="sxs-lookup"><span data-stu-id="af0bd-121">Type</span></span>|<span data-ttu-id="af0bd-122">说明</span><span class="sxs-lookup"><span data-stu-id="af0bd-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af0bd-123">displayName</span><span class="sxs-lookup"><span data-stu-id="af0bd-123">displayName</span></span>|<span data-ttu-id="af0bd-124">String</span><span class="sxs-lookup"><span data-stu-id="af0bd-124">String</span></span>|<span data-ttu-id="af0bd-125">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="af0bd-125">Policy display name.</span></span>|
|<span data-ttu-id="af0bd-126">description</span><span class="sxs-lookup"><span data-stu-id="af0bd-126">description</span></span>|<span data-ttu-id="af0bd-127">String</span><span class="sxs-lookup"><span data-stu-id="af0bd-127">String</span></span>|<span data-ttu-id="af0bd-128">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="af0bd-128">The policy's description.</span></span>|
|<span data-ttu-id="af0bd-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af0bd-129">createdDateTime</span></span>|<span data-ttu-id="af0bd-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af0bd-130">DateTimeOffset</span></span>|<span data-ttu-id="af0bd-131">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="af0bd-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="af0bd-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af0bd-132">lastModifiedDateTime</span></span>|<span data-ttu-id="af0bd-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af0bd-133">DateTimeOffset</span></span>|<span data-ttu-id="af0bd-134">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="af0bd-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="af0bd-135">id</span><span class="sxs-lookup"><span data-stu-id="af0bd-135">id</span></span>|<span data-ttu-id="af0bd-136">String</span><span class="sxs-lookup"><span data-stu-id="af0bd-136">String</span></span>|<span data-ttu-id="af0bd-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="af0bd-137">Key of the entity.</span></span>|
|<span data-ttu-id="af0bd-138">version</span><span class="sxs-lookup"><span data-stu-id="af0bd-138">version</span></span>|<span data-ttu-id="af0bd-139">String</span><span class="sxs-lookup"><span data-stu-id="af0bd-139">String</span></span>|<span data-ttu-id="af0bd-140">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="af0bd-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af0bd-141">关系</span><span class="sxs-lookup"><span data-stu-id="af0bd-141">Relationships</span></span>
<span data-ttu-id="af0bd-142">无</span><span class="sxs-lookup"><span data-stu-id="af0bd-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="af0bd-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af0bd-143">JSON Representation</span></span>
<span data-ttu-id="af0bd-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af0bd-144">Here is a JSON representation of the resource.</span></span>
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



