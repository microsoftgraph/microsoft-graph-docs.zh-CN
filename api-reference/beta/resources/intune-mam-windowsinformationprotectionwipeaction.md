---
title: windowsInformationProtectionWipeAction 资源类型
description: 表示租户管理员发出的用于引入设备 (BYOD) Windows 设备的擦除请求。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8f8e3d08dc8b05564c3be10f4bccf9b8a82740f1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029895"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a><span data-ttu-id="b8c25-103">windowsInformationProtectionWipeAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8c25-103">windowsInformationProtectionWipeAction resource type</span></span>

<span data-ttu-id="b8c25-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8c25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8c25-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b8c25-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8c25-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8c25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8c25-107">表示租户管理员发出的用于引入设备 (BYOD) Windows 设备的擦除请求。</span><span class="sxs-lookup"><span data-stu-id="b8c25-107">Represents wipe requests issued by tenant admin for Bring-Your-Own-Device(BYOD) Windows devices.</span></span>

## <a name="methods"></a><span data-ttu-id="b8c25-108">方法</span><span class="sxs-lookup"><span data-stu-id="b8c25-108">Methods</span></span>
|<span data-ttu-id="b8c25-109">方法</span><span class="sxs-lookup"><span data-stu-id="b8c25-109">Method</span></span>|<span data-ttu-id="b8c25-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b8c25-110">Return Type</span></span>|<span data-ttu-id="b8c25-111">说明</span><span class="sxs-lookup"><span data-stu-id="b8c25-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b8c25-112">列出 windowsInformationProtectionWipeActions</span><span class="sxs-lookup"><span data-stu-id="b8c25-112">List windowsInformationProtectionWipeActions</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|<span data-ttu-id="b8c25-113">[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8c25-113">[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) collection</span></span>|<span data-ttu-id="b8c25-114">列出 [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8c25-114">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>|
|[<span data-ttu-id="b8c25-115">获取 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="b8c25-115">Get windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[<span data-ttu-id="b8c25-116">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="b8c25-116">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="b8c25-117">读取 [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8c25-117">Read properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="b8c25-118">创建 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="b8c25-118">Create windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[<span data-ttu-id="b8c25-119">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="b8c25-119">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="b8c25-120">创建新的 [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b8c25-120">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="b8c25-121">删除 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="b8c25-121">Delete windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|<span data-ttu-id="b8c25-122">无</span><span class="sxs-lookup"><span data-stu-id="b8c25-122">None</span></span>|<span data-ttu-id="b8c25-123">删除 [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)。</span><span class="sxs-lookup"><span data-stu-id="b8c25-123">Deletes a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>|
|[<span data-ttu-id="b8c25-124">更新 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="b8c25-124">Update windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[<span data-ttu-id="b8c25-125">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="b8c25-125">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="b8c25-126">更新 [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b8c25-126">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8c25-127">属性</span><span class="sxs-lookup"><span data-stu-id="b8c25-127">Properties</span></span>
|<span data-ttu-id="b8c25-128">属性</span><span class="sxs-lookup"><span data-stu-id="b8c25-128">Property</span></span>|<span data-ttu-id="b8c25-129">类型</span><span class="sxs-lookup"><span data-stu-id="b8c25-129">Type</span></span>|<span data-ttu-id="b8c25-130">说明</span><span class="sxs-lookup"><span data-stu-id="b8c25-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8c25-131">id</span><span class="sxs-lookup"><span data-stu-id="b8c25-131">id</span></span>|<span data-ttu-id="b8c25-132">String</span><span class="sxs-lookup"><span data-stu-id="b8c25-132">String</span></span>|<span data-ttu-id="b8c25-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b8c25-133">Key of the entity.</span></span>|
|<span data-ttu-id="b8c25-134">状态</span><span class="sxs-lookup"><span data-stu-id="b8c25-134">status</span></span>|[<span data-ttu-id="b8c25-135">actionState</span><span class="sxs-lookup"><span data-stu-id="b8c25-135">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b8c25-136">擦除操作状态。</span><span class="sxs-lookup"><span data-stu-id="b8c25-136">Wipe action status.</span></span> <span data-ttu-id="b8c25-137">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="b8c25-137">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b8c25-138">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="b8c25-138">targetedUserId</span></span>|<span data-ttu-id="b8c25-139">String</span><span class="sxs-lookup"><span data-stu-id="b8c25-139">String</span></span>|<span data-ttu-id="b8c25-140">此擦除操作针对的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="b8c25-140">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="b8c25-141">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="b8c25-141">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="b8c25-142">String</span><span class="sxs-lookup"><span data-stu-id="b8c25-142">String</span></span>|<span data-ttu-id="b8c25-143">此擦除操作针对的 DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="b8c25-143">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="b8c25-144">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="b8c25-144">targetedDeviceName</span></span>|<span data-ttu-id="b8c25-145">String</span><span class="sxs-lookup"><span data-stu-id="b8c25-145">String</span></span>|<span data-ttu-id="b8c25-146">目标设备名称。</span><span class="sxs-lookup"><span data-stu-id="b8c25-146">Targeted device name.</span></span>|
|<span data-ttu-id="b8c25-147">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="b8c25-147">targetedDeviceMacAddress</span></span>|<span data-ttu-id="b8c25-148">String</span><span class="sxs-lookup"><span data-stu-id="b8c25-148">String</span></span>|<span data-ttu-id="b8c25-149">目标设备 Mac 地址。</span><span class="sxs-lookup"><span data-stu-id="b8c25-149">Targeted device Mac address.</span></span>|
|<span data-ttu-id="b8c25-150">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="b8c25-150">lastCheckInDateTime</span></span>|<span data-ttu-id="b8c25-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8c25-151">DateTimeOffset</span></span>|<span data-ttu-id="b8c25-152">此擦除操作所针对的设备的上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="b8c25-152">Last checkin time of the device that was targeted by this wipe action.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8c25-153">关系</span><span class="sxs-lookup"><span data-stu-id="b8c25-153">Relationships</span></span>
<span data-ttu-id="b8c25-154">无</span><span class="sxs-lookup"><span data-stu-id="b8c25-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8c25-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8c25-155">JSON Representation</span></span>
<span data-ttu-id="b8c25-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8c25-156">Here is a JSON representation of the resource.</span></span>
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






