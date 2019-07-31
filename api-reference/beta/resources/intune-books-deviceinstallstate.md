---
title: deviceInstallState 资源类型
description: 包含某个设备的安装状态的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3d1e9b86d9e3be0607cbaedb44735eab4243a769
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012063"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="58ec1-103">deviceInstallState 资源类型</span><span class="sxs-lookup"><span data-stu-id="58ec1-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="58ec1-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="58ec1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58ec1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58ec1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58ec1-106">包含某个设备的安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="58ec1-106">Contains properties for the installation state for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="58ec1-107">方法</span><span class="sxs-lookup"><span data-stu-id="58ec1-107">Methods</span></span>
|<span data-ttu-id="58ec1-108">方法</span><span class="sxs-lookup"><span data-stu-id="58ec1-108">Method</span></span>|<span data-ttu-id="58ec1-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="58ec1-109">Return Type</span></span>|<span data-ttu-id="58ec1-110">说明</span><span class="sxs-lookup"><span data-stu-id="58ec1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="58ec1-111">列出 deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="58ec1-111">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="58ec1-112">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="58ec1-112">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="58ec1-113">列出 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="58ec1-113">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="58ec1-114">获取 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="58ec1-114">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="58ec1-115">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="58ec1-115">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="58ec1-116">读取 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="58ec1-116">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="58ec1-117">创建 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="58ec1-117">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="58ec1-118">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="58ec1-118">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="58ec1-119">创建新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58ec1-119">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="58ec1-120">删除 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="58ec1-120">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="58ec1-121">无</span><span class="sxs-lookup"><span data-stu-id="58ec1-121">None</span></span>|<span data-ttu-id="58ec1-122">删除 [deviceInstallState](../resources/intune-books-deviceinstallstate.md)。</span><span class="sxs-lookup"><span data-stu-id="58ec1-122">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="58ec1-123">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="58ec1-123">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="58ec1-124">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="58ec1-124">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="58ec1-125">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="58ec1-125">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="58ec1-126">属性</span><span class="sxs-lookup"><span data-stu-id="58ec1-126">Properties</span></span>
|<span data-ttu-id="58ec1-127">属性</span><span class="sxs-lookup"><span data-stu-id="58ec1-127">Property</span></span>|<span data-ttu-id="58ec1-128">类型</span><span class="sxs-lookup"><span data-stu-id="58ec1-128">Type</span></span>|<span data-ttu-id="58ec1-129">说明</span><span class="sxs-lookup"><span data-stu-id="58ec1-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58ec1-130">id</span><span class="sxs-lookup"><span data-stu-id="58ec1-130">id</span></span>|<span data-ttu-id="58ec1-131">String</span><span class="sxs-lookup"><span data-stu-id="58ec1-131">String</span></span>|<span data-ttu-id="58ec1-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="58ec1-132">Key of the entity.</span></span>|
|<span data-ttu-id="58ec1-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="58ec1-133">deviceName</span></span>|<span data-ttu-id="58ec1-134">String</span><span class="sxs-lookup"><span data-stu-id="58ec1-134">String</span></span>|<span data-ttu-id="58ec1-135">设备名称。</span><span class="sxs-lookup"><span data-stu-id="58ec1-135">Device name.</span></span>|
|<span data-ttu-id="58ec1-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="58ec1-136">deviceId</span></span>|<span data-ttu-id="58ec1-137">String</span><span class="sxs-lookup"><span data-stu-id="58ec1-137">String</span></span>|<span data-ttu-id="58ec1-138">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="58ec1-138">Device Id.</span></span>|
|<span data-ttu-id="58ec1-139">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="58ec1-139">lastSyncDateTime</span></span>|<span data-ttu-id="58ec1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58ec1-140">DateTimeOffset</span></span>|<span data-ttu-id="58ec1-141">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="58ec1-141">Last sync date and time.</span></span>|
|<span data-ttu-id="58ec1-142">installState</span><span class="sxs-lookup"><span data-stu-id="58ec1-142">installState</span></span>|[<span data-ttu-id="58ec1-143">installState</span><span class="sxs-lookup"><span data-stu-id="58ec1-143">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="58ec1-144">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="58ec1-144">The install state of the eBook.</span></span> <span data-ttu-id="58ec1-145">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="58ec1-145">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="58ec1-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="58ec1-146">errorCode</span></span>|<span data-ttu-id="58ec1-147">String</span><span class="sxs-lookup"><span data-stu-id="58ec1-147">String</span></span>|<span data-ttu-id="58ec1-148">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="58ec1-148">The error code for install failures.</span></span>|
|<span data-ttu-id="58ec1-149">osVersion</span><span class="sxs-lookup"><span data-stu-id="58ec1-149">osVersion</span></span>|<span data-ttu-id="58ec1-150">String</span><span class="sxs-lookup"><span data-stu-id="58ec1-150">String</span></span>|<span data-ttu-id="58ec1-151">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="58ec1-151">OS Version.</span></span>|
|<span data-ttu-id="58ec1-152">osDescription</span><span class="sxs-lookup"><span data-stu-id="58ec1-152">osDescription</span></span>|<span data-ttu-id="58ec1-153">String</span><span class="sxs-lookup"><span data-stu-id="58ec1-153">String</span></span>|<span data-ttu-id="58ec1-154">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="58ec1-154">OS Description.</span></span>|
|<span data-ttu-id="58ec1-155">userName</span><span class="sxs-lookup"><span data-stu-id="58ec1-155">userName</span></span>|<span data-ttu-id="58ec1-156">String</span><span class="sxs-lookup"><span data-stu-id="58ec1-156">String</span></span>|<span data-ttu-id="58ec1-157">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="58ec1-157">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58ec1-158">关系</span><span class="sxs-lookup"><span data-stu-id="58ec1-158">Relationships</span></span>
<span data-ttu-id="58ec1-159">无</span><span class="sxs-lookup"><span data-stu-id="58ec1-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58ec1-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58ec1-160">JSON Representation</span></span>
<span data-ttu-id="58ec1-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58ec1-161">Here is a JSON representation of the resource.</span></span>
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





