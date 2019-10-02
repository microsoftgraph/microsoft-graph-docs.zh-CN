---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a133983c7bc58b4e0abacbfa336280a54c373df5
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356392"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="56d75-103">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="56d75-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="56d75-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56d75-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56d75-105">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="56d75-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="56d75-106">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56d75-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="56d75-107">方法</span><span class="sxs-lookup"><span data-stu-id="56d75-107">Methods</span></span>
|<span data-ttu-id="56d75-108">方法</span><span class="sxs-lookup"><span data-stu-id="56d75-108">Method</span></span>|<span data-ttu-id="56d75-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="56d75-109">Return Type</span></span>|<span data-ttu-id="56d75-110">说明</span><span class="sxs-lookup"><span data-stu-id="56d75-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="56d75-111">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="56d75-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="56d75-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56d75-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="56d75-113">列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56d75-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="56d75-114">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="56d75-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="56d75-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="56d75-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="56d75-116">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56d75-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="56d75-117">属性</span><span class="sxs-lookup"><span data-stu-id="56d75-117">Properties</span></span>
|<span data-ttu-id="56d75-118">属性</span><span class="sxs-lookup"><span data-stu-id="56d75-118">Property</span></span>|<span data-ttu-id="56d75-119">类型</span><span class="sxs-lookup"><span data-stu-id="56d75-119">Type</span></span>|<span data-ttu-id="56d75-120">说明</span><span class="sxs-lookup"><span data-stu-id="56d75-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56d75-121">displayName</span><span class="sxs-lookup"><span data-stu-id="56d75-121">displayName</span></span>|<span data-ttu-id="56d75-122">字符串</span><span class="sxs-lookup"><span data-stu-id="56d75-122">String</span></span>|<span data-ttu-id="56d75-123">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="56d75-123">Policy display name.</span></span> <span data-ttu-id="56d75-124">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56d75-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="56d75-125">说明</span><span class="sxs-lookup"><span data-stu-id="56d75-125">description</span></span>|<span data-ttu-id="56d75-126">String</span><span class="sxs-lookup"><span data-stu-id="56d75-126">String</span></span>|<span data-ttu-id="56d75-127">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="56d75-127">The policy's description.</span></span> <span data-ttu-id="56d75-128">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56d75-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="56d75-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56d75-129">createdDateTime</span></span>|<span data-ttu-id="56d75-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56d75-130">DateTimeOffset</span></span>|<span data-ttu-id="56d75-131">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="56d75-131">The date and time the policy was created.</span></span> <span data-ttu-id="56d75-132">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56d75-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="56d75-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56d75-133">lastModifiedDateTime</span></span>|<span data-ttu-id="56d75-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56d75-134">DateTimeOffset</span></span>|<span data-ttu-id="56d75-135">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="56d75-135">Last time the policy was modified.</span></span> <span data-ttu-id="56d75-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56d75-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="56d75-137">id</span><span class="sxs-lookup"><span data-stu-id="56d75-137">id</span></span>|<span data-ttu-id="56d75-138">字符串</span><span class="sxs-lookup"><span data-stu-id="56d75-138">String</span></span>|<span data-ttu-id="56d75-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="56d75-139">Key of the entity.</span></span> <span data-ttu-id="56d75-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56d75-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="56d75-141">version</span><span class="sxs-lookup"><span data-stu-id="56d75-141">version</span></span>|<span data-ttu-id="56d75-142">String</span><span class="sxs-lookup"><span data-stu-id="56d75-142">String</span></span>|<span data-ttu-id="56d75-143">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="56d75-143">Version of the entity.</span></span> <span data-ttu-id="56d75-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56d75-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="56d75-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="56d75-145">customSettings</span></span>|<span data-ttu-id="56d75-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56d75-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="56d75-147">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="56d75-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="56d75-148">关系</span><span class="sxs-lookup"><span data-stu-id="56d75-148">Relationships</span></span>
<span data-ttu-id="56d75-149">无</span><span class="sxs-lookup"><span data-stu-id="56d75-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56d75-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56d75-150">JSON Representation</span></span>
<span data-ttu-id="56d75-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56d75-151">Here is a JSON representation of the resource.</span></span>
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




