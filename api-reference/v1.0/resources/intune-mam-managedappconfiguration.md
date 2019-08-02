---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 86e1e5a2a768a9356ae580c4ceb01360a243c5cf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038029"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="6c283-103">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c283-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="6c283-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c283-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c283-105">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="6c283-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="6c283-106">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c283-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6c283-107">方法</span><span class="sxs-lookup"><span data-stu-id="6c283-107">Methods</span></span>
|<span data-ttu-id="6c283-108">方法</span><span class="sxs-lookup"><span data-stu-id="6c283-108">Method</span></span>|<span data-ttu-id="6c283-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="6c283-109">Return Type</span></span>|<span data-ttu-id="6c283-110">说明</span><span class="sxs-lookup"><span data-stu-id="6c283-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c283-111">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="6c283-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="6c283-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c283-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="6c283-113">列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6c283-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="6c283-114">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c283-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="6c283-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c283-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="6c283-116">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6c283-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c283-117">属性</span><span class="sxs-lookup"><span data-stu-id="6c283-117">Properties</span></span>
|<span data-ttu-id="6c283-118">属性</span><span class="sxs-lookup"><span data-stu-id="6c283-118">Property</span></span>|<span data-ttu-id="6c283-119">类型</span><span class="sxs-lookup"><span data-stu-id="6c283-119">Type</span></span>|<span data-ttu-id="6c283-120">说明</span><span class="sxs-lookup"><span data-stu-id="6c283-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c283-121">displayName</span><span class="sxs-lookup"><span data-stu-id="6c283-121">displayName</span></span>|<span data-ttu-id="6c283-122">字符串</span><span class="sxs-lookup"><span data-stu-id="6c283-122">String</span></span>|<span data-ttu-id="6c283-123">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="6c283-123">Policy display name.</span></span> <span data-ttu-id="6c283-124">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c283-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6c283-125">说明</span><span class="sxs-lookup"><span data-stu-id="6c283-125">description</span></span>|<span data-ttu-id="6c283-126">String</span><span class="sxs-lookup"><span data-stu-id="6c283-126">String</span></span>|<span data-ttu-id="6c283-127">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="6c283-127">The policy's description.</span></span> <span data-ttu-id="6c283-128">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c283-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6c283-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c283-129">createdDateTime</span></span>|<span data-ttu-id="6c283-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c283-130">DateTimeOffset</span></span>|<span data-ttu-id="6c283-131">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6c283-131">The date and time the policy was created.</span></span> <span data-ttu-id="6c283-132">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c283-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6c283-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c283-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6c283-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c283-134">DateTimeOffset</span></span>|<span data-ttu-id="6c283-135">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="6c283-135">Last time the policy was modified.</span></span> <span data-ttu-id="6c283-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c283-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6c283-137">id</span><span class="sxs-lookup"><span data-stu-id="6c283-137">id</span></span>|<span data-ttu-id="6c283-138">字符串</span><span class="sxs-lookup"><span data-stu-id="6c283-138">String</span></span>|<span data-ttu-id="6c283-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6c283-139">Key of the entity.</span></span> <span data-ttu-id="6c283-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c283-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6c283-141">version</span><span class="sxs-lookup"><span data-stu-id="6c283-141">version</span></span>|<span data-ttu-id="6c283-142">String</span><span class="sxs-lookup"><span data-stu-id="6c283-142">String</span></span>|<span data-ttu-id="6c283-143">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="6c283-143">Version of the entity.</span></span> <span data-ttu-id="6c283-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c283-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6c283-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="6c283-145">customSettings</span></span>|<span data-ttu-id="6c283-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c283-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6c283-147">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="6c283-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c283-148">关系</span><span class="sxs-lookup"><span data-stu-id="6c283-148">Relationships</span></span>
<span data-ttu-id="6c283-149">无</span><span class="sxs-lookup"><span data-stu-id="6c283-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c283-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c283-150">JSON Representation</span></span>
<span data-ttu-id="6c283-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c283-151">Here is a JSON representation of the resource.</span></span>
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



