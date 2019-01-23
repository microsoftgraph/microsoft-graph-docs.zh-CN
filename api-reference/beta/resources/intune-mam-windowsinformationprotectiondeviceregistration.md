---
title: windowsInformationProtectionDeviceRegistration 资源类型
description: 代表 Bring-Your-Own-Device(BYOD) Windows 设备的设备注册记录。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ae81d973db8c47d9fa613db0eb1b661bb8fa0f9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429396"
---
# <a name="windowsinformationprotectiondeviceregistration-resource-type"></a><span data-ttu-id="dd304-103">windowsInformationProtectionDeviceRegistration 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd304-103">windowsInformationProtectionDeviceRegistration resource type</span></span>

> <span data-ttu-id="dd304-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="dd304-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dd304-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dd304-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd304-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd304-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd304-107">代表 Bring-Your-Own-Device(BYOD) Windows 设备的设备注册记录。</span><span class="sxs-lookup"><span data-stu-id="dd304-107">Represents device registration records for Bring-Your-Own-Device(BYOD) Windows devices.</span></span>

## <a name="methods"></a><span data-ttu-id="dd304-108">方法</span><span class="sxs-lookup"><span data-stu-id="dd304-108">Methods</span></span>
|<span data-ttu-id="dd304-109">方法</span><span class="sxs-lookup"><span data-stu-id="dd304-109">Method</span></span>|<span data-ttu-id="dd304-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="dd304-110">Return Type</span></span>|<span data-ttu-id="dd304-111">说明</span><span class="sxs-lookup"><span data-stu-id="dd304-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dd304-112">列表 windowsInformationProtectionDeviceRegistrations</span><span class="sxs-lookup"><span data-stu-id="dd304-112">List windowsInformationProtectionDeviceRegistrations</span></span>](../api/intune-mam-windowsinformationprotectiondeviceregistration-list.md)|<span data-ttu-id="dd304-113">[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)集合</span><span class="sxs-lookup"><span data-stu-id="dd304-113">[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) collection</span></span>|<span data-ttu-id="dd304-114">列出属性和[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="dd304-114">List properties and relationships of the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) objects.</span></span>|
|[<span data-ttu-id="dd304-115">获取 windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="dd304-115">Get windowsInformationProtectionDeviceRegistration</span></span>](../api/intune-mam-windowsinformationprotectiondeviceregistration-get.md)|[<span data-ttu-id="dd304-116">windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="dd304-116">windowsInformationProtectionDeviceRegistration</span></span>](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|<span data-ttu-id="dd304-117">读取属性和[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="dd304-117">Read properties and relationships of the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>|
|[<span data-ttu-id="dd304-118">创建 windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="dd304-118">Create windowsInformationProtectionDeviceRegistration</span></span>](../api/intune-mam-windowsinformationprotectiondeviceregistration-create.md)|[<span data-ttu-id="dd304-119">windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="dd304-119">windowsInformationProtectionDeviceRegistration</span></span>](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|<span data-ttu-id="dd304-120">创建新的[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dd304-120">Create a new [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>|
|[<span data-ttu-id="dd304-121">删除 windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="dd304-121">Delete windowsInformationProtectionDeviceRegistration</span></span>](../api/intune-mam-windowsinformationprotectiondeviceregistration-delete.md)|<span data-ttu-id="dd304-122">无</span><span class="sxs-lookup"><span data-stu-id="dd304-122">None</span></span>|<span data-ttu-id="dd304-123">删除[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)。</span><span class="sxs-lookup"><span data-stu-id="dd304-123">Deletes a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span></span>|
|[<span data-ttu-id="dd304-124">更新 windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="dd304-124">Update windowsInformationProtectionDeviceRegistration</span></span>](../api/intune-mam-windowsinformationprotectiondeviceregistration-update.md)|[<span data-ttu-id="dd304-125">windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="dd304-125">windowsInformationProtectionDeviceRegistration</span></span>](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|<span data-ttu-id="dd304-126">更新[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dd304-126">Update the properties of a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>|
|[<span data-ttu-id="dd304-127">wipe 操作</span><span class="sxs-lookup"><span data-stu-id="dd304-127">wipe action</span></span>](../api/intune-mam-windowsinformationprotectiondeviceregistration-wipe.md)|<span data-ttu-id="dd304-128">无</span><span class="sxs-lookup"><span data-stu-id="dd304-128">None</span></span>|<span data-ttu-id="dd304-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dd304-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="dd304-130">属性</span><span class="sxs-lookup"><span data-stu-id="dd304-130">Properties</span></span>
|<span data-ttu-id="dd304-131">属性</span><span class="sxs-lookup"><span data-stu-id="dd304-131">Property</span></span>|<span data-ttu-id="dd304-132">类型</span><span class="sxs-lookup"><span data-stu-id="dd304-132">Type</span></span>|<span data-ttu-id="dd304-133">说明</span><span class="sxs-lookup"><span data-stu-id="dd304-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd304-134">id</span><span class="sxs-lookup"><span data-stu-id="dd304-134">id</span></span>|<span data-ttu-id="dd304-135">String</span><span class="sxs-lookup"><span data-stu-id="dd304-135">String</span></span>|<span data-ttu-id="dd304-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dd304-136">Key of the entity.</span></span>|
|<span data-ttu-id="dd304-137">userId</span><span class="sxs-lookup"><span data-stu-id="dd304-137">userId</span></span>|<span data-ttu-id="dd304-138">String</span><span class="sxs-lookup"><span data-stu-id="dd304-138">String</span></span>|<span data-ttu-id="dd304-139">此设备注册记录相关联的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="dd304-139">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="dd304-140">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="dd304-140">deviceRegistrationId</span></span>|<span data-ttu-id="dd304-141">字符串</span><span class="sxs-lookup"><span data-stu-id="dd304-141">String</span></span>|<span data-ttu-id="dd304-142">此设备注册记录的的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="dd304-142">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="dd304-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="dd304-143">deviceName</span></span>|<span data-ttu-id="dd304-144">String</span><span class="sxs-lookup"><span data-stu-id="dd304-144">String</span></span>|<span data-ttu-id="dd304-145">设备名称。</span><span class="sxs-lookup"><span data-stu-id="dd304-145">Device name.</span></span>|
|<span data-ttu-id="dd304-146">deviceType</span><span class="sxs-lookup"><span data-stu-id="dd304-146">deviceType</span></span>|<span data-ttu-id="dd304-147">String</span><span class="sxs-lookup"><span data-stu-id="dd304-147">String</span></span>|<span data-ttu-id="dd304-148">设备类型，例如 Windows 便携式计算机 VS Windows phone。</span><span class="sxs-lookup"><span data-stu-id="dd304-148">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="dd304-149">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="dd304-149">deviceMacAddress</span></span>|<span data-ttu-id="dd304-150">String</span><span class="sxs-lookup"><span data-stu-id="dd304-150">String</span></span>|<span data-ttu-id="dd304-151">设备的 Mac 地址。</span><span class="sxs-lookup"><span data-stu-id="dd304-151">Device Mac address.</span></span>|
|<span data-ttu-id="dd304-152">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="dd304-152">lastCheckInDateTime</span></span>|<span data-ttu-id="dd304-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd304-153">DateTimeOffset</span></span>|<span data-ttu-id="dd304-154">设备的最后一个签入时间。</span><span class="sxs-lookup"><span data-stu-id="dd304-154">Last checkin time of the device.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd304-155">关系</span><span class="sxs-lookup"><span data-stu-id="dd304-155">Relationships</span></span>
<span data-ttu-id="dd304-156">无</span><span class="sxs-lookup"><span data-stu-id="dd304-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd304-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd304-157">JSON Representation</span></span>
<span data-ttu-id="dd304-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd304-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDeviceRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "String (identifier)",
  "userId": "String",
  "deviceRegistrationId": "String",
  "deviceName": "String",
  "deviceType": "String",
  "deviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```




