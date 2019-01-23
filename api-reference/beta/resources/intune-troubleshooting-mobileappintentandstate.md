---
title: mobileAppIntentAndState 资源类型
description: MobileApp 意图和给定的设备的安装状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 01792d30bdf821d4dd0795926e116bdc12b95ad9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402403"
---
# <a name="mobileappintentandstate-resource-type"></a><span data-ttu-id="e5513-103">mobileAppIntentAndState 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5513-103">mobileAppIntentAndState resource type</span></span>

> <span data-ttu-id="e5513-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e5513-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e5513-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e5513-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5513-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5513-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5513-107">MobileApp 意图和给定的设备的安装状态。</span><span class="sxs-lookup"><span data-stu-id="e5513-107">MobileApp Intent and Install State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="e5513-108">方法</span><span class="sxs-lookup"><span data-stu-id="e5513-108">Methods</span></span>
|<span data-ttu-id="e5513-109">方法</span><span class="sxs-lookup"><span data-stu-id="e5513-109">Method</span></span>|<span data-ttu-id="e5513-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e5513-110">Return Type</span></span>|<span data-ttu-id="e5513-111">说明</span><span class="sxs-lookup"><span data-stu-id="e5513-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e5513-112">列表 mobileAppIntentAndStates</span><span class="sxs-lookup"><span data-stu-id="e5513-112">List mobileAppIntentAndStates</span></span>](../api/intune-troubleshooting-mobileappintentandstate-list.md)|<span data-ttu-id="e5513-113">[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="e5513-113">[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) collection</span></span>|<span data-ttu-id="e5513-114">列出属性和[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="e5513-114">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>|
|[<span data-ttu-id="e5513-115">获取 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="e5513-115">Get mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[<span data-ttu-id="e5513-116">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="e5513-116">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="e5513-117">读取属性和[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="e5513-117">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|
|[<span data-ttu-id="e5513-118">创建 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="e5513-118">Create mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[<span data-ttu-id="e5513-119">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="e5513-119">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="e5513-120">创建新的[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e5513-120">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|
|[<span data-ttu-id="e5513-121">删除 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="e5513-121">Delete mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|<span data-ttu-id="e5513-122">无</span><span class="sxs-lookup"><span data-stu-id="e5513-122">None</span></span>|<span data-ttu-id="e5513-123">删除[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)。</span><span class="sxs-lookup"><span data-stu-id="e5513-123">Deletes a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>|
|[<span data-ttu-id="e5513-124">更新 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="e5513-124">Update mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[<span data-ttu-id="e5513-125">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="e5513-125">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="e5513-126">更新[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e5513-126">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5513-127">属性</span><span class="sxs-lookup"><span data-stu-id="e5513-127">Properties</span></span>
|<span data-ttu-id="e5513-128">属性</span><span class="sxs-lookup"><span data-stu-id="e5513-128">Property</span></span>|<span data-ttu-id="e5513-129">类型</span><span class="sxs-lookup"><span data-stu-id="e5513-129">Type</span></span>|<span data-ttu-id="e5513-130">说明</span><span class="sxs-lookup"><span data-stu-id="e5513-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5513-131">id</span><span class="sxs-lookup"><span data-stu-id="e5513-131">id</span></span>|<span data-ttu-id="e5513-132">String</span><span class="sxs-lookup"><span data-stu-id="e5513-132">String</span></span>|<span data-ttu-id="e5513-133">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="e5513-133">UUID for the object</span></span>|
|<span data-ttu-id="e5513-134">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e5513-134">managedDeviceIdentifier</span></span>|<span data-ttu-id="e5513-135">String</span><span class="sxs-lookup"><span data-stu-id="e5513-135">String</span></span>|<span data-ttu-id="e5513-136">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="e5513-136">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="e5513-137">userId</span><span class="sxs-lookup"><span data-stu-id="e5513-137">userId</span></span>|<span data-ttu-id="e5513-138">String</span><span class="sxs-lookup"><span data-stu-id="e5513-138">String</span></span>|<span data-ttu-id="e5513-139">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="e5513-139">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="e5513-140">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="e5513-140">mobileAppList</span></span>|<span data-ttu-id="e5513-141">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)集合</span><span class="sxs-lookup"><span data-stu-id="e5513-141">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="e5513-142">负载方法和租户的状态的列表。</span><span class="sxs-lookup"><span data-stu-id="e5513-142">The list of payload intents and states for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5513-143">关系</span><span class="sxs-lookup"><span data-stu-id="e5513-143">Relationships</span></span>
<span data-ttu-id="e5513-144">无</span><span class="sxs-lookup"><span data-stu-id="e5513-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5513-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5513-145">JSON Representation</span></span>
<span data-ttu-id="e5513-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5513-146">Here is a JSON representation of the resource.</span></span>
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




