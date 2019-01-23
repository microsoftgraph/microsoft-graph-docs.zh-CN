---
title: deviceInstallState 资源类型
description: 包含某个设备的安装状态的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c90b3e8e0693a28781a45f77cd00661528648439
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410719"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="60e28-103">deviceInstallState 资源类型</span><span class="sxs-lookup"><span data-stu-id="60e28-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="60e28-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="60e28-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="60e28-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="60e28-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60e28-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="60e28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60e28-107">包含某个设备的安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="60e28-107">Contains properties for the installation state for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="60e28-108">方法</span><span class="sxs-lookup"><span data-stu-id="60e28-108">Methods</span></span>
|<span data-ttu-id="60e28-109">方法</span><span class="sxs-lookup"><span data-stu-id="60e28-109">Method</span></span>|<span data-ttu-id="60e28-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="60e28-110">Return Type</span></span>|<span data-ttu-id="60e28-111">说明</span><span class="sxs-lookup"><span data-stu-id="60e28-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="60e28-112">列出 deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="60e28-112">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="60e28-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="60e28-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="60e28-114">列出 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="60e28-114">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="60e28-115">获取 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="60e28-115">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="60e28-116">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="60e28-116">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="60e28-117">读取 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="60e28-117">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="60e28-118">创建 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="60e28-118">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="60e28-119">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="60e28-119">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="60e28-120">创建新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60e28-120">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="60e28-121">删除 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="60e28-121">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="60e28-122">无</span><span class="sxs-lookup"><span data-stu-id="60e28-122">None</span></span>|<span data-ttu-id="60e28-123">删除 [deviceInstallState](../resources/intune-books-deviceinstallstate.md)。</span><span class="sxs-lookup"><span data-stu-id="60e28-123">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="60e28-124">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="60e28-124">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="60e28-125">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="60e28-125">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="60e28-126">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="60e28-126">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="60e28-127">属性</span><span class="sxs-lookup"><span data-stu-id="60e28-127">Properties</span></span>
|<span data-ttu-id="60e28-128">属性</span><span class="sxs-lookup"><span data-stu-id="60e28-128">Property</span></span>|<span data-ttu-id="60e28-129">类型</span><span class="sxs-lookup"><span data-stu-id="60e28-129">Type</span></span>|<span data-ttu-id="60e28-130">说明</span><span class="sxs-lookup"><span data-stu-id="60e28-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60e28-131">id</span><span class="sxs-lookup"><span data-stu-id="60e28-131">id</span></span>|<span data-ttu-id="60e28-132">String</span><span class="sxs-lookup"><span data-stu-id="60e28-132">String</span></span>|<span data-ttu-id="60e28-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="60e28-133">Key of the entity.</span></span>|
|<span data-ttu-id="60e28-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="60e28-134">deviceName</span></span>|<span data-ttu-id="60e28-135">String</span><span class="sxs-lookup"><span data-stu-id="60e28-135">String</span></span>|<span data-ttu-id="60e28-136">设备名称。</span><span class="sxs-lookup"><span data-stu-id="60e28-136">Device name.</span></span>|
|<span data-ttu-id="60e28-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="60e28-137">deviceId</span></span>|<span data-ttu-id="60e28-138">String</span><span class="sxs-lookup"><span data-stu-id="60e28-138">String</span></span>|<span data-ttu-id="60e28-139">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="60e28-139">Device Id.</span></span>|
|<span data-ttu-id="60e28-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="60e28-140">lastSyncDateTime</span></span>|<span data-ttu-id="60e28-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60e28-141">DateTimeOffset</span></span>|<span data-ttu-id="60e28-142">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="60e28-142">Last sync date and time.</span></span>|
|<span data-ttu-id="60e28-143">installState</span><span class="sxs-lookup"><span data-stu-id="60e28-143">installState</span></span>|[<span data-ttu-id="60e28-144">installState</span><span class="sxs-lookup"><span data-stu-id="60e28-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="60e28-145">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="60e28-145">The install state of the eBook.</span></span> <span data-ttu-id="60e28-146">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="60e28-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="60e28-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="60e28-147">errorCode</span></span>|<span data-ttu-id="60e28-148">String</span><span class="sxs-lookup"><span data-stu-id="60e28-148">String</span></span>|<span data-ttu-id="60e28-149">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="60e28-149">The error code for install failures.</span></span>|
|<span data-ttu-id="60e28-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="60e28-150">osVersion</span></span>|<span data-ttu-id="60e28-151">String</span><span class="sxs-lookup"><span data-stu-id="60e28-151">String</span></span>|<span data-ttu-id="60e28-152">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="60e28-152">OS Version.</span></span>|
|<span data-ttu-id="60e28-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="60e28-153">osDescription</span></span>|<span data-ttu-id="60e28-154">String</span><span class="sxs-lookup"><span data-stu-id="60e28-154">String</span></span>|<span data-ttu-id="60e28-155">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="60e28-155">OS Description.</span></span>|
|<span data-ttu-id="60e28-156">userName</span><span class="sxs-lookup"><span data-stu-id="60e28-156">userName</span></span>|<span data-ttu-id="60e28-157">String</span><span class="sxs-lookup"><span data-stu-id="60e28-157">String</span></span>|<span data-ttu-id="60e28-158">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="60e28-158">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60e28-159">关系</span><span class="sxs-lookup"><span data-stu-id="60e28-159">Relationships</span></span>
<span data-ttu-id="60e28-160">无</span><span class="sxs-lookup"><span data-stu-id="60e28-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60e28-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60e28-161">JSON Representation</span></span>
<span data-ttu-id="60e28-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60e28-162">Here is a JSON representation of the resource.</span></span>
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




