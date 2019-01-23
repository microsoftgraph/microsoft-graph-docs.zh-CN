---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 67b445c5f7882bb4befc3e2c5cc46e26c5cf50fc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405672"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="81332-103">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="81332-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="81332-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="81332-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="81332-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="81332-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81332-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81332-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81332-107">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="81332-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="81332-108">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81332-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="81332-109">方法</span><span class="sxs-lookup"><span data-stu-id="81332-109">Methods</span></span>
|<span data-ttu-id="81332-110">方法</span><span class="sxs-lookup"><span data-stu-id="81332-110">Method</span></span>|<span data-ttu-id="81332-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="81332-111">Return Type</span></span>|<span data-ttu-id="81332-112">说明</span><span class="sxs-lookup"><span data-stu-id="81332-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81332-113">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="81332-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="81332-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81332-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="81332-115">列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81332-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="81332-116">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="81332-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="81332-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="81332-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="81332-118">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81332-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81332-119">属性</span><span class="sxs-lookup"><span data-stu-id="81332-119">Properties</span></span>
|<span data-ttu-id="81332-120">属性</span><span class="sxs-lookup"><span data-stu-id="81332-120">Property</span></span>|<span data-ttu-id="81332-121">类型</span><span class="sxs-lookup"><span data-stu-id="81332-121">Type</span></span>|<span data-ttu-id="81332-122">说明</span><span class="sxs-lookup"><span data-stu-id="81332-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81332-123">displayName</span><span class="sxs-lookup"><span data-stu-id="81332-123">displayName</span></span>|<span data-ttu-id="81332-124">String</span><span class="sxs-lookup"><span data-stu-id="81332-124">String</span></span>|<span data-ttu-id="81332-125">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="81332-125">Policy display name.</span></span> <span data-ttu-id="81332-126">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81332-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81332-127">description</span><span class="sxs-lookup"><span data-stu-id="81332-127">description</span></span>|<span data-ttu-id="81332-128">String</span><span class="sxs-lookup"><span data-stu-id="81332-128">String</span></span>|<span data-ttu-id="81332-129">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="81332-129">The policy's description.</span></span> <span data-ttu-id="81332-130">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81332-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81332-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81332-131">createdDateTime</span></span>|<span data-ttu-id="81332-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81332-132">DateTimeOffset</span></span>|<span data-ttu-id="81332-133">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="81332-133">The date and time the policy was created.</span></span> <span data-ttu-id="81332-134">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81332-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81332-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81332-135">lastModifiedDateTime</span></span>|<span data-ttu-id="81332-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81332-136">DateTimeOffset</span></span>|<span data-ttu-id="81332-137">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="81332-137">Last time the policy was modified.</span></span> <span data-ttu-id="81332-138">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81332-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81332-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="81332-139">roleScopeTagIds</span></span>|<span data-ttu-id="81332-140">String 集合</span><span class="sxs-lookup"><span data-stu-id="81332-140">String collection</span></span>|<span data-ttu-id="81332-141">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="81332-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="81332-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81332-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81332-143">id</span><span class="sxs-lookup"><span data-stu-id="81332-143">id</span></span>|<span data-ttu-id="81332-144">String</span><span class="sxs-lookup"><span data-stu-id="81332-144">String</span></span>|<span data-ttu-id="81332-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="81332-145">Key of the entity.</span></span> <span data-ttu-id="81332-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81332-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81332-147">version</span><span class="sxs-lookup"><span data-stu-id="81332-147">version</span></span>|<span data-ttu-id="81332-148">String</span><span class="sxs-lookup"><span data-stu-id="81332-148">String</span></span>|<span data-ttu-id="81332-149">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="81332-149">Version of the entity.</span></span> <span data-ttu-id="81332-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81332-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81332-151">customSettings</span><span class="sxs-lookup"><span data-stu-id="81332-151">customSettings</span></span>|<span data-ttu-id="81332-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81332-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="81332-153">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="81332-153">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="81332-154">关系</span><span class="sxs-lookup"><span data-stu-id="81332-154">Relationships</span></span>
<span data-ttu-id="81332-155">无</span><span class="sxs-lookup"><span data-stu-id="81332-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81332-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81332-156">JSON Representation</span></span>
<span data-ttu-id="81332-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81332-157">Here is a JSON representation of the resource.</span></span>
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




