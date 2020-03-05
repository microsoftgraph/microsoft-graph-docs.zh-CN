---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60ee8156773db386d5ad8496bf037984005dc5bb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448429"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="99ae6-103">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="99ae6-103">managedAppConfiguration resource type</span></span>

<span data-ttu-id="99ae6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="99ae6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99ae6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99ae6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99ae6-106">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="99ae6-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="99ae6-107">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="99ae6-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="99ae6-108">方法</span><span class="sxs-lookup"><span data-stu-id="99ae6-108">Methods</span></span>
|<span data-ttu-id="99ae6-109">方法</span><span class="sxs-lookup"><span data-stu-id="99ae6-109">Method</span></span>|<span data-ttu-id="99ae6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="99ae6-110">Return Type</span></span>|<span data-ttu-id="99ae6-111">说明</span><span class="sxs-lookup"><span data-stu-id="99ae6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="99ae6-112">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="99ae6-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="99ae6-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="99ae6-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="99ae6-114">列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="99ae6-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="99ae6-115">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="99ae6-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="99ae6-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="99ae6-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="99ae6-117">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="99ae6-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="99ae6-118">属性</span><span class="sxs-lookup"><span data-stu-id="99ae6-118">Properties</span></span>
|<span data-ttu-id="99ae6-119">属性</span><span class="sxs-lookup"><span data-stu-id="99ae6-119">Property</span></span>|<span data-ttu-id="99ae6-120">类型</span><span class="sxs-lookup"><span data-stu-id="99ae6-120">Type</span></span>|<span data-ttu-id="99ae6-121">说明</span><span class="sxs-lookup"><span data-stu-id="99ae6-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99ae6-122">displayName</span><span class="sxs-lookup"><span data-stu-id="99ae6-122">displayName</span></span>|<span data-ttu-id="99ae6-123">字符串</span><span class="sxs-lookup"><span data-stu-id="99ae6-123">String</span></span>|<span data-ttu-id="99ae6-124">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="99ae6-124">Policy display name.</span></span> <span data-ttu-id="99ae6-125">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="99ae6-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="99ae6-126">说明</span><span class="sxs-lookup"><span data-stu-id="99ae6-126">description</span></span>|<span data-ttu-id="99ae6-127">String</span><span class="sxs-lookup"><span data-stu-id="99ae6-127">String</span></span>|<span data-ttu-id="99ae6-128">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="99ae6-128">The policy's description.</span></span> <span data-ttu-id="99ae6-129">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="99ae6-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="99ae6-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99ae6-130">createdDateTime</span></span>|<span data-ttu-id="99ae6-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99ae6-131">DateTimeOffset</span></span>|<span data-ttu-id="99ae6-132">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="99ae6-132">The date and time the policy was created.</span></span> <span data-ttu-id="99ae6-133">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="99ae6-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="99ae6-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99ae6-134">lastModifiedDateTime</span></span>|<span data-ttu-id="99ae6-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99ae6-135">DateTimeOffset</span></span>|<span data-ttu-id="99ae6-136">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="99ae6-136">Last time the policy was modified.</span></span> <span data-ttu-id="99ae6-137">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="99ae6-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="99ae6-138">id</span><span class="sxs-lookup"><span data-stu-id="99ae6-138">id</span></span>|<span data-ttu-id="99ae6-139">字符串</span><span class="sxs-lookup"><span data-stu-id="99ae6-139">String</span></span>|<span data-ttu-id="99ae6-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="99ae6-140">Key of the entity.</span></span> <span data-ttu-id="99ae6-141">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="99ae6-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="99ae6-142">version</span><span class="sxs-lookup"><span data-stu-id="99ae6-142">version</span></span>|<span data-ttu-id="99ae6-143">String</span><span class="sxs-lookup"><span data-stu-id="99ae6-143">String</span></span>|<span data-ttu-id="99ae6-144">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="99ae6-144">Version of the entity.</span></span> <span data-ttu-id="99ae6-145">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="99ae6-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="99ae6-146">customSettings</span><span class="sxs-lookup"><span data-stu-id="99ae6-146">customSettings</span></span>|<span data-ttu-id="99ae6-147">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="99ae6-147">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="99ae6-148">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="99ae6-148">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="99ae6-149">关系</span><span class="sxs-lookup"><span data-stu-id="99ae6-149">Relationships</span></span>
<span data-ttu-id="99ae6-150">无</span><span class="sxs-lookup"><span data-stu-id="99ae6-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99ae6-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99ae6-151">JSON Representation</span></span>
<span data-ttu-id="99ae6-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99ae6-152">Here is a JSON representation of the resource.</span></span>
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




