---
title: deviceInstallState 资源类型
description: 包含某个设备的安装状态的属性。
ms.openlocfilehash: 944cb57d397ffe7b75f0a378680b0f1468b10f49
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048020"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="9e27a-103">deviceInstallState 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e27a-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="9e27a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9e27a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e27a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9e27a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e27a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9e27a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e27a-107">包含某个设备的安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="9e27a-107">Contains properties for the installation state for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="9e27a-108">方法</span><span class="sxs-lookup"><span data-stu-id="9e27a-108">Methods</span></span>
|<span data-ttu-id="9e27a-109">方法</span><span class="sxs-lookup"><span data-stu-id="9e27a-109">Method</span></span>|<span data-ttu-id="9e27a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9e27a-110">Return Type</span></span>|<span data-ttu-id="9e27a-111">说明</span><span class="sxs-lookup"><span data-stu-id="9e27a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9e27a-112">列出 deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="9e27a-112">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="9e27a-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e27a-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="9e27a-114">列出 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9e27a-114">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="9e27a-115">获取 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9e27a-115">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="9e27a-116">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9e27a-116">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="9e27a-117">读取 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9e27a-117">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="9e27a-118">创建 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9e27a-118">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="9e27a-119">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9e27a-119">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="9e27a-120">创建新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e27a-120">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="9e27a-121">删除 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9e27a-121">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="9e27a-122">无</span><span class="sxs-lookup"><span data-stu-id="9e27a-122">None</span></span>|<span data-ttu-id="9e27a-123">删除 [deviceInstallState](../resources/intune-books-deviceinstallstate.md)。</span><span class="sxs-lookup"><span data-stu-id="9e27a-123">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="9e27a-124">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9e27a-124">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="9e27a-125">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9e27a-125">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="9e27a-126">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9e27a-126">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9e27a-127">属性</span><span class="sxs-lookup"><span data-stu-id="9e27a-127">Properties</span></span>
|<span data-ttu-id="9e27a-128">属性</span><span class="sxs-lookup"><span data-stu-id="9e27a-128">Property</span></span>|<span data-ttu-id="9e27a-129">类型</span><span class="sxs-lookup"><span data-stu-id="9e27a-129">Type</span></span>|<span data-ttu-id="9e27a-130">说明</span><span class="sxs-lookup"><span data-stu-id="9e27a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e27a-131">id</span><span class="sxs-lookup"><span data-stu-id="9e27a-131">id</span></span>|<span data-ttu-id="9e27a-132">String</span><span class="sxs-lookup"><span data-stu-id="9e27a-132">String</span></span>|<span data-ttu-id="9e27a-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9e27a-133">Key of the entity.</span></span>|
|<span data-ttu-id="9e27a-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="9e27a-134">deviceName</span></span>|<span data-ttu-id="9e27a-135">String</span><span class="sxs-lookup"><span data-stu-id="9e27a-135">String</span></span>|<span data-ttu-id="9e27a-136">设备名称。</span><span class="sxs-lookup"><span data-stu-id="9e27a-136">Device name.</span></span>|
|<span data-ttu-id="9e27a-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="9e27a-137">deviceId</span></span>|<span data-ttu-id="9e27a-138">String</span><span class="sxs-lookup"><span data-stu-id="9e27a-138">String</span></span>|<span data-ttu-id="9e27a-139">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="9e27a-139">Device Id.</span></span>|
|<span data-ttu-id="9e27a-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9e27a-140">lastSyncDateTime</span></span>|<span data-ttu-id="9e27a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e27a-141">DateTimeOffset</span></span>|<span data-ttu-id="9e27a-142">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9e27a-142">Last sync date and time.</span></span>|
|<span data-ttu-id="9e27a-143">installState</span><span class="sxs-lookup"><span data-stu-id="9e27a-143">installState</span></span>|[<span data-ttu-id="9e27a-144">installState</span><span class="sxs-lookup"><span data-stu-id="9e27a-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="9e27a-145">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="9e27a-145">The install state of the eBook.</span></span> <span data-ttu-id="9e27a-146">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="9e27a-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="9e27a-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="9e27a-147">errorCode</span></span>|<span data-ttu-id="9e27a-148">String</span><span class="sxs-lookup"><span data-stu-id="9e27a-148">String</span></span>|<span data-ttu-id="9e27a-149">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="9e27a-149">The error code for install failures.</span></span>|
|<span data-ttu-id="9e27a-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="9e27a-150">osVersion</span></span>|<span data-ttu-id="9e27a-151">String</span><span class="sxs-lookup"><span data-stu-id="9e27a-151">String</span></span>|<span data-ttu-id="9e27a-152">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9e27a-152">OS Version.</span></span>|
|<span data-ttu-id="9e27a-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="9e27a-153">osDescription</span></span>|<span data-ttu-id="9e27a-154">String</span><span class="sxs-lookup"><span data-stu-id="9e27a-154">String</span></span>|<span data-ttu-id="9e27a-155">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="9e27a-155">OS Description.</span></span>|
|<span data-ttu-id="9e27a-156">userName</span><span class="sxs-lookup"><span data-stu-id="9e27a-156">userName</span></span>|<span data-ttu-id="9e27a-157">String</span><span class="sxs-lookup"><span data-stu-id="9e27a-157">String</span></span>|<span data-ttu-id="9e27a-158">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="9e27a-158">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e27a-159">关系</span><span class="sxs-lookup"><span data-stu-id="9e27a-159">Relationships</span></span>
<span data-ttu-id="9e27a-160">无</span><span class="sxs-lookup"><span data-stu-id="9e27a-160">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e27a-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e27a-161">JSON Representation</span></span>
<span data-ttu-id="9e27a-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e27a-162">Here is a JSON representation of the resource.</span></span>
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





