---
title: windowsInformationProtectionWipeAction 资源类型
description: 代表擦除 Bring-Your-Own-Device(BYOD) Windows 设备的租户管理员发出请求。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 67af8bdde412381bb6362ef1768dca12fdfce6c2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431385"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a><span data-ttu-id="464a3-103">windowsInformationProtectionWipeAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="464a3-103">windowsInformationProtectionWipeAction resource type</span></span>

> <span data-ttu-id="464a3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="464a3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="464a3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="464a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="464a3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="464a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="464a3-107">代表擦除 Bring-Your-Own-Device(BYOD) Windows 设备的租户管理员发出请求。</span><span class="sxs-lookup"><span data-stu-id="464a3-107">Represents wipe requests issued by tenant admin for Bring-Your-Own-Device(BYOD) Windows devices.</span></span>

## <a name="methods"></a><span data-ttu-id="464a3-108">方法</span><span class="sxs-lookup"><span data-stu-id="464a3-108">Methods</span></span>
|<span data-ttu-id="464a3-109">方法</span><span class="sxs-lookup"><span data-stu-id="464a3-109">Method</span></span>|<span data-ttu-id="464a3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="464a3-110">Return Type</span></span>|<span data-ttu-id="464a3-111">说明</span><span class="sxs-lookup"><span data-stu-id="464a3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="464a3-112">列表 windowsInformationProtectionWipeActions</span><span class="sxs-lookup"><span data-stu-id="464a3-112">List windowsInformationProtectionWipeActions</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|<span data-ttu-id="464a3-113">[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="464a3-113">[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) collection</span></span>|<span data-ttu-id="464a3-114">列出属性和[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="464a3-114">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>|
|[<span data-ttu-id="464a3-115">获取 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="464a3-115">Get windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[<span data-ttu-id="464a3-116">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="464a3-116">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="464a3-117">读取属性和[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="464a3-117">Read properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="464a3-118">创建 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="464a3-118">Create windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[<span data-ttu-id="464a3-119">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="464a3-119">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="464a3-120">创建新的[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="464a3-120">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="464a3-121">删除 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="464a3-121">Delete windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|<span data-ttu-id="464a3-122">无</span><span class="sxs-lookup"><span data-stu-id="464a3-122">None</span></span>|<span data-ttu-id="464a3-123">删除[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)。</span><span class="sxs-lookup"><span data-stu-id="464a3-123">Deletes a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>|
|[<span data-ttu-id="464a3-124">更新 windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="464a3-124">Update windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[<span data-ttu-id="464a3-125">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="464a3-125">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="464a3-126">更新[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="464a3-126">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="464a3-127">属性</span><span class="sxs-lookup"><span data-stu-id="464a3-127">Properties</span></span>
|<span data-ttu-id="464a3-128">属性</span><span class="sxs-lookup"><span data-stu-id="464a3-128">Property</span></span>|<span data-ttu-id="464a3-129">类型</span><span class="sxs-lookup"><span data-stu-id="464a3-129">Type</span></span>|<span data-ttu-id="464a3-130">说明</span><span class="sxs-lookup"><span data-stu-id="464a3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="464a3-131">id</span><span class="sxs-lookup"><span data-stu-id="464a3-131">id</span></span>|<span data-ttu-id="464a3-132">String</span><span class="sxs-lookup"><span data-stu-id="464a3-132">String</span></span>|<span data-ttu-id="464a3-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="464a3-133">Key of the entity.</span></span>|
|<span data-ttu-id="464a3-134">status</span><span class="sxs-lookup"><span data-stu-id="464a3-134">status</span></span>|[<span data-ttu-id="464a3-135">actionState</span><span class="sxs-lookup"><span data-stu-id="464a3-135">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="464a3-136">擦除操作状态。</span><span class="sxs-lookup"><span data-stu-id="464a3-136">Wipe action status.</span></span> <span data-ttu-id="464a3-137">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="464a3-137">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="464a3-138">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="464a3-138">targetedUserId</span></span>|<span data-ttu-id="464a3-139">String</span><span class="sxs-lookup"><span data-stu-id="464a3-139">String</span></span>|<span data-ttu-id="464a3-140">此擦除操作所针对的 UserId。</span><span class="sxs-lookup"><span data-stu-id="464a3-140">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="464a3-141">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="464a3-141">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="464a3-142">String</span><span class="sxs-lookup"><span data-stu-id="464a3-142">String</span></span>|<span data-ttu-id="464a3-143">此擦除操作所针对 DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="464a3-143">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="464a3-144">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="464a3-144">targetedDeviceName</span></span>|<span data-ttu-id="464a3-145">String</span><span class="sxs-lookup"><span data-stu-id="464a3-145">String</span></span>|<span data-ttu-id="464a3-146">目标的设备名称。</span><span class="sxs-lookup"><span data-stu-id="464a3-146">Targeted device name.</span></span>|
|<span data-ttu-id="464a3-147">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="464a3-147">targetedDeviceMacAddress</span></span>|<span data-ttu-id="464a3-148">String</span><span class="sxs-lookup"><span data-stu-id="464a3-148">String</span></span>|<span data-ttu-id="464a3-149">目标的设备的 Mac 地址。</span><span class="sxs-lookup"><span data-stu-id="464a3-149">Targeted device Mac address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="464a3-150">关系</span><span class="sxs-lookup"><span data-stu-id="464a3-150">Relationships</span></span>
<span data-ttu-id="464a3-151">无</span><span class="sxs-lookup"><span data-stu-id="464a3-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="464a3-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="464a3-152">JSON Representation</span></span>
<span data-ttu-id="464a3-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="464a3-153">Here is a JSON representation of the resource.</span></span>
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
  "targetedDeviceMacAddress": "String"
}
```




