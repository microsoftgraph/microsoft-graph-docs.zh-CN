---
title: managedAppPolicy 资源类型
description: ManagedAppPolicy 资源表示特定于平台的策略的基类型。
ms.openlocfilehash: 0cd886e594e58dec3486af6d447969f1610c84fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010283"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="5eb8a-103">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="5eb8a-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="5eb8a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5eb8a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5eb8a-105">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="5eb8a-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="5eb8a-106">方法</span><span class="sxs-lookup"><span data-stu-id="5eb8a-106">Methods</span></span>
|<span data-ttu-id="5eb8a-107">方法</span><span class="sxs-lookup"><span data-stu-id="5eb8a-107">Method</span></span>|<span data-ttu-id="5eb8a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="5eb8a-108">Return Type</span></span>|<span data-ttu-id="5eb8a-109">说明</span><span class="sxs-lookup"><span data-stu-id="5eb8a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5eb8a-110">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="5eb8a-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="5eb8a-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5eb8a-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="5eb8a-112">列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5eb8a-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="5eb8a-113">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="5eb8a-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="5eb8a-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="5eb8a-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="5eb8a-115">读取 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5eb8a-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="5eb8a-116">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="5eb8a-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="5eb8a-117">无</span><span class="sxs-lookup"><span data-stu-id="5eb8a-117">None</span></span>|<span data-ttu-id="5eb8a-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5eb8a-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5eb8a-119">属性</span><span class="sxs-lookup"><span data-stu-id="5eb8a-119">Properties</span></span>
|<span data-ttu-id="5eb8a-120">属性</span><span class="sxs-lookup"><span data-stu-id="5eb8a-120">Property</span></span>|<span data-ttu-id="5eb8a-121">类型</span><span class="sxs-lookup"><span data-stu-id="5eb8a-121">Type</span></span>|<span data-ttu-id="5eb8a-122">说明</span><span class="sxs-lookup"><span data-stu-id="5eb8a-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5eb8a-123">displayName</span><span class="sxs-lookup"><span data-stu-id="5eb8a-123">displayName</span></span>|<span data-ttu-id="5eb8a-124">String</span><span class="sxs-lookup"><span data-stu-id="5eb8a-124">String</span></span>|<span data-ttu-id="5eb8a-125">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="5eb8a-125">Policy display name.</span></span>|
|<span data-ttu-id="5eb8a-126">description</span><span class="sxs-lookup"><span data-stu-id="5eb8a-126">description</span></span>|<span data-ttu-id="5eb8a-127">String</span><span class="sxs-lookup"><span data-stu-id="5eb8a-127">String</span></span>|<span data-ttu-id="5eb8a-128">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="5eb8a-128">The policy's description.</span></span>|
|<span data-ttu-id="5eb8a-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5eb8a-129">createdDateTime</span></span>|<span data-ttu-id="5eb8a-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5eb8a-130">DateTimeOffset</span></span>|<span data-ttu-id="5eb8a-131">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5eb8a-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="5eb8a-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5eb8a-132">lastModifiedDateTime</span></span>|<span data-ttu-id="5eb8a-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5eb8a-133">DateTimeOffset</span></span>|<span data-ttu-id="5eb8a-134">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="5eb8a-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="5eb8a-135">id</span><span class="sxs-lookup"><span data-stu-id="5eb8a-135">id</span></span>|<span data-ttu-id="5eb8a-136">String</span><span class="sxs-lookup"><span data-stu-id="5eb8a-136">String</span></span>|<span data-ttu-id="5eb8a-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5eb8a-137">Key of the entity.</span></span>|
|<span data-ttu-id="5eb8a-138">version</span><span class="sxs-lookup"><span data-stu-id="5eb8a-138">version</span></span>|<span data-ttu-id="5eb8a-139">String</span><span class="sxs-lookup"><span data-stu-id="5eb8a-139">String</span></span>|<span data-ttu-id="5eb8a-140">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="5eb8a-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5eb8a-141">关系</span><span class="sxs-lookup"><span data-stu-id="5eb8a-141">Relationships</span></span>
<span data-ttu-id="5eb8a-142">无</span><span class="sxs-lookup"><span data-stu-id="5eb8a-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5eb8a-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5eb8a-143">JSON Representation</span></span>
<span data-ttu-id="5eb8a-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5eb8a-144">Here is a JSON representation of the resource.</span></span>
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



