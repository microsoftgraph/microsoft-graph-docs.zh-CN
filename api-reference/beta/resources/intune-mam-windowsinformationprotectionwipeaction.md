---
title: windowsInformationProtectionWipeAction 资源类型
description: 表示由租户管理员发出的用于引入并提供自己的设备 (BYOD) Windows 设备的擦除请求。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e08cd6a2cf27830f6f88328440fb100bcd77ef6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148004"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a><span data-ttu-id="7fa7b-103">windowsInformationProtectionWipeAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="7fa7b-103">windowsInformationProtectionWipeAction resource type</span></span>

> <span data-ttu-id="7fa7b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fa7b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fa7b-106">表示由租户管理员发出的用于引入并提供自己的设备 (BYOD) Windows 设备的擦除请求。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-106">Represents wipe requests issued by tenant admin for Bring-Your-Own-Device(BYOD) Windows devices.</span></span>

## <a name="methods"></a><span data-ttu-id="7fa7b-107">方法</span><span class="sxs-lookup"><span data-stu-id="7fa7b-107">Methods</span></span>
|<span data-ttu-id="7fa7b-108">方法</span><span class="sxs-lookup"><span data-stu-id="7fa7b-108">Method</span></span>|<span data-ttu-id="7fa7b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7fa7b-109">Return Type</span></span>|<span data-ttu-id="7fa7b-110">说明</span><span class="sxs-lookup"><span data-stu-id="7fa7b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7fa7b-111">列出 windowsInformationProtectionWipeActions</span><span class="sxs-lookup"><span data-stu-id="7fa7b-111">List windowsInformationProtectionWipeActions</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|<span data-ttu-id="7fa7b-112">[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="7fa7b-112">[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) collection</span></span>|<span data-ttu-id="7fa7b-113">列出[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-113">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>|
|[<span data-ttu-id="7fa7b-114">获取 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="7fa7b-114">Get windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[<span data-ttu-id="7fa7b-115">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="7fa7b-115">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="7fa7b-116">读取[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-116">Read properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="7fa7b-117">创建 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="7fa7b-117">Create windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[<span data-ttu-id="7fa7b-118">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="7fa7b-118">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="7fa7b-119">创建新的[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-119">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="7fa7b-120">删除 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="7fa7b-120">Delete windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|<span data-ttu-id="7fa7b-121">无</span><span class="sxs-lookup"><span data-stu-id="7fa7b-121">None</span></span>|<span data-ttu-id="7fa7b-122">删除[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-122">Deletes a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>|
|[<span data-ttu-id="7fa7b-123">更新 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="7fa7b-123">Update windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[<span data-ttu-id="7fa7b-124">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="7fa7b-124">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="7fa7b-125">更新[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-125">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7fa7b-126">属性</span><span class="sxs-lookup"><span data-stu-id="7fa7b-126">Properties</span></span>
|<span data-ttu-id="7fa7b-127">属性</span><span class="sxs-lookup"><span data-stu-id="7fa7b-127">Property</span></span>|<span data-ttu-id="7fa7b-128">类型</span><span class="sxs-lookup"><span data-stu-id="7fa7b-128">Type</span></span>|<span data-ttu-id="7fa7b-129">说明</span><span class="sxs-lookup"><span data-stu-id="7fa7b-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fa7b-130">id</span><span class="sxs-lookup"><span data-stu-id="7fa7b-130">id</span></span>|<span data-ttu-id="7fa7b-131">String</span><span class="sxs-lookup"><span data-stu-id="7fa7b-131">String</span></span>|<span data-ttu-id="7fa7b-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-132">Key of the entity.</span></span>|
|<span data-ttu-id="7fa7b-133">status</span><span class="sxs-lookup"><span data-stu-id="7fa7b-133">status</span></span>|[<span data-ttu-id="7fa7b-134">actionState</span><span class="sxs-lookup"><span data-stu-id="7fa7b-134">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="7fa7b-135">擦除操作状态。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-135">Wipe action status.</span></span> <span data-ttu-id="7fa7b-136">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-136">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7fa7b-137">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="7fa7b-137">targetedUserId</span></span>|<span data-ttu-id="7fa7b-138">字符串</span><span class="sxs-lookup"><span data-stu-id="7fa7b-138">String</span></span>|<span data-ttu-id="7fa7b-139">此擦除操作针对的用户 id。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-139">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="7fa7b-140">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="7fa7b-140">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="7fa7b-141">字符串</span><span class="sxs-lookup"><span data-stu-id="7fa7b-141">String</span></span>|<span data-ttu-id="7fa7b-142">此擦除操作针对的 DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-142">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="7fa7b-143">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="7fa7b-143">targetedDeviceName</span></span>|<span data-ttu-id="7fa7b-144">字符串</span><span class="sxs-lookup"><span data-stu-id="7fa7b-144">String</span></span>|<span data-ttu-id="7fa7b-145">目标设备名称。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-145">Targeted device name.</span></span>|
|<span data-ttu-id="7fa7b-146">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="7fa7b-146">targetedDeviceMacAddress</span></span>|<span data-ttu-id="7fa7b-147">字符串</span><span class="sxs-lookup"><span data-stu-id="7fa7b-147">String</span></span>|<span data-ttu-id="7fa7b-148">目标设备 Mac 地址。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-148">Targeted device Mac address.</span></span>|
|<span data-ttu-id="7fa7b-149">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="7fa7b-149">lastCheckInDateTime</span></span>|<span data-ttu-id="7fa7b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fa7b-150">DateTimeOffset</span></span>|<span data-ttu-id="7fa7b-151">此擦除操作所针对的设备的上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-151">Last checkin time of the device that was targeted by this wipe action.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fa7b-152">关系</span><span class="sxs-lookup"><span data-stu-id="7fa7b-152">Relationships</span></span>
<span data-ttu-id="7fa7b-153">无</span><span class="sxs-lookup"><span data-stu-id="7fa7b-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7fa7b-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7fa7b-154">JSON Representation</span></span>
<span data-ttu-id="7fa7b-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fa7b-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionWipeAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "String (identifier)",
  "status": "String",
  "targetedUserId": "String",
  "targetedDeviceRegistrationId": "String",
  "targetedDeviceName": "String",
  "targetedDeviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```




