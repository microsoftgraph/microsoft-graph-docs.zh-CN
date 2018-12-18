---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
author: tfitzmac
ms.openlocfilehash: ffbbb5758fd8192e5acc5c674caa6f5acecdcf3c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358518"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="039dc-103">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="039dc-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="039dc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="039dc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="039dc-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="039dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="039dc-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="039dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="039dc-107">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="039dc-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="039dc-108">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="039dc-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="039dc-109">方法</span><span class="sxs-lookup"><span data-stu-id="039dc-109">Methods</span></span>
|<span data-ttu-id="039dc-110">方法</span><span class="sxs-lookup"><span data-stu-id="039dc-110">Method</span></span>|<span data-ttu-id="039dc-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="039dc-111">Return Type</span></span>|<span data-ttu-id="039dc-112">说明</span><span class="sxs-lookup"><span data-stu-id="039dc-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="039dc-113">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="039dc-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="039dc-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="039dc-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="039dc-115">列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="039dc-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="039dc-116">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="039dc-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="039dc-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="039dc-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="039dc-118">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="039dc-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="039dc-119">属性</span><span class="sxs-lookup"><span data-stu-id="039dc-119">Properties</span></span>
|<span data-ttu-id="039dc-120">属性</span><span class="sxs-lookup"><span data-stu-id="039dc-120">Property</span></span>|<span data-ttu-id="039dc-121">类型</span><span class="sxs-lookup"><span data-stu-id="039dc-121">Type</span></span>|<span data-ttu-id="039dc-122">说明</span><span class="sxs-lookup"><span data-stu-id="039dc-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="039dc-123">displayName</span><span class="sxs-lookup"><span data-stu-id="039dc-123">displayName</span></span>|<span data-ttu-id="039dc-124">String</span><span class="sxs-lookup"><span data-stu-id="039dc-124">String</span></span>|<span data-ttu-id="039dc-125">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="039dc-125">Policy display name.</span></span> <span data-ttu-id="039dc-126">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="039dc-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="039dc-127">description</span><span class="sxs-lookup"><span data-stu-id="039dc-127">description</span></span>|<span data-ttu-id="039dc-128">String</span><span class="sxs-lookup"><span data-stu-id="039dc-128">String</span></span>|<span data-ttu-id="039dc-129">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="039dc-129">The policy's description.</span></span> <span data-ttu-id="039dc-130">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="039dc-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="039dc-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="039dc-131">createdDateTime</span></span>|<span data-ttu-id="039dc-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="039dc-132">DateTimeOffset</span></span>|<span data-ttu-id="039dc-133">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="039dc-133">The date and time the policy was created.</span></span> <span data-ttu-id="039dc-134">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="039dc-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="039dc-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="039dc-135">lastModifiedDateTime</span></span>|<span data-ttu-id="039dc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="039dc-136">DateTimeOffset</span></span>|<span data-ttu-id="039dc-137">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="039dc-137">Last time the policy was modified.</span></span> <span data-ttu-id="039dc-138">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="039dc-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="039dc-139">id</span><span class="sxs-lookup"><span data-stu-id="039dc-139">id</span></span>|<span data-ttu-id="039dc-140">String</span><span class="sxs-lookup"><span data-stu-id="039dc-140">String</span></span>|<span data-ttu-id="039dc-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="039dc-141">Key of the entity.</span></span> <span data-ttu-id="039dc-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="039dc-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="039dc-143">version</span><span class="sxs-lookup"><span data-stu-id="039dc-143">version</span></span>|<span data-ttu-id="039dc-144">String</span><span class="sxs-lookup"><span data-stu-id="039dc-144">String</span></span>|<span data-ttu-id="039dc-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="039dc-145">Version of the entity.</span></span> <span data-ttu-id="039dc-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="039dc-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="039dc-147">customSettings</span><span class="sxs-lookup"><span data-stu-id="039dc-147">customSettings</span></span>|<span data-ttu-id="039dc-148">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="039dc-148">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="039dc-149">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="039dc-149">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="039dc-150">关系</span><span class="sxs-lookup"><span data-stu-id="039dc-150">Relationships</span></span>
<span data-ttu-id="039dc-151">无</span><span class="sxs-lookup"><span data-stu-id="039dc-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="039dc-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="039dc-152">JSON Representation</span></span>
<span data-ttu-id="039dc-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="039dc-153">Here is a JSON representation of the resource.</span></span>
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





