---
title: mobileAppIntentAndState 资源类型
description: 给定设备的 MobileApp 意图和安装状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aff331007171f611ed96cadeee055f412f391e6b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163873"
---
# <a name="mobileappintentandstate-resource-type"></a><span data-ttu-id="06cd2-103">mobileAppIntentAndState 资源类型</span><span class="sxs-lookup"><span data-stu-id="06cd2-103">mobileAppIntentAndState resource type</span></span>

> <span data-ttu-id="06cd2-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="06cd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06cd2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06cd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06cd2-106">给定设备的 MobileApp 意图和安装状态。</span><span class="sxs-lookup"><span data-stu-id="06cd2-106">MobileApp Intent and Install State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="06cd2-107">方法</span><span class="sxs-lookup"><span data-stu-id="06cd2-107">Methods</span></span>
|<span data-ttu-id="06cd2-108">方法</span><span class="sxs-lookup"><span data-stu-id="06cd2-108">Method</span></span>|<span data-ttu-id="06cd2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="06cd2-109">Return Type</span></span>|<span data-ttu-id="06cd2-110">说明</span><span class="sxs-lookup"><span data-stu-id="06cd2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06cd2-111">列出 mobileAppIntentAndStates</span><span class="sxs-lookup"><span data-stu-id="06cd2-111">List mobileAppIntentAndStates</span></span>](../api/intune-troubleshooting-mobileappintentandstate-list.md)|<span data-ttu-id="06cd2-112">[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="06cd2-112">[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) collection</span></span>|<span data-ttu-id="06cd2-113">列出[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06cd2-113">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>|
|[<span data-ttu-id="06cd2-114">获取 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="06cd2-114">Get mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[<span data-ttu-id="06cd2-115">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="06cd2-115">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="06cd2-116">读取[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06cd2-116">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|
|[<span data-ttu-id="06cd2-117">创建 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="06cd2-117">Create mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[<span data-ttu-id="06cd2-118">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="06cd2-118">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="06cd2-119">创建新的[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="06cd2-119">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|
|[<span data-ttu-id="06cd2-120">删除 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="06cd2-120">Delete mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|<span data-ttu-id="06cd2-121">无</span><span class="sxs-lookup"><span data-stu-id="06cd2-121">None</span></span>|<span data-ttu-id="06cd2-122">删除[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)。</span><span class="sxs-lookup"><span data-stu-id="06cd2-122">Deletes a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>|
|[<span data-ttu-id="06cd2-123">更新 mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="06cd2-123">Update mobileAppIntentAndState</span></span>](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[<span data-ttu-id="06cd2-124">mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="06cd2-124">mobileAppIntentAndState</span></span>](../resources/intune-troubleshooting-mobileappintentandstate.md)|<span data-ttu-id="06cd2-125">更新[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="06cd2-125">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06cd2-126">属性</span><span class="sxs-lookup"><span data-stu-id="06cd2-126">Properties</span></span>
|<span data-ttu-id="06cd2-127">属性</span><span class="sxs-lookup"><span data-stu-id="06cd2-127">Property</span></span>|<span data-ttu-id="06cd2-128">类型</span><span class="sxs-lookup"><span data-stu-id="06cd2-128">Type</span></span>|<span data-ttu-id="06cd2-129">说明</span><span class="sxs-lookup"><span data-stu-id="06cd2-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06cd2-130">id</span><span class="sxs-lookup"><span data-stu-id="06cd2-130">id</span></span>|<span data-ttu-id="06cd2-131">String</span><span class="sxs-lookup"><span data-stu-id="06cd2-131">String</span></span>|<span data-ttu-id="06cd2-132">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="06cd2-132">UUID for the object</span></span>|
|<span data-ttu-id="06cd2-133">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="06cd2-133">managedDeviceIdentifier</span></span>|<span data-ttu-id="06cd2-134">String</span><span class="sxs-lookup"><span data-stu-id="06cd2-134">String</span></span>|<span data-ttu-id="06cd2-135">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="06cd2-135">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="06cd2-136">userId</span><span class="sxs-lookup"><span data-stu-id="06cd2-136">userId</span></span>|<span data-ttu-id="06cd2-137">String</span><span class="sxs-lookup"><span data-stu-id="06cd2-137">String</span></span>|<span data-ttu-id="06cd2-138">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="06cd2-138">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="06cd2-139">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="06cd2-139">mobileAppList</span></span>|<span data-ttu-id="06cd2-140">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)集合</span><span class="sxs-lookup"><span data-stu-id="06cd2-140">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="06cd2-141">租户的有效负载意图和状态列表。</span><span class="sxs-lookup"><span data-stu-id="06cd2-141">The list of payload intents and states for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06cd2-142">关系</span><span class="sxs-lookup"><span data-stu-id="06cd2-142">Relationships</span></span>
<span data-ttu-id="06cd2-143">无</span><span class="sxs-lookup"><span data-stu-id="06cd2-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06cd2-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06cd2-144">JSON Representation</span></span>
<span data-ttu-id="06cd2-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06cd2-145">Here is a JSON representation of the resource.</span></span>
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




