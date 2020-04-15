---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e2b2d74da530ea6a5479efc2f98c4b8afa68e02f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445807"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="14457-103">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="14457-103">managedAppConfiguration resource type</span></span>

<span data-ttu-id="14457-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14457-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14457-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14457-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14457-106">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="14457-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="14457-107">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="14457-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="14457-108">方法</span><span class="sxs-lookup"><span data-stu-id="14457-108">Methods</span></span>
|<span data-ttu-id="14457-109">方法</span><span class="sxs-lookup"><span data-stu-id="14457-109">Method</span></span>|<span data-ttu-id="14457-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="14457-110">Return Type</span></span>|<span data-ttu-id="14457-111">说明</span><span class="sxs-lookup"><span data-stu-id="14457-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="14457-112">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="14457-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="14457-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14457-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="14457-114">列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14457-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="14457-115">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="14457-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="14457-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="14457-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="14457-117">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14457-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="14457-118">属性</span><span class="sxs-lookup"><span data-stu-id="14457-118">Properties</span></span>
|<span data-ttu-id="14457-119">属性</span><span class="sxs-lookup"><span data-stu-id="14457-119">Property</span></span>|<span data-ttu-id="14457-120">类型</span><span class="sxs-lookup"><span data-stu-id="14457-120">Type</span></span>|<span data-ttu-id="14457-121">说明</span><span class="sxs-lookup"><span data-stu-id="14457-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14457-122">displayName</span><span class="sxs-lookup"><span data-stu-id="14457-122">displayName</span></span>|<span data-ttu-id="14457-123">字符串</span><span class="sxs-lookup"><span data-stu-id="14457-123">String</span></span>|<span data-ttu-id="14457-124">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="14457-124">Policy display name.</span></span> <span data-ttu-id="14457-125">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="14457-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="14457-126">description</span><span class="sxs-lookup"><span data-stu-id="14457-126">description</span></span>|<span data-ttu-id="14457-127">String</span><span class="sxs-lookup"><span data-stu-id="14457-127">String</span></span>|<span data-ttu-id="14457-128">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="14457-128">The policy's description.</span></span> <span data-ttu-id="14457-129">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="14457-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="14457-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14457-130">createdDateTime</span></span>|<span data-ttu-id="14457-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14457-131">DateTimeOffset</span></span>|<span data-ttu-id="14457-132">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="14457-132">The date and time the policy was created.</span></span> <span data-ttu-id="14457-133">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="14457-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="14457-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14457-134">lastModifiedDateTime</span></span>|<span data-ttu-id="14457-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14457-135">DateTimeOffset</span></span>|<span data-ttu-id="14457-136">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="14457-136">Last time the policy was modified.</span></span> <span data-ttu-id="14457-137">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="14457-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="14457-138">id</span><span class="sxs-lookup"><span data-stu-id="14457-138">id</span></span>|<span data-ttu-id="14457-139">字符串</span><span class="sxs-lookup"><span data-stu-id="14457-139">String</span></span>|<span data-ttu-id="14457-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="14457-140">Key of the entity.</span></span> <span data-ttu-id="14457-141">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="14457-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="14457-142">version</span><span class="sxs-lookup"><span data-stu-id="14457-142">version</span></span>|<span data-ttu-id="14457-143">String</span><span class="sxs-lookup"><span data-stu-id="14457-143">String</span></span>|<span data-ttu-id="14457-144">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="14457-144">Version of the entity.</span></span> <span data-ttu-id="14457-145">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="14457-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="14457-146">customSettings</span><span class="sxs-lookup"><span data-stu-id="14457-146">customSettings</span></span>|<span data-ttu-id="14457-147">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14457-147">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="14457-148">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="14457-148">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="14457-149">关系</span><span class="sxs-lookup"><span data-stu-id="14457-149">Relationships</span></span>
<span data-ttu-id="14457-150">无</span><span class="sxs-lookup"><span data-stu-id="14457-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14457-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14457-151">JSON Representation</span></span>
<span data-ttu-id="14457-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14457-152">Here is a JSON representation of the resource.</span></span>
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







