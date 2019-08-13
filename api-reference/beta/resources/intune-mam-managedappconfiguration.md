---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 37d0f1d845891a397d5109a4d50d4de83b27f212
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332181"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="d69bf-103">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d69bf-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="d69bf-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d69bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d69bf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d69bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d69bf-106">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="d69bf-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="d69bf-107">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d69bf-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d69bf-108">方法</span><span class="sxs-lookup"><span data-stu-id="d69bf-108">Methods</span></span>
|<span data-ttu-id="d69bf-109">方法</span><span class="sxs-lookup"><span data-stu-id="d69bf-109">Method</span></span>|<span data-ttu-id="d69bf-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d69bf-110">Return Type</span></span>|<span data-ttu-id="d69bf-111">说明</span><span class="sxs-lookup"><span data-stu-id="d69bf-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d69bf-112">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="d69bf-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="d69bf-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d69bf-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="d69bf-114">列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d69bf-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d69bf-115">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d69bf-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="d69bf-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d69bf-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="d69bf-117">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d69bf-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d69bf-118">属性</span><span class="sxs-lookup"><span data-stu-id="d69bf-118">Properties</span></span>
|<span data-ttu-id="d69bf-119">属性</span><span class="sxs-lookup"><span data-stu-id="d69bf-119">Property</span></span>|<span data-ttu-id="d69bf-120">类型</span><span class="sxs-lookup"><span data-stu-id="d69bf-120">Type</span></span>|<span data-ttu-id="d69bf-121">说明</span><span class="sxs-lookup"><span data-stu-id="d69bf-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d69bf-122">displayName</span><span class="sxs-lookup"><span data-stu-id="d69bf-122">displayName</span></span>|<span data-ttu-id="d69bf-123">字符串</span><span class="sxs-lookup"><span data-stu-id="d69bf-123">String</span></span>|<span data-ttu-id="d69bf-124">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="d69bf-124">Policy display name.</span></span> <span data-ttu-id="d69bf-125">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d69bf-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d69bf-126">说明</span><span class="sxs-lookup"><span data-stu-id="d69bf-126">description</span></span>|<span data-ttu-id="d69bf-127">String</span><span class="sxs-lookup"><span data-stu-id="d69bf-127">String</span></span>|<span data-ttu-id="d69bf-128">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="d69bf-128">The policy's description.</span></span> <span data-ttu-id="d69bf-129">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d69bf-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d69bf-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d69bf-130">createdDateTime</span></span>|<span data-ttu-id="d69bf-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d69bf-131">DateTimeOffset</span></span>|<span data-ttu-id="d69bf-132">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d69bf-132">The date and time the policy was created.</span></span> <span data-ttu-id="d69bf-133">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d69bf-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d69bf-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d69bf-134">lastModifiedDateTime</span></span>|<span data-ttu-id="d69bf-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d69bf-135">DateTimeOffset</span></span>|<span data-ttu-id="d69bf-136">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="d69bf-136">Last time the policy was modified.</span></span> <span data-ttu-id="d69bf-137">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d69bf-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d69bf-138">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d69bf-138">roleScopeTagIds</span></span>|<span data-ttu-id="d69bf-139">String collection</span><span class="sxs-lookup"><span data-stu-id="d69bf-139">String collection</span></span>|<span data-ttu-id="d69bf-140">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d69bf-140">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d69bf-141">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d69bf-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d69bf-142">id</span><span class="sxs-lookup"><span data-stu-id="d69bf-142">id</span></span>|<span data-ttu-id="d69bf-143">字符串</span><span class="sxs-lookup"><span data-stu-id="d69bf-143">String</span></span>|<span data-ttu-id="d69bf-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d69bf-144">Key of the entity.</span></span> <span data-ttu-id="d69bf-145">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d69bf-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d69bf-146">version</span><span class="sxs-lookup"><span data-stu-id="d69bf-146">version</span></span>|<span data-ttu-id="d69bf-147">String</span><span class="sxs-lookup"><span data-stu-id="d69bf-147">String</span></span>|<span data-ttu-id="d69bf-148">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="d69bf-148">Version of the entity.</span></span> <span data-ttu-id="d69bf-149">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d69bf-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d69bf-150">customSettings</span><span class="sxs-lookup"><span data-stu-id="d69bf-150">customSettings</span></span>|<span data-ttu-id="d69bf-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d69bf-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d69bf-152">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="d69bf-152">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="d69bf-153">关系</span><span class="sxs-lookup"><span data-stu-id="d69bf-153">Relationships</span></span>
<span data-ttu-id="d69bf-154">无</span><span class="sxs-lookup"><span data-stu-id="d69bf-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d69bf-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d69bf-155">JSON Representation</span></span>
<span data-ttu-id="d69bf-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d69bf-156">Here is a JSON representation of the resource.</span></span>
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



