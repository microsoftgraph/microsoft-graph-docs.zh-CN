---
title: deviceInstallState 资源类型
description: 包含某个设备的安装状态的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0405bdb5e4a4c53a508f7b81171dd9ede41bdbb1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032086"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="1f73e-103">deviceInstallState 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f73e-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="1f73e-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1f73e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f73e-105">包含某个设备的安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="1f73e-105">Contains properties for the installation state for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="1f73e-106">方法</span><span class="sxs-lookup"><span data-stu-id="1f73e-106">Methods</span></span>
|<span data-ttu-id="1f73e-107">方法</span><span class="sxs-lookup"><span data-stu-id="1f73e-107">Method</span></span>|<span data-ttu-id="1f73e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1f73e-108">Return Type</span></span>|<span data-ttu-id="1f73e-109">说明</span><span class="sxs-lookup"><span data-stu-id="1f73e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1f73e-110">列出 deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="1f73e-110">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="1f73e-111">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1f73e-111">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="1f73e-112">列出 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1f73e-112">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="1f73e-113">获取 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="1f73e-113">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="1f73e-114">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="1f73e-114">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="1f73e-115">读取 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1f73e-115">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="1f73e-116">创建 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="1f73e-116">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="1f73e-117">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="1f73e-117">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="1f73e-118">创建新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f73e-118">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="1f73e-119">删除 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="1f73e-119">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="1f73e-120">无</span><span class="sxs-lookup"><span data-stu-id="1f73e-120">None</span></span>|<span data-ttu-id="1f73e-121">删除 [deviceInstallState](../resources/intune-books-deviceinstallstate.md)。</span><span class="sxs-lookup"><span data-stu-id="1f73e-121">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="1f73e-122">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="1f73e-122">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="1f73e-123">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="1f73e-123">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="1f73e-124">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1f73e-124">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1f73e-125">属性</span><span class="sxs-lookup"><span data-stu-id="1f73e-125">Properties</span></span>
|<span data-ttu-id="1f73e-126">属性</span><span class="sxs-lookup"><span data-stu-id="1f73e-126">Property</span></span>|<span data-ttu-id="1f73e-127">类型</span><span class="sxs-lookup"><span data-stu-id="1f73e-127">Type</span></span>|<span data-ttu-id="1f73e-128">说明</span><span class="sxs-lookup"><span data-stu-id="1f73e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f73e-129">id</span><span class="sxs-lookup"><span data-stu-id="1f73e-129">id</span></span>|<span data-ttu-id="1f73e-130">String</span><span class="sxs-lookup"><span data-stu-id="1f73e-130">String</span></span>|<span data-ttu-id="1f73e-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1f73e-131">Key of the entity.</span></span>|
|<span data-ttu-id="1f73e-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="1f73e-132">deviceName</span></span>|<span data-ttu-id="1f73e-133">String</span><span class="sxs-lookup"><span data-stu-id="1f73e-133">String</span></span>|<span data-ttu-id="1f73e-134">设备名称。</span><span class="sxs-lookup"><span data-stu-id="1f73e-134">Device name.</span></span>|
|<span data-ttu-id="1f73e-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="1f73e-135">deviceId</span></span>|<span data-ttu-id="1f73e-136">String</span><span class="sxs-lookup"><span data-stu-id="1f73e-136">String</span></span>|<span data-ttu-id="1f73e-137">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="1f73e-137">Device Id.</span></span>|
|<span data-ttu-id="1f73e-138">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1f73e-138">lastSyncDateTime</span></span>|<span data-ttu-id="1f73e-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f73e-139">DateTimeOffset</span></span>|<span data-ttu-id="1f73e-140">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1f73e-140">Last sync date and time.</span></span>|
|<span data-ttu-id="1f73e-141">installState</span><span class="sxs-lookup"><span data-stu-id="1f73e-141">installState</span></span>|[<span data-ttu-id="1f73e-142">installState</span><span class="sxs-lookup"><span data-stu-id="1f73e-142">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="1f73e-143">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="1f73e-143">The install state of the eBook.</span></span> <span data-ttu-id="1f73e-144">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="1f73e-144">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="1f73e-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="1f73e-145">errorCode</span></span>|<span data-ttu-id="1f73e-146">String</span><span class="sxs-lookup"><span data-stu-id="1f73e-146">String</span></span>|<span data-ttu-id="1f73e-147">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="1f73e-147">The error code for install failures.</span></span>|
|<span data-ttu-id="1f73e-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="1f73e-148">osVersion</span></span>|<span data-ttu-id="1f73e-149">String</span><span class="sxs-lookup"><span data-stu-id="1f73e-149">String</span></span>|<span data-ttu-id="1f73e-150">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="1f73e-150">OS Version.</span></span>|
|<span data-ttu-id="1f73e-151">osDescription</span><span class="sxs-lookup"><span data-stu-id="1f73e-151">osDescription</span></span>|<span data-ttu-id="1f73e-152">String</span><span class="sxs-lookup"><span data-stu-id="1f73e-152">String</span></span>|<span data-ttu-id="1f73e-153">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="1f73e-153">OS Description.</span></span>|
|<span data-ttu-id="1f73e-154">userName</span><span class="sxs-lookup"><span data-stu-id="1f73e-154">userName</span></span>|<span data-ttu-id="1f73e-155">String</span><span class="sxs-lookup"><span data-stu-id="1f73e-155">String</span></span>|<span data-ttu-id="1f73e-156">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="1f73e-156">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f73e-157">关系</span><span class="sxs-lookup"><span data-stu-id="1f73e-157">Relationships</span></span>
<span data-ttu-id="1f73e-158">无</span><span class="sxs-lookup"><span data-stu-id="1f73e-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f73e-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f73e-159">JSON Representation</span></span>
<span data-ttu-id="1f73e-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f73e-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```



