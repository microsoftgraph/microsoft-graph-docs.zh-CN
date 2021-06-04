---
title: managedAppPolicy 资源类型
description: ManagedAppPolicy 资源表示特定于平台的策略的基类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 61fedfab47ee44d187d2de81c0699885c4af06f4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752775"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="8b3b0-103">managedAppPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b3b0-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="8b3b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b3b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b3b0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8b3b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b3b0-106">ManagedAppPolicy 资源表示特定于平台的策略的基类型。</span><span class="sxs-lookup"><span data-stu-id="8b3b0-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="8b3b0-107">Methods</span><span class="sxs-lookup"><span data-stu-id="8b3b0-107">Methods</span></span>
|<span data-ttu-id="8b3b0-108">方法</span><span class="sxs-lookup"><span data-stu-id="8b3b0-108">Method</span></span>|<span data-ttu-id="8b3b0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8b3b0-109">Return Type</span></span>|<span data-ttu-id="8b3b0-110">Description</span><span class="sxs-lookup"><span data-stu-id="8b3b0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8b3b0-111">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="8b3b0-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="8b3b0-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8b3b0-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="8b3b0-113">列出 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8b3b0-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="8b3b0-114">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="8b3b0-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="8b3b0-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="8b3b0-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="8b3b0-116">读取 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8b3b0-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="8b3b0-117">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="8b3b0-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="8b3b0-118">无</span><span class="sxs-lookup"><span data-stu-id="8b3b0-118">None</span></span>|<span data-ttu-id="8b3b0-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8b3b0-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8b3b0-120">属性</span><span class="sxs-lookup"><span data-stu-id="8b3b0-120">Properties</span></span>
|<span data-ttu-id="8b3b0-121">属性</span><span class="sxs-lookup"><span data-stu-id="8b3b0-121">Property</span></span>|<span data-ttu-id="8b3b0-122">类型</span><span class="sxs-lookup"><span data-stu-id="8b3b0-122">Type</span></span>|<span data-ttu-id="8b3b0-123">说明</span><span class="sxs-lookup"><span data-stu-id="8b3b0-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b3b0-124">displayName</span><span class="sxs-lookup"><span data-stu-id="8b3b0-124">displayName</span></span>|<span data-ttu-id="8b3b0-125">String</span><span class="sxs-lookup"><span data-stu-id="8b3b0-125">String</span></span>|<span data-ttu-id="8b3b0-126">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="8b3b0-126">Policy display name.</span></span>|
|<span data-ttu-id="8b3b0-127">说明</span><span class="sxs-lookup"><span data-stu-id="8b3b0-127">description</span></span>|<span data-ttu-id="8b3b0-128">String</span><span class="sxs-lookup"><span data-stu-id="8b3b0-128">String</span></span>|<span data-ttu-id="8b3b0-129">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="8b3b0-129">The policy's description.</span></span>|
|<span data-ttu-id="8b3b0-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b3b0-130">createdDateTime</span></span>|<span data-ttu-id="8b3b0-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b3b0-131">DateTimeOffset</span></span>|<span data-ttu-id="8b3b0-132">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8b3b0-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="8b3b0-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b3b0-133">lastModifiedDateTime</span></span>|<span data-ttu-id="8b3b0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b3b0-134">DateTimeOffset</span></span>|<span data-ttu-id="8b3b0-135">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="8b3b0-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="8b3b0-136">id</span><span class="sxs-lookup"><span data-stu-id="8b3b0-136">id</span></span>|<span data-ttu-id="8b3b0-137">String</span><span class="sxs-lookup"><span data-stu-id="8b3b0-137">String</span></span>|<span data-ttu-id="8b3b0-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8b3b0-138">Key of the entity.</span></span>|
|<span data-ttu-id="8b3b0-139">version</span><span class="sxs-lookup"><span data-stu-id="8b3b0-139">version</span></span>|<span data-ttu-id="8b3b0-140">String</span><span class="sxs-lookup"><span data-stu-id="8b3b0-140">String</span></span>|<span data-ttu-id="8b3b0-141">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="8b3b0-141">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b3b0-142">关系</span><span class="sxs-lookup"><span data-stu-id="8b3b0-142">Relationships</span></span>
<span data-ttu-id="8b3b0-143">无</span><span class="sxs-lookup"><span data-stu-id="8b3b0-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b3b0-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b3b0-144">JSON Representation</span></span>
<span data-ttu-id="8b3b0-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b3b0-145">Here is a JSON representation of the resource.</span></span>
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




