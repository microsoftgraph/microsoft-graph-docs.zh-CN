---
title: deviceInstallState 资源类型
description: 包含某个设备的安装状态的属性。
ms.openlocfilehash: 9fb7f7b2bbbb46a068d5ba41db022eed3072520d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011600"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="3aa79-103">deviceInstallState 资源类型</span><span class="sxs-lookup"><span data-stu-id="3aa79-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="3aa79-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3aa79-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3aa79-105">包含某个设备的安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="3aa79-105">Contains properties for the installation state for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="3aa79-106">方法</span><span class="sxs-lookup"><span data-stu-id="3aa79-106">Methods</span></span>
|<span data-ttu-id="3aa79-107">方法</span><span class="sxs-lookup"><span data-stu-id="3aa79-107">Method</span></span>|<span data-ttu-id="3aa79-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3aa79-108">Return Type</span></span>|<span data-ttu-id="3aa79-109">说明</span><span class="sxs-lookup"><span data-stu-id="3aa79-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3aa79-110">列出 deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="3aa79-110">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="3aa79-111">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3aa79-111">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="3aa79-112">列出 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3aa79-112">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="3aa79-113">获取 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="3aa79-113">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="3aa79-114">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="3aa79-114">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="3aa79-115">读取 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3aa79-115">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="3aa79-116">创建 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="3aa79-116">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="3aa79-117">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="3aa79-117">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="3aa79-118">创建新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3aa79-118">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="3aa79-119">删除 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="3aa79-119">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="3aa79-120">无</span><span class="sxs-lookup"><span data-stu-id="3aa79-120">None</span></span>|<span data-ttu-id="3aa79-121">删除 [deviceInstallState](../resources/intune-books-deviceinstallstate.md)。</span><span class="sxs-lookup"><span data-stu-id="3aa79-121">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="3aa79-122">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="3aa79-122">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="3aa79-123">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="3aa79-123">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="3aa79-124">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3aa79-124">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3aa79-125">属性</span><span class="sxs-lookup"><span data-stu-id="3aa79-125">Properties</span></span>
|<span data-ttu-id="3aa79-126">属性</span><span class="sxs-lookup"><span data-stu-id="3aa79-126">Property</span></span>|<span data-ttu-id="3aa79-127">类型</span><span class="sxs-lookup"><span data-stu-id="3aa79-127">Type</span></span>|<span data-ttu-id="3aa79-128">说明</span><span class="sxs-lookup"><span data-stu-id="3aa79-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3aa79-129">id</span><span class="sxs-lookup"><span data-stu-id="3aa79-129">id</span></span>|<span data-ttu-id="3aa79-130">String</span><span class="sxs-lookup"><span data-stu-id="3aa79-130">String</span></span>|<span data-ttu-id="3aa79-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3aa79-131">Key of the entity.</span></span>|
|<span data-ttu-id="3aa79-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="3aa79-132">deviceName</span></span>|<span data-ttu-id="3aa79-133">String</span><span class="sxs-lookup"><span data-stu-id="3aa79-133">String</span></span>|<span data-ttu-id="3aa79-134">设备名称。</span><span class="sxs-lookup"><span data-stu-id="3aa79-134">Device name.</span></span>|
|<span data-ttu-id="3aa79-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="3aa79-135">deviceId</span></span>|<span data-ttu-id="3aa79-136">String</span><span class="sxs-lookup"><span data-stu-id="3aa79-136">String</span></span>|<span data-ttu-id="3aa79-137">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="3aa79-137">Device Id.</span></span>|
|<span data-ttu-id="3aa79-138">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3aa79-138">lastSyncDateTime</span></span>|<span data-ttu-id="3aa79-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3aa79-139">DateTimeOffset</span></span>|<span data-ttu-id="3aa79-140">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3aa79-140">Last sync date and time.</span></span>|
|<span data-ttu-id="3aa79-141">installState</span><span class="sxs-lookup"><span data-stu-id="3aa79-141">installState</span></span>|[<span data-ttu-id="3aa79-142">installState</span><span class="sxs-lookup"><span data-stu-id="3aa79-142">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="3aa79-143">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="3aa79-143">The install state of the eBook.</span></span> <span data-ttu-id="3aa79-144">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="3aa79-144">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="3aa79-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="3aa79-145">errorCode</span></span>|<span data-ttu-id="3aa79-146">String</span><span class="sxs-lookup"><span data-stu-id="3aa79-146">String</span></span>|<span data-ttu-id="3aa79-147">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="3aa79-147">The error code for install failures.</span></span>|
|<span data-ttu-id="3aa79-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="3aa79-148">osVersion</span></span>|<span data-ttu-id="3aa79-149">String</span><span class="sxs-lookup"><span data-stu-id="3aa79-149">String</span></span>|<span data-ttu-id="3aa79-150">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="3aa79-150">OS Version.</span></span>|
|<span data-ttu-id="3aa79-151">osDescription</span><span class="sxs-lookup"><span data-stu-id="3aa79-151">osDescription</span></span>|<span data-ttu-id="3aa79-152">String</span><span class="sxs-lookup"><span data-stu-id="3aa79-152">String</span></span>|<span data-ttu-id="3aa79-153">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="3aa79-153">OS Description.</span></span>|
|<span data-ttu-id="3aa79-154">userName</span><span class="sxs-lookup"><span data-stu-id="3aa79-154">userName</span></span>|<span data-ttu-id="3aa79-155">String</span><span class="sxs-lookup"><span data-stu-id="3aa79-155">String</span></span>|<span data-ttu-id="3aa79-156">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="3aa79-156">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3aa79-157">关系</span><span class="sxs-lookup"><span data-stu-id="3aa79-157">Relationships</span></span>
<span data-ttu-id="3aa79-158">无</span><span class="sxs-lookup"><span data-stu-id="3aa79-158">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3aa79-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3aa79-159">JSON Representation</span></span>
<span data-ttu-id="3aa79-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3aa79-160">Here is a JSON representation of the resource.</span></span>
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



