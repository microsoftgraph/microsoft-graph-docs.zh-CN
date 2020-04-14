---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80484c3e5446cbb309ee3ae403475dedf075da56
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43373413"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="40331-103">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="40331-103">managedAppConfiguration resource type</span></span>

<span data-ttu-id="40331-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40331-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40331-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="40331-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40331-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40331-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40331-107">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="40331-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="40331-108">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="40331-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="40331-109">方法</span><span class="sxs-lookup"><span data-stu-id="40331-109">Methods</span></span>
|<span data-ttu-id="40331-110">方法</span><span class="sxs-lookup"><span data-stu-id="40331-110">Method</span></span>|<span data-ttu-id="40331-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="40331-111">Return Type</span></span>|<span data-ttu-id="40331-112">说明</span><span class="sxs-lookup"><span data-stu-id="40331-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="40331-113">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="40331-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="40331-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="40331-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="40331-115">列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="40331-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="40331-116">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="40331-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="40331-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="40331-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="40331-118">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="40331-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="40331-119">属性</span><span class="sxs-lookup"><span data-stu-id="40331-119">Properties</span></span>
|<span data-ttu-id="40331-120">属性</span><span class="sxs-lookup"><span data-stu-id="40331-120">Property</span></span>|<span data-ttu-id="40331-121">类型</span><span class="sxs-lookup"><span data-stu-id="40331-121">Type</span></span>|<span data-ttu-id="40331-122">说明</span><span class="sxs-lookup"><span data-stu-id="40331-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40331-123">displayName</span><span class="sxs-lookup"><span data-stu-id="40331-123">displayName</span></span>|<span data-ttu-id="40331-124">字符串</span><span class="sxs-lookup"><span data-stu-id="40331-124">String</span></span>|<span data-ttu-id="40331-125">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="40331-125">Policy display name.</span></span> <span data-ttu-id="40331-126">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="40331-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="40331-127">description</span><span class="sxs-lookup"><span data-stu-id="40331-127">description</span></span>|<span data-ttu-id="40331-128">String</span><span class="sxs-lookup"><span data-stu-id="40331-128">String</span></span>|<span data-ttu-id="40331-129">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="40331-129">The policy's description.</span></span> <span data-ttu-id="40331-130">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="40331-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="40331-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40331-131">createdDateTime</span></span>|<span data-ttu-id="40331-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40331-132">DateTimeOffset</span></span>|<span data-ttu-id="40331-133">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="40331-133">The date and time the policy was created.</span></span> <span data-ttu-id="40331-134">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="40331-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="40331-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40331-135">lastModifiedDateTime</span></span>|<span data-ttu-id="40331-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40331-136">DateTimeOffset</span></span>|<span data-ttu-id="40331-137">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="40331-137">Last time the policy was modified.</span></span> <span data-ttu-id="40331-138">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="40331-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="40331-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="40331-139">roleScopeTagIds</span></span>|<span data-ttu-id="40331-140">String 集合</span><span class="sxs-lookup"><span data-stu-id="40331-140">String collection</span></span>|<span data-ttu-id="40331-141">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="40331-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="40331-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="40331-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="40331-143">id</span><span class="sxs-lookup"><span data-stu-id="40331-143">id</span></span>|<span data-ttu-id="40331-144">字符串</span><span class="sxs-lookup"><span data-stu-id="40331-144">String</span></span>|<span data-ttu-id="40331-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="40331-145">Key of the entity.</span></span> <span data-ttu-id="40331-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="40331-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="40331-147">version</span><span class="sxs-lookup"><span data-stu-id="40331-147">version</span></span>|<span data-ttu-id="40331-148">String</span><span class="sxs-lookup"><span data-stu-id="40331-148">String</span></span>|<span data-ttu-id="40331-149">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="40331-149">Version of the entity.</span></span> <span data-ttu-id="40331-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="40331-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="40331-151">customSettings</span><span class="sxs-lookup"><span data-stu-id="40331-151">customSettings</span></span>|<span data-ttu-id="40331-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="40331-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="40331-153">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="40331-153">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="40331-154">关系</span><span class="sxs-lookup"><span data-stu-id="40331-154">Relationships</span></span>
<span data-ttu-id="40331-155">无</span><span class="sxs-lookup"><span data-stu-id="40331-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40331-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40331-156">JSON Representation</span></span>
<span data-ttu-id="40331-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40331-157">Here is a JSON representation of the resource.</span></span>
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



