---
title: importedDeviceIdentityResult 资源类型
description: importedDeviceIdentityResult 资源表示尝试导入设备标识的结果。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b94eff5ea5e2ed37173341b45980e9b60437822d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524496"
---
# <a name="importeddeviceidentityresult-resource-type"></a><span data-ttu-id="34c66-103">importedDeviceIdentityResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="34c66-103">importedDeviceIdentityResult resource type</span></span>

> <span data-ttu-id="34c66-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34c66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34c66-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34c66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34c66-106">importedDeviceIdentityResult 资源表示尝试导入设备标识的结果。</span><span class="sxs-lookup"><span data-stu-id="34c66-106">The importedDeviceIdentityResult resource represents the result of attempting to import a device identity.</span></span>


<span data-ttu-id="34c66-107">继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="34c66-107">Inherits from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>

## <a name="methods"></a><span data-ttu-id="34c66-108">方法</span><span class="sxs-lookup"><span data-stu-id="34c66-108">Methods</span></span>
|<span data-ttu-id="34c66-109">方法</span><span class="sxs-lookup"><span data-stu-id="34c66-109">Method</span></span>|<span data-ttu-id="34c66-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="34c66-110">Return Type</span></span>|<span data-ttu-id="34c66-111">说明</span><span class="sxs-lookup"><span data-stu-id="34c66-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="34c66-112">列出 importedDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="34c66-112">List importedDeviceIdentityResults</span></span>](../api/intune-enrollment-importeddeviceidentityresult-list.md)|<span data-ttu-id="34c66-113">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="34c66-113">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="34c66-114">列出[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="34c66-114">List properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects.</span></span>|
|[<span data-ttu-id="34c66-115">获取 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="34c66-115">Get importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[<span data-ttu-id="34c66-116">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="34c66-116">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="34c66-117">读取[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="34c66-117">Read properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="34c66-118">创建 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="34c66-118">Create importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[<span data-ttu-id="34c66-119">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="34c66-119">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="34c66-120">创建新的[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象。</span><span class="sxs-lookup"><span data-stu-id="34c66-120">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="34c66-121">删除 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="34c66-121">Delete importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|<span data-ttu-id="34c66-122">无</span><span class="sxs-lookup"><span data-stu-id="34c66-122">None</span></span>|<span data-ttu-id="34c66-123">删除[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)。</span><span class="sxs-lookup"><span data-stu-id="34c66-123">Deletes a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>|
|[<span data-ttu-id="34c66-124">更新 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="34c66-124">Update importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[<span data-ttu-id="34c66-125">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="34c66-125">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="34c66-126">更新[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="34c66-126">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="34c66-127">属性</span><span class="sxs-lookup"><span data-stu-id="34c66-127">Properties</span></span>
|<span data-ttu-id="34c66-128">属性</span><span class="sxs-lookup"><span data-stu-id="34c66-128">Property</span></span>|<span data-ttu-id="34c66-129">类型</span><span class="sxs-lookup"><span data-stu-id="34c66-129">Type</span></span>|<span data-ttu-id="34c66-130">说明</span><span class="sxs-lookup"><span data-stu-id="34c66-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34c66-131">id</span><span class="sxs-lookup"><span data-stu-id="34c66-131">id</span></span>|<span data-ttu-id="34c66-132">字符串</span><span class="sxs-lookup"><span data-stu-id="34c66-132">String</span></span>|<span data-ttu-id="34c66-133">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识的 Id</span><span class="sxs-lookup"><span data-stu-id="34c66-133">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="34c66-134">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="34c66-134">importedDeviceIdentifier</span></span>|<span data-ttu-id="34c66-135">String</span><span class="sxs-lookup"><span data-stu-id="34c66-135">String</span></span>|<span data-ttu-id="34c66-136">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识符</span><span class="sxs-lookup"><span data-stu-id="34c66-136">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="34c66-137">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="34c66-137">importedDeviceIdentityType</span></span>|[<span data-ttu-id="34c66-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="34c66-138">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="34c66-139">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识的类型。</span><span class="sxs-lookup"><span data-stu-id="34c66-139">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="34c66-140">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="34c66-140">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="34c66-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34c66-141">lastModifiedDateTime</span></span>|<span data-ttu-id="34c66-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34c66-142">DateTimeOffset</span></span>|<span data-ttu-id="34c66-143">继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)的说明的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="34c66-143">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="34c66-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34c66-144">createdDateTime</span></span>|<span data-ttu-id="34c66-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34c66-145">DateTimeOffset</span></span>|<span data-ttu-id="34c66-146">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="34c66-146">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="34c66-147">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="34c66-147">lastContactedDateTime</span></span>|<span data-ttu-id="34c66-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34c66-148">DateTimeOffset</span></span>|<span data-ttu-id="34c66-149">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="34c66-149">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="34c66-150">description</span><span class="sxs-lookup"><span data-stu-id="34c66-150">description</span></span>|<span data-ttu-id="34c66-151">String</span><span class="sxs-lookup"><span data-stu-id="34c66-151">String</span></span>|<span data-ttu-id="34c66-152">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的说明</span><span class="sxs-lookup"><span data-stu-id="34c66-152">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="34c66-153">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="34c66-153">enrollmentState</span></span>|[<span data-ttu-id="34c66-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="34c66-154">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="34c66-155">Intune 中的设备的状态继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="34c66-155">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="34c66-156">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="34c66-156">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="34c66-157">platform</span><span class="sxs-lookup"><span data-stu-id="34c66-157">platform</span></span>|[<span data-ttu-id="34c66-158">平台</span><span class="sxs-lookup"><span data-stu-id="34c66-158">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="34c66-159">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="34c66-159">The platform of the Device.</span></span> <span data-ttu-id="34c66-160">继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="34c66-160">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="34c66-161">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="34c66-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="34c66-162">状态</span><span class="sxs-lookup"><span data-stu-id="34c66-162">status</span></span>|<span data-ttu-id="34c66-163">布尔值</span><span class="sxs-lookup"><span data-stu-id="34c66-163">Boolean</span></span>|<span data-ttu-id="34c66-164">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="34c66-164">Status of imported device identity</span></span>|

## <a name="relationships"></a><span data-ttu-id="34c66-165">关系</span><span class="sxs-lookup"><span data-stu-id="34c66-165">Relationships</span></span>
<span data-ttu-id="34c66-166">无</span><span class="sxs-lookup"><span data-stu-id="34c66-166">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34c66-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34c66-167">JSON Representation</span></span>
<span data-ttu-id="34c66-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34c66-168">Here is a JSON representation of the resource.</span></span>
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





