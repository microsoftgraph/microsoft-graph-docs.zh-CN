---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2b3acf921f76e34e21427364ef84d1647cc7d0f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861318"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="4c6d7-103">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c6d7-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="4c6d7-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4c6d7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c6d7-105">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="4c6d7-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="4c6d7-106">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4c6d7-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="4c6d7-107">方法</span><span class="sxs-lookup"><span data-stu-id="4c6d7-107">Methods</span></span>
|<span data-ttu-id="4c6d7-108">方法</span><span class="sxs-lookup"><span data-stu-id="4c6d7-108">Method</span></span>|<span data-ttu-id="4c6d7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4c6d7-109">Return Type</span></span>|<span data-ttu-id="4c6d7-110">说明</span><span class="sxs-lookup"><span data-stu-id="4c6d7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4c6d7-111">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="4c6d7-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="4c6d7-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c6d7-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="4c6d7-113">列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4c6d7-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="4c6d7-114">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c6d7-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="4c6d7-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c6d7-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="4c6d7-116">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4c6d7-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4c6d7-117">属性</span><span class="sxs-lookup"><span data-stu-id="4c6d7-117">Properties</span></span>
|<span data-ttu-id="4c6d7-118">属性</span><span class="sxs-lookup"><span data-stu-id="4c6d7-118">Property</span></span>|<span data-ttu-id="4c6d7-119">类型</span><span class="sxs-lookup"><span data-stu-id="4c6d7-119">Type</span></span>|<span data-ttu-id="4c6d7-120">说明</span><span class="sxs-lookup"><span data-stu-id="4c6d7-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c6d7-121">displayName</span><span class="sxs-lookup"><span data-stu-id="4c6d7-121">displayName</span></span>|<span data-ttu-id="4c6d7-122">String</span><span class="sxs-lookup"><span data-stu-id="4c6d7-122">String</span></span>|<span data-ttu-id="4c6d7-123">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="4c6d7-123">Policy display name.</span></span> <span data-ttu-id="4c6d7-124">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4c6d7-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4c6d7-125">description</span><span class="sxs-lookup"><span data-stu-id="4c6d7-125">description</span></span>|<span data-ttu-id="4c6d7-126">String</span><span class="sxs-lookup"><span data-stu-id="4c6d7-126">String</span></span>|<span data-ttu-id="4c6d7-127">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="4c6d7-127">The policy's description.</span></span> <span data-ttu-id="4c6d7-128">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4c6d7-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4c6d7-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c6d7-129">createdDateTime</span></span>|<span data-ttu-id="4c6d7-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c6d7-130">DateTimeOffset</span></span>|<span data-ttu-id="4c6d7-131">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4c6d7-131">The date and time the policy was created.</span></span> <span data-ttu-id="4c6d7-132">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4c6d7-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4c6d7-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c6d7-133">lastModifiedDateTime</span></span>|<span data-ttu-id="4c6d7-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c6d7-134">DateTimeOffset</span></span>|<span data-ttu-id="4c6d7-135">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="4c6d7-135">Last time the policy was modified.</span></span> <span data-ttu-id="4c6d7-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4c6d7-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4c6d7-137">id</span><span class="sxs-lookup"><span data-stu-id="4c6d7-137">id</span></span>|<span data-ttu-id="4c6d7-138">String</span><span class="sxs-lookup"><span data-stu-id="4c6d7-138">String</span></span>|<span data-ttu-id="4c6d7-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4c6d7-139">Key of the entity.</span></span> <span data-ttu-id="4c6d7-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4c6d7-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4c6d7-141">version</span><span class="sxs-lookup"><span data-stu-id="4c6d7-141">version</span></span>|<span data-ttu-id="4c6d7-142">String</span><span class="sxs-lookup"><span data-stu-id="4c6d7-142">String</span></span>|<span data-ttu-id="4c6d7-143">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="4c6d7-143">Version of the entity.</span></span> <span data-ttu-id="4c6d7-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4c6d7-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4c6d7-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="4c6d7-145">customSettings</span></span>|<span data-ttu-id="4c6d7-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c6d7-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="4c6d7-147">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="4c6d7-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c6d7-148">关系</span><span class="sxs-lookup"><span data-stu-id="4c6d7-148">Relationships</span></span>
<span data-ttu-id="4c6d7-149">无</span><span class="sxs-lookup"><span data-stu-id="4c6d7-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4c6d7-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c6d7-150">JSON Representation</span></span>
<span data-ttu-id="4c6d7-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c6d7-151">Here is a JSON representation of the resource.</span></span>
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



