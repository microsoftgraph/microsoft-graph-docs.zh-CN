---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cad1606def61db9f185aba6804fdb546264e1b1a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267059"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="07942-103">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="07942-103">managedAppConfiguration resource type</span></span>

<span data-ttu-id="07942-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07942-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07942-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="07942-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07942-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07942-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07942-107">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="07942-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="07942-108">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="07942-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="07942-109">方法</span><span class="sxs-lookup"><span data-stu-id="07942-109">Methods</span></span>
|<span data-ttu-id="07942-110">方法</span><span class="sxs-lookup"><span data-stu-id="07942-110">Method</span></span>|<span data-ttu-id="07942-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="07942-111">Return Type</span></span>|<span data-ttu-id="07942-112">说明</span><span class="sxs-lookup"><span data-stu-id="07942-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="07942-113">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="07942-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="07942-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07942-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="07942-115">列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="07942-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="07942-116">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="07942-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="07942-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="07942-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="07942-118">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="07942-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="07942-119">属性</span><span class="sxs-lookup"><span data-stu-id="07942-119">Properties</span></span>
|<span data-ttu-id="07942-120">属性</span><span class="sxs-lookup"><span data-stu-id="07942-120">Property</span></span>|<span data-ttu-id="07942-121">类型</span><span class="sxs-lookup"><span data-stu-id="07942-121">Type</span></span>|<span data-ttu-id="07942-122">说明</span><span class="sxs-lookup"><span data-stu-id="07942-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07942-123">displayName</span><span class="sxs-lookup"><span data-stu-id="07942-123">displayName</span></span>|<span data-ttu-id="07942-124">字符串</span><span class="sxs-lookup"><span data-stu-id="07942-124">String</span></span>|<span data-ttu-id="07942-125">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="07942-125">Policy display name.</span></span> <span data-ttu-id="07942-126">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="07942-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="07942-127">description</span><span class="sxs-lookup"><span data-stu-id="07942-127">description</span></span>|<span data-ttu-id="07942-128">字符串</span><span class="sxs-lookup"><span data-stu-id="07942-128">String</span></span>|<span data-ttu-id="07942-129">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="07942-129">The policy's description.</span></span> <span data-ttu-id="07942-130">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="07942-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="07942-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07942-131">createdDateTime</span></span>|<span data-ttu-id="07942-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07942-132">DateTimeOffset</span></span>|<span data-ttu-id="07942-133">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="07942-133">The date and time the policy was created.</span></span> <span data-ttu-id="07942-134">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="07942-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="07942-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07942-135">lastModifiedDateTime</span></span>|<span data-ttu-id="07942-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07942-136">DateTimeOffset</span></span>|<span data-ttu-id="07942-137">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="07942-137">Last time the policy was modified.</span></span> <span data-ttu-id="07942-138">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="07942-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="07942-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="07942-139">roleScopeTagIds</span></span>|<span data-ttu-id="07942-140">String 集合</span><span class="sxs-lookup"><span data-stu-id="07942-140">String collection</span></span>|<span data-ttu-id="07942-141">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="07942-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="07942-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="07942-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="07942-143">id</span><span class="sxs-lookup"><span data-stu-id="07942-143">id</span></span>|<span data-ttu-id="07942-144">字符串</span><span class="sxs-lookup"><span data-stu-id="07942-144">String</span></span>|<span data-ttu-id="07942-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="07942-145">Key of the entity.</span></span> <span data-ttu-id="07942-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="07942-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="07942-147">version</span><span class="sxs-lookup"><span data-stu-id="07942-147">version</span></span>|<span data-ttu-id="07942-148">String</span><span class="sxs-lookup"><span data-stu-id="07942-148">String</span></span>|<span data-ttu-id="07942-149">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="07942-149">Version of the entity.</span></span> <span data-ttu-id="07942-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="07942-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="07942-151">customSettings</span><span class="sxs-lookup"><span data-stu-id="07942-151">customSettings</span></span>|<span data-ttu-id="07942-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07942-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="07942-153">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="07942-153">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="07942-154">关系</span><span class="sxs-lookup"><span data-stu-id="07942-154">Relationships</span></span>
<span data-ttu-id="07942-155">无</span><span class="sxs-lookup"><span data-stu-id="07942-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07942-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07942-156">JSON Representation</span></span>
<span data-ttu-id="07942-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07942-157">Here is a JSON representation of the resource.</span></span>
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




