---
title: managedAppPolicy 资源类型
description: ManagedAppPolicy 资源表示特定于平台的策略的基类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 55045faa017c852b812c04b2565269773090ee2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448380"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="39826-103">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="39826-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="39826-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="39826-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39826-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="39826-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39826-106">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="39826-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="39826-107">方法</span><span class="sxs-lookup"><span data-stu-id="39826-107">Methods</span></span>
|<span data-ttu-id="39826-108">方法</span><span class="sxs-lookup"><span data-stu-id="39826-108">Method</span></span>|<span data-ttu-id="39826-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="39826-109">Return Type</span></span>|<span data-ttu-id="39826-110">说明</span><span class="sxs-lookup"><span data-stu-id="39826-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39826-111">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="39826-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="39826-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39826-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="39826-113">列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="39826-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="39826-114">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="39826-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="39826-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="39826-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="39826-116">读取 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="39826-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="39826-117">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="39826-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="39826-118">无</span><span class="sxs-lookup"><span data-stu-id="39826-118">None</span></span>|<span data-ttu-id="39826-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="39826-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="39826-120">属性</span><span class="sxs-lookup"><span data-stu-id="39826-120">Properties</span></span>
|<span data-ttu-id="39826-121">属性</span><span class="sxs-lookup"><span data-stu-id="39826-121">Property</span></span>|<span data-ttu-id="39826-122">类型</span><span class="sxs-lookup"><span data-stu-id="39826-122">Type</span></span>|<span data-ttu-id="39826-123">说明</span><span class="sxs-lookup"><span data-stu-id="39826-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39826-124">displayName</span><span class="sxs-lookup"><span data-stu-id="39826-124">displayName</span></span>|<span data-ttu-id="39826-125">字符串</span><span class="sxs-lookup"><span data-stu-id="39826-125">String</span></span>|<span data-ttu-id="39826-126">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="39826-126">Policy display name.</span></span>|
|<span data-ttu-id="39826-127">说明</span><span class="sxs-lookup"><span data-stu-id="39826-127">description</span></span>|<span data-ttu-id="39826-128">String</span><span class="sxs-lookup"><span data-stu-id="39826-128">String</span></span>|<span data-ttu-id="39826-129">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="39826-129">The policy's description.</span></span>|
|<span data-ttu-id="39826-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39826-130">createdDateTime</span></span>|<span data-ttu-id="39826-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39826-131">DateTimeOffset</span></span>|<span data-ttu-id="39826-132">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="39826-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="39826-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39826-133">lastModifiedDateTime</span></span>|<span data-ttu-id="39826-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39826-134">DateTimeOffset</span></span>|<span data-ttu-id="39826-135">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="39826-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="39826-136">id</span><span class="sxs-lookup"><span data-stu-id="39826-136">id</span></span>|<span data-ttu-id="39826-137">字符串</span><span class="sxs-lookup"><span data-stu-id="39826-137">String</span></span>|<span data-ttu-id="39826-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="39826-138">Key of the entity.</span></span>|
|<span data-ttu-id="39826-139">version</span><span class="sxs-lookup"><span data-stu-id="39826-139">version</span></span>|<span data-ttu-id="39826-140">String</span><span class="sxs-lookup"><span data-stu-id="39826-140">String</span></span>|<span data-ttu-id="39826-141">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="39826-141">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39826-142">关系</span><span class="sxs-lookup"><span data-stu-id="39826-142">Relationships</span></span>
<span data-ttu-id="39826-143">无</span><span class="sxs-lookup"><span data-stu-id="39826-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39826-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39826-144">JSON Representation</span></span>
<span data-ttu-id="39826-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39826-145">Here is a JSON representation of the resource.</span></span>
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




