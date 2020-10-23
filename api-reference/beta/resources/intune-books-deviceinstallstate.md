---
title: deviceInstallState 资源类型
description: 包含某个设备的安装状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2d1d3fcad9b0daa07a4f122ee3a87b9a4df95eec
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706016"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="dc35b-103">deviceInstallState 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc35b-103">deviceInstallState resource type</span></span>

<span data-ttu-id="dc35b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc35b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc35b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dc35b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc35b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc35b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc35b-107">包含某个设备的安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="dc35b-107">Contains properties for the installation state for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="dc35b-108">Methods</span><span class="sxs-lookup"><span data-stu-id="dc35b-108">Methods</span></span>
|<span data-ttu-id="dc35b-109">方法</span><span class="sxs-lookup"><span data-stu-id="dc35b-109">Method</span></span>|<span data-ttu-id="dc35b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="dc35b-110">Return Type</span></span>|<span data-ttu-id="dc35b-111">说明</span><span class="sxs-lookup"><span data-stu-id="dc35b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dc35b-112">列出 deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="dc35b-112">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="dc35b-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dc35b-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="dc35b-114">列出 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dc35b-114">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="dc35b-115">获取 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="dc35b-115">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="dc35b-116">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="dc35b-116">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="dc35b-117">读取 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dc35b-117">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="dc35b-118">创建 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="dc35b-118">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="dc35b-119">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="dc35b-119">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="dc35b-120">创建新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dc35b-120">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="dc35b-121">删除 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="dc35b-121">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="dc35b-122">无</span><span class="sxs-lookup"><span data-stu-id="dc35b-122">None</span></span>|<span data-ttu-id="dc35b-123">删除 [deviceInstallState](../resources/intune-books-deviceinstallstate.md)。</span><span class="sxs-lookup"><span data-stu-id="dc35b-123">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="dc35b-124">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="dc35b-124">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="dc35b-125">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="dc35b-125">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="dc35b-126">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dc35b-126">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc35b-127">属性</span><span class="sxs-lookup"><span data-stu-id="dc35b-127">Properties</span></span>
|<span data-ttu-id="dc35b-128">属性</span><span class="sxs-lookup"><span data-stu-id="dc35b-128">Property</span></span>|<span data-ttu-id="dc35b-129">类型</span><span class="sxs-lookup"><span data-stu-id="dc35b-129">Type</span></span>|<span data-ttu-id="dc35b-130">说明</span><span class="sxs-lookup"><span data-stu-id="dc35b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc35b-131">id</span><span class="sxs-lookup"><span data-stu-id="dc35b-131">id</span></span>|<span data-ttu-id="dc35b-132">String</span><span class="sxs-lookup"><span data-stu-id="dc35b-132">String</span></span>|<span data-ttu-id="dc35b-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dc35b-133">Key of the entity.</span></span>|
|<span data-ttu-id="dc35b-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="dc35b-134">deviceName</span></span>|<span data-ttu-id="dc35b-135">String</span><span class="sxs-lookup"><span data-stu-id="dc35b-135">String</span></span>|<span data-ttu-id="dc35b-136">设备名称。</span><span class="sxs-lookup"><span data-stu-id="dc35b-136">Device name.</span></span>|
|<span data-ttu-id="dc35b-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="dc35b-137">deviceId</span></span>|<span data-ttu-id="dc35b-138">String</span><span class="sxs-lookup"><span data-stu-id="dc35b-138">String</span></span>|<span data-ttu-id="dc35b-139">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="dc35b-139">Device Id.</span></span>|
|<span data-ttu-id="dc35b-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="dc35b-140">lastSyncDateTime</span></span>|<span data-ttu-id="dc35b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc35b-141">DateTimeOffset</span></span>|<span data-ttu-id="dc35b-142">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="dc35b-142">Last sync date and time.</span></span>|
|<span data-ttu-id="dc35b-143">installState</span><span class="sxs-lookup"><span data-stu-id="dc35b-143">installState</span></span>|[<span data-ttu-id="dc35b-144">installState</span><span class="sxs-lookup"><span data-stu-id="dc35b-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="dc35b-145">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="dc35b-145">The install state of the eBook.</span></span> <span data-ttu-id="dc35b-146">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="dc35b-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="dc35b-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="dc35b-147">errorCode</span></span>|<span data-ttu-id="dc35b-148">String</span><span class="sxs-lookup"><span data-stu-id="dc35b-148">String</span></span>|<span data-ttu-id="dc35b-149">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="dc35b-149">The error code for install failures.</span></span>|
|<span data-ttu-id="dc35b-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="dc35b-150">osVersion</span></span>|<span data-ttu-id="dc35b-151">String</span><span class="sxs-lookup"><span data-stu-id="dc35b-151">String</span></span>|<span data-ttu-id="dc35b-152">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="dc35b-152">OS Version.</span></span>|
|<span data-ttu-id="dc35b-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="dc35b-153">osDescription</span></span>|<span data-ttu-id="dc35b-154">String</span><span class="sxs-lookup"><span data-stu-id="dc35b-154">String</span></span>|<span data-ttu-id="dc35b-155">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="dc35b-155">OS Description.</span></span>|
|<span data-ttu-id="dc35b-156">userName</span><span class="sxs-lookup"><span data-stu-id="dc35b-156">userName</span></span>|<span data-ttu-id="dc35b-157">String</span><span class="sxs-lookup"><span data-stu-id="dc35b-157">String</span></span>|<span data-ttu-id="dc35b-158">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="dc35b-158">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc35b-159">关系</span><span class="sxs-lookup"><span data-stu-id="dc35b-159">Relationships</span></span>
<span data-ttu-id="dc35b-160">无</span><span class="sxs-lookup"><span data-stu-id="dc35b-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc35b-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc35b-161">JSON Representation</span></span>
<span data-ttu-id="dc35b-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc35b-162">Here is a JSON representation of the resource.</span></span>
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





