---
title: importedDeviceIdentityResult 资源类型
description: ImportedDeviceIdentityResult 资源表示尝试导入设备标识的结果。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e4a1720fee543b4814430476ebd6c84a0fc33d73
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395802"
---
# <a name="importeddeviceidentityresult-resource-type"></a><span data-ttu-id="724c5-103">importedDeviceIdentityResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="724c5-103">importedDeviceIdentityResult resource type</span></span>

> <span data-ttu-id="724c5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="724c5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="724c5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="724c5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="724c5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="724c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="724c5-107">ImportedDeviceIdentityResult 资源表示尝试导入设备标识的结果。</span><span class="sxs-lookup"><span data-stu-id="724c5-107">The importedDeviceIdentityResult resource represents the result of attempting to import a device identity.</span></span>


<span data-ttu-id="724c5-108">继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="724c5-108">Inherits from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>

## <a name="methods"></a><span data-ttu-id="724c5-109">方法</span><span class="sxs-lookup"><span data-stu-id="724c5-109">Methods</span></span>
|<span data-ttu-id="724c5-110">方法</span><span class="sxs-lookup"><span data-stu-id="724c5-110">Method</span></span>|<span data-ttu-id="724c5-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="724c5-111">Return Type</span></span>|<span data-ttu-id="724c5-112">说明</span><span class="sxs-lookup"><span data-stu-id="724c5-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="724c5-113">列表 importedDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="724c5-113">List importedDeviceIdentityResults</span></span>](../api/intune-enrollment-importeddeviceidentityresult-list.md)|<span data-ttu-id="724c5-114">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="724c5-114">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="724c5-115">列出属性和[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="724c5-115">List properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects.</span></span>|
|[<span data-ttu-id="724c5-116">获取 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="724c5-116">Get importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[<span data-ttu-id="724c5-117">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="724c5-117">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="724c5-118">读取属性和[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="724c5-118">Read properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="724c5-119">创建 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="724c5-119">Create importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[<span data-ttu-id="724c5-120">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="724c5-120">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="724c5-121">创建新的[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象。</span><span class="sxs-lookup"><span data-stu-id="724c5-121">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="724c5-122">删除 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="724c5-122">Delete importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|<span data-ttu-id="724c5-123">无</span><span class="sxs-lookup"><span data-stu-id="724c5-123">None</span></span>|<span data-ttu-id="724c5-124">删除[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)。</span><span class="sxs-lookup"><span data-stu-id="724c5-124">Deletes a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>|
|[<span data-ttu-id="724c5-125">更新 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="724c5-125">Update importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[<span data-ttu-id="724c5-126">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="724c5-126">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="724c5-127">更新[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="724c5-127">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="724c5-128">属性</span><span class="sxs-lookup"><span data-stu-id="724c5-128">Properties</span></span>
|<span data-ttu-id="724c5-129">属性</span><span class="sxs-lookup"><span data-stu-id="724c5-129">Property</span></span>|<span data-ttu-id="724c5-130">类型</span><span class="sxs-lookup"><span data-stu-id="724c5-130">Type</span></span>|<span data-ttu-id="724c5-131">说明</span><span class="sxs-lookup"><span data-stu-id="724c5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="724c5-132">id</span><span class="sxs-lookup"><span data-stu-id="724c5-132">id</span></span>|<span data-ttu-id="724c5-133">String</span><span class="sxs-lookup"><span data-stu-id="724c5-133">String</span></span>|<span data-ttu-id="724c5-134">来自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)导入的设备的标识继承的 id</span><span class="sxs-lookup"><span data-stu-id="724c5-134">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="724c5-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="724c5-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="724c5-136">String</span><span class="sxs-lookup"><span data-stu-id="724c5-136">String</span></span>|<span data-ttu-id="724c5-137">导入设备标识符继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="724c5-137">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="724c5-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="724c5-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="724c5-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="724c5-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="724c5-140">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)导入设备标识继承的类型。</span><span class="sxs-lookup"><span data-stu-id="724c5-140">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="724c5-141">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="724c5-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="724c5-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="724c5-142">lastModifiedDateTime</span></span>|<span data-ttu-id="724c5-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="724c5-143">DateTimeOffset</span></span>|<span data-ttu-id="724c5-144">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)的说明继承的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="724c5-144">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="724c5-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="724c5-145">createdDateTime</span></span>|<span data-ttu-id="724c5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="724c5-146">DateTimeOffset</span></span>|<span data-ttu-id="724c5-147">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)创建设备继承的日期时间</span><span class="sxs-lookup"><span data-stu-id="724c5-147">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="724c5-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="724c5-148">lastContactedDateTime</span></span>|<span data-ttu-id="724c5-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="724c5-149">DateTimeOffset</span></span>|<span data-ttu-id="724c5-150">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)设备继承的最后一个联系日期时间</span><span class="sxs-lookup"><span data-stu-id="724c5-150">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="724c5-151">说明</span><span class="sxs-lookup"><span data-stu-id="724c5-151">description</span></span>|<span data-ttu-id="724c5-152">String</span><span class="sxs-lookup"><span data-stu-id="724c5-152">String</span></span>|<span data-ttu-id="724c5-153">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)设备继承说明</span><span class="sxs-lookup"><span data-stu-id="724c5-153">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="724c5-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="724c5-154">enrollmentState</span></span>|[<span data-ttu-id="724c5-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="724c5-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="724c5-156">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)中 Intune 继承的设备的状态。</span><span class="sxs-lookup"><span data-stu-id="724c5-156">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="724c5-157">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="724c5-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="724c5-158">platform</span><span class="sxs-lookup"><span data-stu-id="724c5-158">platform</span></span>|[<span data-ttu-id="724c5-159">平台</span><span class="sxs-lookup"><span data-stu-id="724c5-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="724c5-160">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="724c5-160">The platform of the Device.</span></span> <span data-ttu-id="724c5-161">继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="724c5-161">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="724c5-162">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="724c5-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="724c5-163">status</span><span class="sxs-lookup"><span data-stu-id="724c5-163">status</span></span>|<span data-ttu-id="724c5-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="724c5-164">Boolean</span></span>|<span data-ttu-id="724c5-165">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="724c5-165">Status of imported device identity</span></span>|

## <a name="relationships"></a><span data-ttu-id="724c5-166">关系</span><span class="sxs-lookup"><span data-stu-id="724c5-166">Relationships</span></span>
<span data-ttu-id="724c5-167">无</span><span class="sxs-lookup"><span data-stu-id="724c5-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="724c5-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="724c5-168">JSON Representation</span></span>
<span data-ttu-id="724c5-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="724c5-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentityResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```




