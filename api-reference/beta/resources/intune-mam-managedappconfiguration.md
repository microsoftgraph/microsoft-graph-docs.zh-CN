---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f8927a4995f7b6e463db83377bc8c80b21730fa
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940839"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="86f5f-103">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="86f5f-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="86f5f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="86f5f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86f5f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86f5f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86f5f-106">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="86f5f-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="86f5f-107">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="86f5f-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="86f5f-108">方法</span><span class="sxs-lookup"><span data-stu-id="86f5f-108">Methods</span></span>
|<span data-ttu-id="86f5f-109">方法</span><span class="sxs-lookup"><span data-stu-id="86f5f-109">Method</span></span>|<span data-ttu-id="86f5f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="86f5f-110">Return Type</span></span>|<span data-ttu-id="86f5f-111">说明</span><span class="sxs-lookup"><span data-stu-id="86f5f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="86f5f-112">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="86f5f-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="86f5f-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="86f5f-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="86f5f-114">列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86f5f-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="86f5f-115">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="86f5f-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="86f5f-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="86f5f-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="86f5f-117">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86f5f-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="86f5f-118">属性</span><span class="sxs-lookup"><span data-stu-id="86f5f-118">Properties</span></span>
|<span data-ttu-id="86f5f-119">属性</span><span class="sxs-lookup"><span data-stu-id="86f5f-119">Property</span></span>|<span data-ttu-id="86f5f-120">类型</span><span class="sxs-lookup"><span data-stu-id="86f5f-120">Type</span></span>|<span data-ttu-id="86f5f-121">说明</span><span class="sxs-lookup"><span data-stu-id="86f5f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86f5f-122">displayName</span><span class="sxs-lookup"><span data-stu-id="86f5f-122">displayName</span></span>|<span data-ttu-id="86f5f-123">字符串</span><span class="sxs-lookup"><span data-stu-id="86f5f-123">String</span></span>|<span data-ttu-id="86f5f-124">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="86f5f-124">Policy display name.</span></span> <span data-ttu-id="86f5f-125">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="86f5f-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="86f5f-126">说明</span><span class="sxs-lookup"><span data-stu-id="86f5f-126">description</span></span>|<span data-ttu-id="86f5f-127">String</span><span class="sxs-lookup"><span data-stu-id="86f5f-127">String</span></span>|<span data-ttu-id="86f5f-128">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="86f5f-128">The policy's description.</span></span> <span data-ttu-id="86f5f-129">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="86f5f-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="86f5f-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86f5f-130">createdDateTime</span></span>|<span data-ttu-id="86f5f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86f5f-131">DateTimeOffset</span></span>|<span data-ttu-id="86f5f-132">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="86f5f-132">The date and time the policy was created.</span></span> <span data-ttu-id="86f5f-133">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="86f5f-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="86f5f-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86f5f-134">lastModifiedDateTime</span></span>|<span data-ttu-id="86f5f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86f5f-135">DateTimeOffset</span></span>|<span data-ttu-id="86f5f-136">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="86f5f-136">Last time the policy was modified.</span></span> <span data-ttu-id="86f5f-137">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="86f5f-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="86f5f-138">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="86f5f-138">roleScopeTagIds</span></span>|<span data-ttu-id="86f5f-139">String collection</span><span class="sxs-lookup"><span data-stu-id="86f5f-139">String collection</span></span>|<span data-ttu-id="86f5f-140">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="86f5f-140">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="86f5f-141">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="86f5f-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="86f5f-142">id</span><span class="sxs-lookup"><span data-stu-id="86f5f-142">id</span></span>|<span data-ttu-id="86f5f-143">字符串</span><span class="sxs-lookup"><span data-stu-id="86f5f-143">String</span></span>|<span data-ttu-id="86f5f-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="86f5f-144">Key of the entity.</span></span> <span data-ttu-id="86f5f-145">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="86f5f-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="86f5f-146">version</span><span class="sxs-lookup"><span data-stu-id="86f5f-146">version</span></span>|<span data-ttu-id="86f5f-147">String</span><span class="sxs-lookup"><span data-stu-id="86f5f-147">String</span></span>|<span data-ttu-id="86f5f-148">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="86f5f-148">Version of the entity.</span></span> <span data-ttu-id="86f5f-149">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="86f5f-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="86f5f-150">customSettings</span><span class="sxs-lookup"><span data-stu-id="86f5f-150">customSettings</span></span>|<span data-ttu-id="86f5f-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="86f5f-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="86f5f-152">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="86f5f-152">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="86f5f-153">关系</span><span class="sxs-lookup"><span data-stu-id="86f5f-153">Relationships</span></span>
<span data-ttu-id="86f5f-154">无</span><span class="sxs-lookup"><span data-stu-id="86f5f-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86f5f-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86f5f-155">JSON Representation</span></span>
<span data-ttu-id="86f5f-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86f5f-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```




