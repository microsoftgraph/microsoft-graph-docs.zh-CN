---
title: windowsInformationProtectionWipeAction 资源类型
description: 表示由租户管理员发出的用于引入并提供自己的设备 (BYOD) Windows 设备的擦除请求。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aba3c4a2f1120b74d4182339fb3778c75f2ff7d3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342066"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a><span data-ttu-id="0b0e2-103">windowsInformationProtectionWipeAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b0e2-103">windowsInformationProtectionWipeAction resource type</span></span>

> <span data-ttu-id="0b0e2-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b0e2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b0e2-106">表示由租户管理员发出的用于引入并提供自己的设备 (BYOD) Windows 设备的擦除请求。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-106">Represents wipe requests issued by tenant admin for Bring-Your-Own-Device(BYOD) Windows devices.</span></span>

## <a name="methods"></a><span data-ttu-id="0b0e2-107">方法</span><span class="sxs-lookup"><span data-stu-id="0b0e2-107">Methods</span></span>
|<span data-ttu-id="0b0e2-108">方法</span><span class="sxs-lookup"><span data-stu-id="0b0e2-108">Method</span></span>|<span data-ttu-id="0b0e2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0b0e2-109">Return Type</span></span>|<span data-ttu-id="0b0e2-110">说明</span><span class="sxs-lookup"><span data-stu-id="0b0e2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0b0e2-111">列出 windowsInformationProtectionWipeActions</span><span class="sxs-lookup"><span data-stu-id="0b0e2-111">List windowsInformationProtectionWipeActions</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|<span data-ttu-id="0b0e2-112">[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="0b0e2-112">[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) collection</span></span>|<span data-ttu-id="0b0e2-113">列出[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-113">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>|
|[<span data-ttu-id="0b0e2-114">获取 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="0b0e2-114">Get windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[<span data-ttu-id="0b0e2-115">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="0b0e2-115">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="0b0e2-116">读取[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-116">Read properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="0b0e2-117">创建 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="0b0e2-117">Create windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[<span data-ttu-id="0b0e2-118">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="0b0e2-118">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="0b0e2-119">创建新的[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-119">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="0b0e2-120">删除 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="0b0e2-120">Delete windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|<span data-ttu-id="0b0e2-121">无</span><span class="sxs-lookup"><span data-stu-id="0b0e2-121">None</span></span>|<span data-ttu-id="0b0e2-122">删除[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-122">Deletes a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>|
|[<span data-ttu-id="0b0e2-123">更新 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="0b0e2-123">Update windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[<span data-ttu-id="0b0e2-124">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="0b0e2-124">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="0b0e2-125">更新[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-125">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b0e2-126">属性</span><span class="sxs-lookup"><span data-stu-id="0b0e2-126">Properties</span></span>
|<span data-ttu-id="0b0e2-127">属性</span><span class="sxs-lookup"><span data-stu-id="0b0e2-127">Property</span></span>|<span data-ttu-id="0b0e2-128">类型</span><span class="sxs-lookup"><span data-stu-id="0b0e2-128">Type</span></span>|<span data-ttu-id="0b0e2-129">说明</span><span class="sxs-lookup"><span data-stu-id="0b0e2-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b0e2-130">id</span><span class="sxs-lookup"><span data-stu-id="0b0e2-130">id</span></span>|<span data-ttu-id="0b0e2-131">String</span><span class="sxs-lookup"><span data-stu-id="0b0e2-131">String</span></span>|<span data-ttu-id="0b0e2-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-132">Key of the entity.</span></span>|
|<span data-ttu-id="0b0e2-133">status</span><span class="sxs-lookup"><span data-stu-id="0b0e2-133">status</span></span>|[<span data-ttu-id="0b0e2-134">actionState</span><span class="sxs-lookup"><span data-stu-id="0b0e2-134">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="0b0e2-135">擦除操作状态。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-135">Wipe action status.</span></span> <span data-ttu-id="0b0e2-136">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-136">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="0b0e2-137">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="0b0e2-137">targetedUserId</span></span>|<span data-ttu-id="0b0e2-138">String</span><span class="sxs-lookup"><span data-stu-id="0b0e2-138">String</span></span>|<span data-ttu-id="0b0e2-139">此擦除操作针对的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-139">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="0b0e2-140">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="0b0e2-140">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="0b0e2-141">String</span><span class="sxs-lookup"><span data-stu-id="0b0e2-141">String</span></span>|<span data-ttu-id="0b0e2-142">此擦除操作针对的 DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-142">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="0b0e2-143">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="0b0e2-143">targetedDeviceName</span></span>|<span data-ttu-id="0b0e2-144">String</span><span class="sxs-lookup"><span data-stu-id="0b0e2-144">String</span></span>|<span data-ttu-id="0b0e2-145">目标设备名称。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-145">Targeted device name.</span></span>|
|<span data-ttu-id="0b0e2-146">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="0b0e2-146">targetedDeviceMacAddress</span></span>|<span data-ttu-id="0b0e2-147">String</span><span class="sxs-lookup"><span data-stu-id="0b0e2-147">String</span></span>|<span data-ttu-id="0b0e2-148">目标设备 Mac 地址。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-148">Targeted device Mac address.</span></span>|
|<span data-ttu-id="0b0e2-149">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="0b0e2-149">lastCheckInDateTime</span></span>|<span data-ttu-id="0b0e2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b0e2-150">DateTimeOffset</span></span>|<span data-ttu-id="0b0e2-151">此擦除操作所针对的设备的上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-151">Last checkin time of the device that was targeted by this wipe action.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b0e2-152">关系</span><span class="sxs-lookup"><span data-stu-id="0b0e2-152">Relationships</span></span>
<span data-ttu-id="0b0e2-153">无</span><span class="sxs-lookup"><span data-stu-id="0b0e2-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b0e2-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b0e2-154">JSON Representation</span></span>
<span data-ttu-id="0b0e2-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b0e2-155">Here is a JSON representation of the resource.</span></span>
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



