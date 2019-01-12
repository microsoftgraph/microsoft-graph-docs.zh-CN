---
title: mobileAppTroubleshootingEvent 资源类型
description: 代表用户设备应用程序事件安装状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d26873b90941f27538a5c71e113a92bb5af1bf26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977323"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a><span data-ttu-id="23fdf-103">mobileAppTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="23fdf-103">mobileAppTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="23fdf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="23fdf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23fdf-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="23fdf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23fdf-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="23fdf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23fdf-107">代表用户设备应用程序事件安装状态。</span><span class="sxs-lookup"><span data-stu-id="23fdf-107">Event representing a users device application install status.</span></span>

<span data-ttu-id="23fdf-108">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="23fdf-108">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="23fdf-109">方法</span><span class="sxs-lookup"><span data-stu-id="23fdf-109">Methods</span></span>
|<span data-ttu-id="23fdf-110">方法</span><span class="sxs-lookup"><span data-stu-id="23fdf-110">Method</span></span>|<span data-ttu-id="23fdf-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="23fdf-111">Return Type</span></span>|<span data-ttu-id="23fdf-112">说明</span><span class="sxs-lookup"><span data-stu-id="23fdf-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="23fdf-113">列表 mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="23fdf-113">List mobileAppTroubleshootingEvents</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-list.md)|<span data-ttu-id="23fdf-114">[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)集合</span><span class="sxs-lookup"><span data-stu-id="23fdf-114">[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) collection</span></span>|<span data-ttu-id="23fdf-115">列出属性和[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="23fdf-115">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="23fdf-116">获取 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="23fdf-116">Get mobileAppTroubleshootingEvent</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-get.md)|[<span data-ttu-id="23fdf-117">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="23fdf-117">mobileAppTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|<span data-ttu-id="23fdf-118">读取属性和[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="23fdf-118">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="23fdf-119">创建 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="23fdf-119">Create mobileAppTroubleshootingEvent</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-create.md)|[<span data-ttu-id="23fdf-120">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="23fdf-120">mobileAppTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|<span data-ttu-id="23fdf-121">创建新的[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="23fdf-121">Create a new [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="23fdf-122">删除 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="23fdf-122">Delete mobileAppTroubleshootingEvent</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-delete.md)|<span data-ttu-id="23fdf-123">无</span><span class="sxs-lookup"><span data-stu-id="23fdf-123">None</span></span>|<span data-ttu-id="23fdf-124">删除[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="23fdf-124">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="23fdf-125">更新 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="23fdf-125">Update mobileAppTroubleshootingEvent</span></span>](../api/intune-troubleshooting-mobileapptroubleshootingevent-update.md)|[<span data-ttu-id="23fdf-126">mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="23fdf-126">mobileAppTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|<span data-ttu-id="23fdf-127">更新[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="23fdf-127">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="23fdf-128">属性</span><span class="sxs-lookup"><span data-stu-id="23fdf-128">Properties</span></span>
|<span data-ttu-id="23fdf-129">属性</span><span class="sxs-lookup"><span data-stu-id="23fdf-129">Property</span></span>|<span data-ttu-id="23fdf-130">类型</span><span class="sxs-lookup"><span data-stu-id="23fdf-130">Type</span></span>|<span data-ttu-id="23fdf-131">说明</span><span class="sxs-lookup"><span data-stu-id="23fdf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23fdf-132">id</span><span class="sxs-lookup"><span data-stu-id="23fdf-132">id</span></span>|<span data-ttu-id="23fdf-133">String</span><span class="sxs-lookup"><span data-stu-id="23fdf-133">String</span></span>|<span data-ttu-id="23fdf-134">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="23fdf-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="23fdf-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="23fdf-135">eventDateTime</span></span>|<span data-ttu-id="23fdf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23fdf-136">DateTimeOffset</span></span>|<span data-ttu-id="23fdf-137">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="23fdf-137">Time when the event occurred .</span></span> <span data-ttu-id="23fdf-138">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="23fdf-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="23fdf-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="23fdf-139">correlationId</span></span>|<span data-ttu-id="23fdf-140">String</span><span class="sxs-lookup"><span data-stu-id="23fdf-140">String</span></span>|<span data-ttu-id="23fdf-141">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="23fdf-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="23fdf-142">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="23fdf-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="23fdf-143">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="23fdf-143">managedDeviceIdentifier</span></span>|<span data-ttu-id="23fdf-144">String</span><span class="sxs-lookup"><span data-stu-id="23fdf-144">String</span></span>|<span data-ttu-id="23fdf-145">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="23fdf-145">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="23fdf-146">userId</span><span class="sxs-lookup"><span data-stu-id="23fdf-146">userId</span></span>|<span data-ttu-id="23fdf-147">String</span><span class="sxs-lookup"><span data-stu-id="23fdf-147">String</span></span>|<span data-ttu-id="23fdf-148">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="23fdf-148">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="23fdf-149">applicationId</span><span class="sxs-lookup"><span data-stu-id="23fdf-149">applicationId</span></span>|<span data-ttu-id="23fdf-150">String</span><span class="sxs-lookup"><span data-stu-id="23fdf-150">String</span></span>|<span data-ttu-id="23fdf-151">Intune 应用程序标识符。</span><span class="sxs-lookup"><span data-stu-id="23fdf-151">Intune application identifier.</span></span>|
|<span data-ttu-id="23fdf-152">历史记录</span><span class="sxs-lookup"><span data-stu-id="23fdf-152">history</span></span>|<span data-ttu-id="23fdf-153">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="23fdf-153">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="23fdf-154">疑难解答历史记录项 Intune 移动应用程序</span><span class="sxs-lookup"><span data-stu-id="23fdf-154">Intune Mobile Application Troubleshooting History Item</span></span>|

## <a name="relationships"></a><span data-ttu-id="23fdf-155">Relationships</span><span class="sxs-lookup"><span data-stu-id="23fdf-155">Relationships</span></span>
<span data-ttu-id="23fdf-156">无</span><span class="sxs-lookup"><span data-stu-id="23fdf-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23fdf-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23fdf-157">JSON Representation</span></span>
<span data-ttu-id="23fdf-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23fdf-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "applicationId": "String",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "String (timestamp)"
    }
  ]
}
```





