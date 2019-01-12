---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5571a1c4b3f115280499ead992758a8ff46b2f26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963666"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="81e6c-103">managedAppConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="81e6c-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="81e6c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="81e6c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81e6c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="81e6c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81e6c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="81e6c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81e6c-107">用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。</span><span class="sxs-lookup"><span data-stu-id="81e6c-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="81e6c-108">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81e6c-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="81e6c-109">方法</span><span class="sxs-lookup"><span data-stu-id="81e6c-109">Methods</span></span>
|<span data-ttu-id="81e6c-110">方法</span><span class="sxs-lookup"><span data-stu-id="81e6c-110">Method</span></span>|<span data-ttu-id="81e6c-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="81e6c-111">Return Type</span></span>|<span data-ttu-id="81e6c-112">说明</span><span class="sxs-lookup"><span data-stu-id="81e6c-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81e6c-113">List managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="81e6c-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="81e6c-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81e6c-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="81e6c-115">列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81e6c-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="81e6c-116">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="81e6c-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="81e6c-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="81e6c-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="81e6c-118">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81e6c-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81e6c-119">属性</span><span class="sxs-lookup"><span data-stu-id="81e6c-119">Properties</span></span>
|<span data-ttu-id="81e6c-120">属性</span><span class="sxs-lookup"><span data-stu-id="81e6c-120">Property</span></span>|<span data-ttu-id="81e6c-121">类型</span><span class="sxs-lookup"><span data-stu-id="81e6c-121">Type</span></span>|<span data-ttu-id="81e6c-122">说明</span><span class="sxs-lookup"><span data-stu-id="81e6c-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81e6c-123">displayName</span><span class="sxs-lookup"><span data-stu-id="81e6c-123">displayName</span></span>|<span data-ttu-id="81e6c-124">String</span><span class="sxs-lookup"><span data-stu-id="81e6c-124">String</span></span>|<span data-ttu-id="81e6c-125">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="81e6c-125">Policy display name.</span></span> <span data-ttu-id="81e6c-126">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81e6c-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81e6c-127">description</span><span class="sxs-lookup"><span data-stu-id="81e6c-127">description</span></span>|<span data-ttu-id="81e6c-128">String</span><span class="sxs-lookup"><span data-stu-id="81e6c-128">String</span></span>|<span data-ttu-id="81e6c-129">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="81e6c-129">The policy's description.</span></span> <span data-ttu-id="81e6c-130">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81e6c-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81e6c-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81e6c-131">createdDateTime</span></span>|<span data-ttu-id="81e6c-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81e6c-132">DateTimeOffset</span></span>|<span data-ttu-id="81e6c-133">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="81e6c-133">The date and time the policy was created.</span></span> <span data-ttu-id="81e6c-134">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81e6c-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81e6c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81e6c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="81e6c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81e6c-136">DateTimeOffset</span></span>|<span data-ttu-id="81e6c-137">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="81e6c-137">Last time the policy was modified.</span></span> <span data-ttu-id="81e6c-138">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81e6c-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81e6c-139">id</span><span class="sxs-lookup"><span data-stu-id="81e6c-139">id</span></span>|<span data-ttu-id="81e6c-140">String</span><span class="sxs-lookup"><span data-stu-id="81e6c-140">String</span></span>|<span data-ttu-id="81e6c-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="81e6c-141">Key of the entity.</span></span> <span data-ttu-id="81e6c-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81e6c-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81e6c-143">version</span><span class="sxs-lookup"><span data-stu-id="81e6c-143">version</span></span>|<span data-ttu-id="81e6c-144">String</span><span class="sxs-lookup"><span data-stu-id="81e6c-144">String</span></span>|<span data-ttu-id="81e6c-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="81e6c-145">Version of the entity.</span></span> <span data-ttu-id="81e6c-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81e6c-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81e6c-147">customSettings</span><span class="sxs-lookup"><span data-stu-id="81e6c-147">customSettings</span></span>|<span data-ttu-id="81e6c-148">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81e6c-148">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="81e6c-149">一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变</span><span class="sxs-lookup"><span data-stu-id="81e6c-149">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="81e6c-150">关系</span><span class="sxs-lookup"><span data-stu-id="81e6c-150">Relationships</span></span>
<span data-ttu-id="81e6c-151">无</span><span class="sxs-lookup"><span data-stu-id="81e6c-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81e6c-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81e6c-152">JSON Representation</span></span>
<span data-ttu-id="81e6c-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81e6c-153">Here is a JSON representation of the resource.</span></span>
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





