---
title: importedDeviceIdentityResult 资源类型
description: ImportedDeviceIdentityResult 资源表示尝试导入设备标识的结果。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b905bcdc0df8d70a1e6e1e0ad8ecfed028043f6e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992596"
---
# <a name="importeddeviceidentityresult-resource-type"></a><span data-ttu-id="1ae4e-103">importedDeviceIdentityResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ae4e-103">importedDeviceIdentityResult resource type</span></span>

> <span data-ttu-id="1ae4e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ae4e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ae4e-106">ImportedDeviceIdentityResult 资源表示尝试导入设备标识的结果。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-106">The importedDeviceIdentityResult resource represents the result of attempting to import a device identity.</span></span>


<span data-ttu-id="1ae4e-107">继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="1ae4e-107">Inherits from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1ae4e-108">方法</span><span class="sxs-lookup"><span data-stu-id="1ae4e-108">Methods</span></span>
|<span data-ttu-id="1ae4e-109">方法</span><span class="sxs-lookup"><span data-stu-id="1ae4e-109">Method</span></span>|<span data-ttu-id="1ae4e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1ae4e-110">Return Type</span></span>|<span data-ttu-id="1ae4e-111">说明</span><span class="sxs-lookup"><span data-stu-id="1ae4e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1ae4e-112">列出 importedDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="1ae4e-112">List importedDeviceIdentityResults</span></span>](../api/intune-enrollment-importeddeviceidentityresult-list.md)|<span data-ttu-id="1ae4e-113">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="1ae4e-113">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="1ae4e-114">列出[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-114">List properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects.</span></span>|
|[<span data-ttu-id="1ae4e-115">获取 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="1ae4e-115">Get importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[<span data-ttu-id="1ae4e-116">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="1ae4e-116">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="1ae4e-117">读取[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-117">Read properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="1ae4e-118">创建 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="1ae4e-118">Create importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[<span data-ttu-id="1ae4e-119">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="1ae4e-119">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="1ae4e-120">创建新的[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-120">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="1ae4e-121">删除 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="1ae4e-121">Delete importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|<span data-ttu-id="1ae4e-122">无</span><span class="sxs-lookup"><span data-stu-id="1ae4e-122">None</span></span>|<span data-ttu-id="1ae4e-123">删除[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-123">Deletes a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>|
|[<span data-ttu-id="1ae4e-124">更新 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="1ae4e-124">Update importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[<span data-ttu-id="1ae4e-125">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="1ae4e-125">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="1ae4e-126">更新[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-126">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1ae4e-127">属性</span><span class="sxs-lookup"><span data-stu-id="1ae4e-127">Properties</span></span>
|<span data-ttu-id="1ae4e-128">属性</span><span class="sxs-lookup"><span data-stu-id="1ae4e-128">Property</span></span>|<span data-ttu-id="1ae4e-129">类型</span><span class="sxs-lookup"><span data-stu-id="1ae4e-129">Type</span></span>|<span data-ttu-id="1ae4e-130">说明</span><span class="sxs-lookup"><span data-stu-id="1ae4e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ae4e-131">id</span><span class="sxs-lookup"><span data-stu-id="1ae4e-131">id</span></span>|<span data-ttu-id="1ae4e-132">字符串</span><span class="sxs-lookup"><span data-stu-id="1ae4e-132">String</span></span>|<span data-ttu-id="1ae4e-133">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识的 Id</span><span class="sxs-lookup"><span data-stu-id="1ae4e-133">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="1ae4e-134">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1ae4e-134">importedDeviceIdentifier</span></span>|<span data-ttu-id="1ae4e-135">String</span><span class="sxs-lookup"><span data-stu-id="1ae4e-135">String</span></span>|<span data-ttu-id="1ae4e-136">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识符</span><span class="sxs-lookup"><span data-stu-id="1ae4e-136">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="1ae4e-137">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="1ae4e-137">importedDeviceIdentityType</span></span>|[<span data-ttu-id="1ae4e-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="1ae4e-138">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="1ae4e-139">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识的类型。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-139">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="1ae4e-140">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-140">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="1ae4e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ae4e-141">lastModifiedDateTime</span></span>|<span data-ttu-id="1ae4e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ae4e-142">DateTimeOffset</span></span>|<span data-ttu-id="1ae4e-143">继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)的说明的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="1ae4e-143">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="1ae4e-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ae4e-144">createdDateTime</span></span>|<span data-ttu-id="1ae4e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ae4e-145">DateTimeOffset</span></span>|<span data-ttu-id="1ae4e-146">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="1ae4e-146">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="1ae4e-147">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ae4e-147">lastContactedDateTime</span></span>|<span data-ttu-id="1ae4e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ae4e-148">DateTimeOffset</span></span>|<span data-ttu-id="1ae4e-149">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="1ae4e-149">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="1ae4e-150">说明</span><span class="sxs-lookup"><span data-stu-id="1ae4e-150">description</span></span>|<span data-ttu-id="1ae4e-151">String</span><span class="sxs-lookup"><span data-stu-id="1ae4e-151">String</span></span>|<span data-ttu-id="1ae4e-152">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的说明</span><span class="sxs-lookup"><span data-stu-id="1ae4e-152">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="1ae4e-153">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="1ae4e-153">enrollmentState</span></span>|[<span data-ttu-id="1ae4e-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="1ae4e-154">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="1ae4e-155">Intune 中的设备的状态继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-155">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="1ae4e-156">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-156">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="1ae4e-157">platform</span><span class="sxs-lookup"><span data-stu-id="1ae4e-157">platform</span></span>|[<span data-ttu-id="1ae4e-158">平台</span><span class="sxs-lookup"><span data-stu-id="1ae4e-158">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="1ae4e-159">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-159">The platform of the Device.</span></span> <span data-ttu-id="1ae4e-160">继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-160">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="1ae4e-161">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="1ae4e-162">status</span><span class="sxs-lookup"><span data-stu-id="1ae4e-162">status</span></span>|<span data-ttu-id="1ae4e-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ae4e-163">Boolean</span></span>|<span data-ttu-id="1ae4e-164">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="1ae4e-164">Status of imported device identity</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ae4e-165">关系</span><span class="sxs-lookup"><span data-stu-id="1ae4e-165">Relationships</span></span>
<span data-ttu-id="1ae4e-166">无</span><span class="sxs-lookup"><span data-stu-id="1ae4e-166">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ae4e-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ae4e-167">JSON Representation</span></span>
<span data-ttu-id="1ae4e-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ae4e-168">Here is a JSON representation of the resource.</span></span>
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





