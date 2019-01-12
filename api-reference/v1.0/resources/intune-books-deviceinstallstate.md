---
title: deviceInstallState 资源类型
description: 包含某个设备的安装状态的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 39f7331f8bc83840b8b5865cb71414382b3d5a50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963687"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="ba663-103">deviceInstallState 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba663-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="ba663-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ba663-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba663-105">包含某个设备的安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="ba663-105">Contains properties for the installation state for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="ba663-106">方法</span><span class="sxs-lookup"><span data-stu-id="ba663-106">Methods</span></span>
|<span data-ttu-id="ba663-107">方法</span><span class="sxs-lookup"><span data-stu-id="ba663-107">Method</span></span>|<span data-ttu-id="ba663-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ba663-108">Return Type</span></span>|<span data-ttu-id="ba663-109">说明</span><span class="sxs-lookup"><span data-stu-id="ba663-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ba663-110">列出 deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="ba663-110">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="ba663-111">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ba663-111">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="ba663-112">列出 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ba663-112">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="ba663-113">获取 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="ba663-113">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="ba663-114">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="ba663-114">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="ba663-115">读取 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ba663-115">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="ba663-116">创建 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="ba663-116">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="ba663-117">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="ba663-117">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="ba663-118">创建新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ba663-118">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="ba663-119">删除 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="ba663-119">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="ba663-120">无</span><span class="sxs-lookup"><span data-stu-id="ba663-120">None</span></span>|<span data-ttu-id="ba663-121">删除 [deviceInstallState](../resources/intune-books-deviceinstallstate.md)。</span><span class="sxs-lookup"><span data-stu-id="ba663-121">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="ba663-122">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="ba663-122">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="ba663-123">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="ba663-123">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="ba663-124">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ba663-124">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ba663-125">属性</span><span class="sxs-lookup"><span data-stu-id="ba663-125">Properties</span></span>
|<span data-ttu-id="ba663-126">属性</span><span class="sxs-lookup"><span data-stu-id="ba663-126">Property</span></span>|<span data-ttu-id="ba663-127">类型</span><span class="sxs-lookup"><span data-stu-id="ba663-127">Type</span></span>|<span data-ttu-id="ba663-128">说明</span><span class="sxs-lookup"><span data-stu-id="ba663-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba663-129">id</span><span class="sxs-lookup"><span data-stu-id="ba663-129">id</span></span>|<span data-ttu-id="ba663-130">String</span><span class="sxs-lookup"><span data-stu-id="ba663-130">String</span></span>|<span data-ttu-id="ba663-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ba663-131">Key of the entity.</span></span>|
|<span data-ttu-id="ba663-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="ba663-132">deviceName</span></span>|<span data-ttu-id="ba663-133">String</span><span class="sxs-lookup"><span data-stu-id="ba663-133">String</span></span>|<span data-ttu-id="ba663-134">设备名称。</span><span class="sxs-lookup"><span data-stu-id="ba663-134">Device name.</span></span>|
|<span data-ttu-id="ba663-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="ba663-135">deviceId</span></span>|<span data-ttu-id="ba663-136">String</span><span class="sxs-lookup"><span data-stu-id="ba663-136">String</span></span>|<span data-ttu-id="ba663-137">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="ba663-137">Device Id.</span></span>|
|<span data-ttu-id="ba663-138">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ba663-138">lastSyncDateTime</span></span>|<span data-ttu-id="ba663-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba663-139">DateTimeOffset</span></span>|<span data-ttu-id="ba663-140">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ba663-140">Last sync date and time.</span></span>|
|<span data-ttu-id="ba663-141">installState</span><span class="sxs-lookup"><span data-stu-id="ba663-141">installState</span></span>|[<span data-ttu-id="ba663-142">installState</span><span class="sxs-lookup"><span data-stu-id="ba663-142">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="ba663-143">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="ba663-143">The install state of the eBook.</span></span> <span data-ttu-id="ba663-144">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="ba663-144">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="ba663-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="ba663-145">errorCode</span></span>|<span data-ttu-id="ba663-146">String</span><span class="sxs-lookup"><span data-stu-id="ba663-146">String</span></span>|<span data-ttu-id="ba663-147">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="ba663-147">The error code for install failures.</span></span>|
|<span data-ttu-id="ba663-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="ba663-148">osVersion</span></span>|<span data-ttu-id="ba663-149">String</span><span class="sxs-lookup"><span data-stu-id="ba663-149">String</span></span>|<span data-ttu-id="ba663-150">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="ba663-150">OS Version.</span></span>|
|<span data-ttu-id="ba663-151">osDescription</span><span class="sxs-lookup"><span data-stu-id="ba663-151">osDescription</span></span>|<span data-ttu-id="ba663-152">String</span><span class="sxs-lookup"><span data-stu-id="ba663-152">String</span></span>|<span data-ttu-id="ba663-153">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="ba663-153">OS Description.</span></span>|
|<span data-ttu-id="ba663-154">userName</span><span class="sxs-lookup"><span data-stu-id="ba663-154">userName</span></span>|<span data-ttu-id="ba663-155">String</span><span class="sxs-lookup"><span data-stu-id="ba663-155">String</span></span>|<span data-ttu-id="ba663-156">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="ba663-156">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba663-157">关系</span><span class="sxs-lookup"><span data-stu-id="ba663-157">Relationships</span></span>
<span data-ttu-id="ba663-158">无</span><span class="sxs-lookup"><span data-stu-id="ba663-158">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ba663-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba663-159">JSON Representation</span></span>
<span data-ttu-id="ba663-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba663-160">Here is a JSON representation of the resource.</span></span>
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



