---
title: mobileAppIntentAndState 资源类型
description: MobileApp 意图和给定的设备的安装状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 689945d1e2f7e7a1c33e9bc098dc64ad16472bd5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947244"
---
# <a name="mobileappintentandstate-resource-type"></a><span data-ttu-id="98d9f-103">mobileAppIntentAndState 资源类型</span><span class="sxs-lookup"><span data-stu-id="98d9f-103">mobileAppIntentAndState resource type</span></span>

> <span data-ttu-id="98d9f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="98d9f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98d9f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="98d9f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98d9f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="98d9f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98d9f-107">MobileApp 意图和给定的设备的安装状态。</span><span class="sxs-lookup"><span data-stu-id="98d9f-107">MobileApp Intent and Install State for a given device.</span></span>
## <a name="methods"></a><span data-ttu-id="98d9f-108">方法</span><span class="sxs-lookup"><span data-stu-id="98d9f-108">Methods</span></span>
|<span data-ttu-id="98d9f-109">方法</span><span class="sxs-lookup"><span data-stu-id="98d9f-109">Method</span></span>|<span data-ttu-id="98d9f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="98d9f-110">Return Type</span></span>|<span data-ttu-id="98d9f-111">说明</span><span class="sxs-lookup"><span data-stu-id="98d9f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="98d9f-112">列表 mobileAppIntentAndStates</span><span class="sxs-lookup"><span data-stu-id="98d9f-112">List mobileAppIntentAndStates</span></span>](../api/intune-troubleshooting-mobileappintentandstate-list.md)|<span data-ttu-id="98d9f-113">[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="98d9f-113">[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) collection</span></span>|<span data-ttu-id="98d9f-114">列出属性和[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="98d9f-114">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>|
|[<span data-ttu-id="98d9f-115">获取 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="98d9f-115">Get mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[<span data-ttu-id="98d9f-116">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="98d9f-116">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="98d9f-117">读取属性和[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="98d9f-117">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|
|[<span data-ttu-id="98d9f-118">创建 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="98d9f-118">Create mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[<span data-ttu-id="98d9f-119">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="98d9f-119">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="98d9f-120">创建新的[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="98d9f-120">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|
|[<span data-ttu-id="98d9f-121">删除 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="98d9f-121">Delete mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|<span data-ttu-id="98d9f-122">无</span><span class="sxs-lookup"><span data-stu-id="98d9f-122">None</span></span>|<span data-ttu-id="98d9f-123">删除[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)。</span><span class="sxs-lookup"><span data-stu-id="98d9f-123">Deletes a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>|
|[<span data-ttu-id="98d9f-124">更新 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="98d9f-124">Update mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[<span data-ttu-id="98d9f-125">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="98d9f-125">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="98d9f-126">更新[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="98d9f-126">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="98d9f-127">属性</span><span class="sxs-lookup"><span data-stu-id="98d9f-127">Properties</span></span>
|<span data-ttu-id="98d9f-128">属性</span><span class="sxs-lookup"><span data-stu-id="98d9f-128">Property</span></span>|<span data-ttu-id="98d9f-129">类型</span><span class="sxs-lookup"><span data-stu-id="98d9f-129">Type</span></span>|<span data-ttu-id="98d9f-130">说明</span><span class="sxs-lookup"><span data-stu-id="98d9f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98d9f-131">id</span><span class="sxs-lookup"><span data-stu-id="98d9f-131">id</span></span>|<span data-ttu-id="98d9f-132">String</span><span class="sxs-lookup"><span data-stu-id="98d9f-132">String</span></span>|<span data-ttu-id="98d9f-133">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="98d9f-133">UUID for the object</span></span>|
|<span data-ttu-id="98d9f-134">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="98d9f-134">managedDeviceIdentifier</span></span>|<span data-ttu-id="98d9f-135">String</span><span class="sxs-lookup"><span data-stu-id="98d9f-135">String</span></span>|<span data-ttu-id="98d9f-136">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="98d9f-136">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="98d9f-137">userId</span><span class="sxs-lookup"><span data-stu-id="98d9f-137">userId</span></span>|<span data-ttu-id="98d9f-138">String</span><span class="sxs-lookup"><span data-stu-id="98d9f-138">String</span></span>|<span data-ttu-id="98d9f-139">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="98d9f-139">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="98d9f-140">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="98d9f-140">mobileAppList</span></span>|<span data-ttu-id="98d9f-141">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)集合</span><span class="sxs-lookup"><span data-stu-id="98d9f-141">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="98d9f-142">负载方法和租户的状态的列表。</span><span class="sxs-lookup"><span data-stu-id="98d9f-142">The list of payload intents and states for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98d9f-143">Relationships</span><span class="sxs-lookup"><span data-stu-id="98d9f-143">Relationships</span></span>
<span data-ttu-id="98d9f-144">无</span><span class="sxs-lookup"><span data-stu-id="98d9f-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98d9f-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98d9f-145">JSON Representation</span></span>
<span data-ttu-id="98d9f-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98d9f-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppIntentAndState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "String (identifier)",
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "String",
      "displayName": "String",
      "mobileAppIntent": "String",
      "displayVersion": "String",
      "installState": "String",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "String",
          "minimumOperatingSystemVersion": "String",
          "maximumOperatingSystemVersion": "String"
        }
      ]
    }
  ]
}
```





