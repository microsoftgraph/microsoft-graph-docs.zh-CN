---
title: deviceManagement 资源类型
description: 充当所有设备管理功能的容器的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bff42d331ac2fe67bdca2193a4ab8ad230b36113
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755237"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="9a22d-103">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a22d-103">deviceManagement resource type</span></span>

<span data-ttu-id="9a22d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a22d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a22d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a22d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a22d-106">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="9a22d-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="9a22d-107">方法</span><span class="sxs-lookup"><span data-stu-id="9a22d-107">Methods</span></span>
|<span data-ttu-id="9a22d-108">方法</span><span class="sxs-lookup"><span data-stu-id="9a22d-108">Method</span></span>|<span data-ttu-id="9a22d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9a22d-109">Return Type</span></span>|<span data-ttu-id="9a22d-110">说明</span><span class="sxs-lookup"><span data-stu-id="9a22d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9a22d-111">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="9a22d-111">Get deviceManagement</span></span>](../api/intune-devices-devicemanagement-get.md)|[<span data-ttu-id="9a22d-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="9a22d-112">deviceManagement</span></span>](../resources/intune-devices-devicemanagement.md)|<span data-ttu-id="9a22d-113">读取 [deviceManagement](../resources/intune-devices-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9a22d-113">Read properties and relationships of the [deviceManagement](../resources/intune-devices-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="9a22d-114">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="9a22d-114">Update deviceManagement</span></span>](../api/intune-devices-devicemanagement-update.md)|[<span data-ttu-id="9a22d-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="9a22d-115">deviceManagement</span></span>](../resources/intune-devices-devicemanagement.md)|<span data-ttu-id="9a22d-116">更新 [deviceManagement](../resources/intune-devices-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9a22d-116">Update the properties of a [deviceManagement](../resources/intune-devices-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9a22d-117">属性</span><span class="sxs-lookup"><span data-stu-id="9a22d-117">Properties</span></span>
|<span data-ttu-id="9a22d-118">属性</span><span class="sxs-lookup"><span data-stu-id="9a22d-118">Property</span></span>|<span data-ttu-id="9a22d-119">类型</span><span class="sxs-lookup"><span data-stu-id="9a22d-119">Type</span></span>|<span data-ttu-id="9a22d-120">说明</span><span class="sxs-lookup"><span data-stu-id="9a22d-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a22d-121">id</span><span class="sxs-lookup"><span data-stu-id="9a22d-121">id</span></span>|<span data-ttu-id="9a22d-122">String</span><span class="sxs-lookup"><span data-stu-id="9a22d-122">String</span></span>|<span data-ttu-id="9a22d-123">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="9a22d-123">Unique Identifier for the device</span></span>|
|<span data-ttu-id="9a22d-124">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="9a22d-124">subscriptionState</span></span>|[<span data-ttu-id="9a22d-125">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="9a22d-125">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="9a22d-126">租户移动设备管理订阅状态。</span><span class="sxs-lookup"><span data-stu-id="9a22d-126">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="9a22d-127">可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="9a22d-127">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a22d-128">关系</span><span class="sxs-lookup"><span data-stu-id="9a22d-128">Relationships</span></span>
|<span data-ttu-id="9a22d-129">关系</span><span class="sxs-lookup"><span data-stu-id="9a22d-129">Relationship</span></span>|<span data-ttu-id="9a22d-130">类型</span><span class="sxs-lookup"><span data-stu-id="9a22d-130">Type</span></span>|<span data-ttu-id="9a22d-131">说明</span><span class="sxs-lookup"><span data-stu-id="9a22d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a22d-132">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="9a22d-132">applePushNotificationCertificate</span></span>|[<span data-ttu-id="9a22d-133">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="9a22d-133">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="9a22d-134">Apple 推送通知证书。</span><span class="sxs-lookup"><span data-stu-id="9a22d-134">Apple push notification certificate.</span></span>|
|<span data-ttu-id="9a22d-135">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9a22d-135">managedDeviceOverview</span></span>|[<span data-ttu-id="9a22d-136">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9a22d-136">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="9a22d-137">设备概述</span><span class="sxs-lookup"><span data-stu-id="9a22d-137">Device overview</span></span>|
|<span data-ttu-id="9a22d-138">detectedApps</span><span class="sxs-lookup"><span data-stu-id="9a22d-138">detectedApps</span></span>|<span data-ttu-id="9a22d-139">[detectedApp](../resources/intune-devices-detectedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a22d-139">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="9a22d-140">检测到与设备关联的应用的列表。</span><span class="sxs-lookup"><span data-stu-id="9a22d-140">The list of detected apps associated with a device.</span></span>|
|<span data-ttu-id="9a22d-141">managedDevices</span><span class="sxs-lookup"><span data-stu-id="9a22d-141">managedDevices</span></span>|<span data-ttu-id="9a22d-142">[managedDevice](../resources/intune-devices-manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a22d-142">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="9a22d-143">托管设备列表。</span><span class="sxs-lookup"><span data-stu-id="9a22d-143">The list of managed devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a22d-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a22d-144">JSON Representation</span></span>
<span data-ttu-id="9a22d-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a22d-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```




