---
title: importedDeviceIdentityResult 资源类型
description: ImportedDeviceIdentityResult 资源表示尝试导入设备标识的结果。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9a1597e66de0e518ecb30ec889f6fde063e35a17
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727307"
---
# <a name="importeddeviceidentityresult-resource-type"></a><span data-ttu-id="143a9-103">importedDeviceIdentityResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="143a9-103">importedDeviceIdentityResult resource type</span></span>

<span data-ttu-id="143a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="143a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="143a9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="143a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="143a9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="143a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="143a9-107">ImportedDeviceIdentityResult 资源表示尝试导入设备标识的结果。</span><span class="sxs-lookup"><span data-stu-id="143a9-107">The importedDeviceIdentityResult resource represents the result of attempting to import a device identity.</span></span>


<span data-ttu-id="143a9-108">继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="143a9-108">Inherits from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>

## <a name="methods"></a><span data-ttu-id="143a9-109">Methods</span><span class="sxs-lookup"><span data-stu-id="143a9-109">Methods</span></span>
|<span data-ttu-id="143a9-110">方法</span><span class="sxs-lookup"><span data-stu-id="143a9-110">Method</span></span>|<span data-ttu-id="143a9-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="143a9-111">Return Type</span></span>|<span data-ttu-id="143a9-112">说明</span><span class="sxs-lookup"><span data-stu-id="143a9-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="143a9-113">列出 importedDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="143a9-113">List importedDeviceIdentityResults</span></span>](../api/intune-enrollment-importeddeviceidentityresult-list.md)|<span data-ttu-id="143a9-114">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="143a9-114">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="143a9-115">列出 [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="143a9-115">List properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects.</span></span>|
|[<span data-ttu-id="143a9-116">获取 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="143a9-116">Get importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[<span data-ttu-id="143a9-117">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="143a9-117">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="143a9-118">读取 [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="143a9-118">Read properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="143a9-119">创建 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="143a9-119">Create importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[<span data-ttu-id="143a9-120">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="143a9-120">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="143a9-121">创建新的 [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="143a9-121">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="143a9-122">删除 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="143a9-122">Delete importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|<span data-ttu-id="143a9-123">无</span><span class="sxs-lookup"><span data-stu-id="143a9-123">None</span></span>|<span data-ttu-id="143a9-124">删除 [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)。</span><span class="sxs-lookup"><span data-stu-id="143a9-124">Deletes a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>|
|[<span data-ttu-id="143a9-125">更新 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="143a9-125">Update importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[<span data-ttu-id="143a9-126">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="143a9-126">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="143a9-127">更新 [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="143a9-127">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="143a9-128">属性</span><span class="sxs-lookup"><span data-stu-id="143a9-128">Properties</span></span>
|<span data-ttu-id="143a9-129">属性</span><span class="sxs-lookup"><span data-stu-id="143a9-129">Property</span></span>|<span data-ttu-id="143a9-130">类型</span><span class="sxs-lookup"><span data-stu-id="143a9-130">Type</span></span>|<span data-ttu-id="143a9-131">说明</span><span class="sxs-lookup"><span data-stu-id="143a9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="143a9-132">id</span><span class="sxs-lookup"><span data-stu-id="143a9-132">id</span></span>|<span data-ttu-id="143a9-133">String</span><span class="sxs-lookup"><span data-stu-id="143a9-133">String</span></span>|<span data-ttu-id="143a9-134">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识的 Id</span><span class="sxs-lookup"><span data-stu-id="143a9-134">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="143a9-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="143a9-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="143a9-136">String</span><span class="sxs-lookup"><span data-stu-id="143a9-136">String</span></span>|<span data-ttu-id="143a9-137">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识符</span><span class="sxs-lookup"><span data-stu-id="143a9-137">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="143a9-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="143a9-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="143a9-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="143a9-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="143a9-140">从 [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识的类型。</span><span class="sxs-lookup"><span data-stu-id="143a9-140">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="143a9-141">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="143a9-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="143a9-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="143a9-142">lastModifiedDateTime</span></span>|<span data-ttu-id="143a9-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="143a9-143">DateTimeOffset</span></span>|<span data-ttu-id="143a9-144">继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)的说明的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="143a9-144">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="143a9-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="143a9-145">createdDateTime</span></span>|<span data-ttu-id="143a9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="143a9-146">DateTimeOffset</span></span>|<span data-ttu-id="143a9-147">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="143a9-147">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="143a9-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="143a9-148">lastContactedDateTime</span></span>|<span data-ttu-id="143a9-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="143a9-149">DateTimeOffset</span></span>|<span data-ttu-id="143a9-150">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="143a9-150">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="143a9-151">说明</span><span class="sxs-lookup"><span data-stu-id="143a9-151">description</span></span>|<span data-ttu-id="143a9-152">String</span><span class="sxs-lookup"><span data-stu-id="143a9-152">String</span></span>|<span data-ttu-id="143a9-153">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的说明</span><span class="sxs-lookup"><span data-stu-id="143a9-153">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="143a9-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="143a9-154">enrollmentState</span></span>|[<span data-ttu-id="143a9-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="143a9-155">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="143a9-156">Intune 中的设备的状态继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="143a9-156">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="143a9-157">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="143a9-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="143a9-158">平台</span><span class="sxs-lookup"><span data-stu-id="143a9-158">platform</span></span>|[<span data-ttu-id="143a9-159">平台</span><span class="sxs-lookup"><span data-stu-id="143a9-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="143a9-160">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="143a9-160">The platform of the Device.</span></span> <span data-ttu-id="143a9-161">继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="143a9-161">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="143a9-162">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="143a9-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="143a9-163">status</span><span class="sxs-lookup"><span data-stu-id="143a9-163">status</span></span>|<span data-ttu-id="143a9-164">布尔</span><span class="sxs-lookup"><span data-stu-id="143a9-164">Boolean</span></span>|<span data-ttu-id="143a9-165">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="143a9-165">Status of imported device identity</span></span>|

## <a name="relationships"></a><span data-ttu-id="143a9-166">关系</span><span class="sxs-lookup"><span data-stu-id="143a9-166">Relationships</span></span>
<span data-ttu-id="143a9-167">无</span><span class="sxs-lookup"><span data-stu-id="143a9-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="143a9-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="143a9-168">JSON Representation</span></span>
<span data-ttu-id="143a9-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="143a9-169">Here is a JSON representation of the resource.</span></span>
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





