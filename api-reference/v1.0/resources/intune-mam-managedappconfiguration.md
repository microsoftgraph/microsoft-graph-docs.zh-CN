---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86c6ecdcad64ae38887370101f96106a9b3aa816
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250766"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="da687-103">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="da687-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="da687-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da687-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da687-105">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="da687-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="da687-106">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="da687-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="da687-107">方法</span><span class="sxs-lookup"><span data-stu-id="da687-107">Methods</span></span>
|<span data-ttu-id="da687-108">方法</span><span class="sxs-lookup"><span data-stu-id="da687-108">Method</span></span>|<span data-ttu-id="da687-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="da687-109">Return Type</span></span>|<span data-ttu-id="da687-110">说明</span><span class="sxs-lookup"><span data-stu-id="da687-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="da687-111">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="da687-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="da687-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="da687-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="da687-113">列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="da687-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="da687-114">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="da687-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="da687-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="da687-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="da687-116">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="da687-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="da687-117">属性</span><span class="sxs-lookup"><span data-stu-id="da687-117">Properties</span></span>
|<span data-ttu-id="da687-118">属性</span><span class="sxs-lookup"><span data-stu-id="da687-118">Property</span></span>|<span data-ttu-id="da687-119">类型</span><span class="sxs-lookup"><span data-stu-id="da687-119">Type</span></span>|<span data-ttu-id="da687-120">说明</span><span class="sxs-lookup"><span data-stu-id="da687-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da687-121">displayName</span><span class="sxs-lookup"><span data-stu-id="da687-121">displayName</span></span>|<span data-ttu-id="da687-122">String</span><span class="sxs-lookup"><span data-stu-id="da687-122">String</span></span>|<span data-ttu-id="da687-123">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="da687-123">Policy display name.</span></span> <span data-ttu-id="da687-124">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="da687-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="da687-125">description</span><span class="sxs-lookup"><span data-stu-id="da687-125">description</span></span>|<span data-ttu-id="da687-126">String</span><span class="sxs-lookup"><span data-stu-id="da687-126">String</span></span>|<span data-ttu-id="da687-127">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="da687-127">The policy's description.</span></span> <span data-ttu-id="da687-128">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="da687-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="da687-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da687-129">createdDateTime</span></span>|<span data-ttu-id="da687-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da687-130">DateTimeOffset</span></span>|<span data-ttu-id="da687-131">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="da687-131">The date and time the policy was created.</span></span> <span data-ttu-id="da687-132">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="da687-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="da687-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da687-133">lastModifiedDateTime</span></span>|<span data-ttu-id="da687-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da687-134">DateTimeOffset</span></span>|<span data-ttu-id="da687-135">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="da687-135">Last time the policy was modified.</span></span> <span data-ttu-id="da687-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="da687-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="da687-137">id</span><span class="sxs-lookup"><span data-stu-id="da687-137">id</span></span>|<span data-ttu-id="da687-138">字符串</span><span class="sxs-lookup"><span data-stu-id="da687-138">String</span></span>|<span data-ttu-id="da687-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="da687-139">Key of the entity.</span></span> <span data-ttu-id="da687-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="da687-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="da687-141">version</span><span class="sxs-lookup"><span data-stu-id="da687-141">version</span></span>|<span data-ttu-id="da687-142">String</span><span class="sxs-lookup"><span data-stu-id="da687-142">String</span></span>|<span data-ttu-id="da687-143">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="da687-143">Version of the entity.</span></span> <span data-ttu-id="da687-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="da687-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="da687-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="da687-145">customSettings</span></span>|<span data-ttu-id="da687-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="da687-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="da687-147">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="da687-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="da687-148">关系</span><span class="sxs-lookup"><span data-stu-id="da687-148">Relationships</span></span>
<span data-ttu-id="da687-149">无</span><span class="sxs-lookup"><span data-stu-id="da687-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da687-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da687-150">JSON Representation</span></span>
<span data-ttu-id="da687-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da687-151">Here is a JSON representation of the resource.</span></span>
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



