---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 48944007e33237e175822cfd2f5b076a5ddbe50e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524341"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="681b1-103">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="681b1-103">managedAppConfiguration resource type</span></span>

<span data-ttu-id="681b1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="681b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="681b1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="681b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="681b1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="681b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="681b1-107">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="681b1-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="681b1-108">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="681b1-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="681b1-109">方法</span><span class="sxs-lookup"><span data-stu-id="681b1-109">Methods</span></span>
|<span data-ttu-id="681b1-110">方法</span><span class="sxs-lookup"><span data-stu-id="681b1-110">Method</span></span>|<span data-ttu-id="681b1-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="681b1-111">Return Type</span></span>|<span data-ttu-id="681b1-112">说明</span><span class="sxs-lookup"><span data-stu-id="681b1-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="681b1-113">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="681b1-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="681b1-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="681b1-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="681b1-115">列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="681b1-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="681b1-116">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="681b1-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="681b1-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="681b1-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="681b1-118">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="681b1-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="681b1-119">属性</span><span class="sxs-lookup"><span data-stu-id="681b1-119">Properties</span></span>
|<span data-ttu-id="681b1-120">属性</span><span class="sxs-lookup"><span data-stu-id="681b1-120">Property</span></span>|<span data-ttu-id="681b1-121">类型</span><span class="sxs-lookup"><span data-stu-id="681b1-121">Type</span></span>|<span data-ttu-id="681b1-122">说明</span><span class="sxs-lookup"><span data-stu-id="681b1-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="681b1-123">displayName</span><span class="sxs-lookup"><span data-stu-id="681b1-123">displayName</span></span>|<span data-ttu-id="681b1-124">字符串</span><span class="sxs-lookup"><span data-stu-id="681b1-124">String</span></span>|<span data-ttu-id="681b1-125">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="681b1-125">Policy display name.</span></span> <span data-ttu-id="681b1-126">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="681b1-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="681b1-127">说明</span><span class="sxs-lookup"><span data-stu-id="681b1-127">description</span></span>|<span data-ttu-id="681b1-128">String</span><span class="sxs-lookup"><span data-stu-id="681b1-128">String</span></span>|<span data-ttu-id="681b1-129">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="681b1-129">The policy's description.</span></span> <span data-ttu-id="681b1-130">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="681b1-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="681b1-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="681b1-131">createdDateTime</span></span>|<span data-ttu-id="681b1-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="681b1-132">DateTimeOffset</span></span>|<span data-ttu-id="681b1-133">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="681b1-133">The date and time the policy was created.</span></span> <span data-ttu-id="681b1-134">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="681b1-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="681b1-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="681b1-135">lastModifiedDateTime</span></span>|<span data-ttu-id="681b1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="681b1-136">DateTimeOffset</span></span>|<span data-ttu-id="681b1-137">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="681b1-137">Last time the policy was modified.</span></span> <span data-ttu-id="681b1-138">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="681b1-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="681b1-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="681b1-139">roleScopeTagIds</span></span>|<span data-ttu-id="681b1-140">String 集合</span><span class="sxs-lookup"><span data-stu-id="681b1-140">String collection</span></span>|<span data-ttu-id="681b1-141">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="681b1-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="681b1-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="681b1-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="681b1-143">id</span><span class="sxs-lookup"><span data-stu-id="681b1-143">id</span></span>|<span data-ttu-id="681b1-144">字符串</span><span class="sxs-lookup"><span data-stu-id="681b1-144">String</span></span>|<span data-ttu-id="681b1-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="681b1-145">Key of the entity.</span></span> <span data-ttu-id="681b1-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="681b1-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="681b1-147">version</span><span class="sxs-lookup"><span data-stu-id="681b1-147">version</span></span>|<span data-ttu-id="681b1-148">String</span><span class="sxs-lookup"><span data-stu-id="681b1-148">String</span></span>|<span data-ttu-id="681b1-149">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="681b1-149">Version of the entity.</span></span> <span data-ttu-id="681b1-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="681b1-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="681b1-151">customSettings</span><span class="sxs-lookup"><span data-stu-id="681b1-151">customSettings</span></span>|<span data-ttu-id="681b1-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="681b1-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="681b1-153">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="681b1-153">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="681b1-154">关系</span><span class="sxs-lookup"><span data-stu-id="681b1-154">Relationships</span></span>
<span data-ttu-id="681b1-155">无</span><span class="sxs-lookup"><span data-stu-id="681b1-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="681b1-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="681b1-156">JSON Representation</span></span>
<span data-ttu-id="681b1-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="681b1-157">Here is a JSON representation of the resource.</span></span>
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



