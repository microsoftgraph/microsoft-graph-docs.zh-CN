---
title: importedDeviceIdentity 资源类型
description: importedDeviceIdentity 资源表示已为预注册配置预暂存的设备的唯一硬件标识。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7ef77b550060d5544a6ee0eda4e6b11923d3571
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151224"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="3f8f6-103">importedDeviceIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f8f6-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="3f8f6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f8f6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f8f6-106">importedDeviceIdentity 资源表示已为预注册配置预暂存的设备的唯一硬件标识。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-106">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="3f8f6-107">方法</span><span class="sxs-lookup"><span data-stu-id="3f8f6-107">Methods</span></span>
|<span data-ttu-id="3f8f6-108">方法</span><span class="sxs-lookup"><span data-stu-id="3f8f6-108">Method</span></span>|<span data-ttu-id="3f8f6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f8f6-109">Return Type</span></span>|<span data-ttu-id="3f8f6-110">说明</span><span class="sxs-lookup"><span data-stu-id="3f8f6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3f8f6-111">列出 importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="3f8f6-111">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="3f8f6-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f8f6-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="3f8f6-113">列出[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-113">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="3f8f6-114">获取 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="3f8f6-114">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="3f8f6-115">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="3f8f6-115">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="3f8f6-116">读取[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-116">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="3f8f6-117">创建 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="3f8f6-117">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="3f8f6-118">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="3f8f6-118">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="3f8f6-119">创建新的[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-119">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="3f8f6-120">删除 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="3f8f6-120">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="3f8f6-121">无</span><span class="sxs-lookup"><span data-stu-id="3f8f6-121">None</span></span>|<span data-ttu-id="3f8f6-122">删除[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-122">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="3f8f6-123">更新 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="3f8f6-123">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="3f8f6-124">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="3f8f6-124">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="3f8f6-125">更新[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-125">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="3f8f6-126">importDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="3f8f6-126">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="3f8f6-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f8f6-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="3f8f6-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3f8f6-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3f8f6-129">属性</span><span class="sxs-lookup"><span data-stu-id="3f8f6-129">Properties</span></span>
|<span data-ttu-id="3f8f6-130">属性</span><span class="sxs-lookup"><span data-stu-id="3f8f6-130">Property</span></span>|<span data-ttu-id="3f8f6-131">类型</span><span class="sxs-lookup"><span data-stu-id="3f8f6-131">Type</span></span>|<span data-ttu-id="3f8f6-132">说明</span><span class="sxs-lookup"><span data-stu-id="3f8f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f8f6-133">id</span><span class="sxs-lookup"><span data-stu-id="3f8f6-133">id</span></span>|<span data-ttu-id="3f8f6-134">String</span><span class="sxs-lookup"><span data-stu-id="3f8f6-134">String</span></span>|<span data-ttu-id="3f8f6-135">导入的设备标识的 Id</span><span class="sxs-lookup"><span data-stu-id="3f8f6-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="3f8f6-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="3f8f6-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="3f8f6-137">字符串</span><span class="sxs-lookup"><span data-stu-id="3f8f6-137">String</span></span>|<span data-ttu-id="3f8f6-138">导入的设备标识符</span><span class="sxs-lookup"><span data-stu-id="3f8f6-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="3f8f6-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="3f8f6-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="3f8f6-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="3f8f6-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="3f8f6-141">导入的设备标识的类型。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="3f8f6-142">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="3f8f6-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f8f6-143">lastModifiedDateTime</span></span>|<span data-ttu-id="3f8f6-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f8f6-144">DateTimeOffset</span></span>|<span data-ttu-id="3f8f6-145">说明的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="3f8f6-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="3f8f6-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f8f6-146">createdDateTime</span></span>|<span data-ttu-id="3f8f6-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f8f6-147">DateTimeOffset</span></span>|<span data-ttu-id="3f8f6-148">设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="3f8f6-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="3f8f6-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f8f6-149">lastContactedDateTime</span></span>|<span data-ttu-id="3f8f6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f8f6-150">DateTimeOffset</span></span>|<span data-ttu-id="3f8f6-151">设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="3f8f6-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="3f8f6-152">说明</span><span class="sxs-lookup"><span data-stu-id="3f8f6-152">description</span></span>|<span data-ttu-id="3f8f6-153">字符串</span><span class="sxs-lookup"><span data-stu-id="3f8f6-153">String</span></span>|<span data-ttu-id="3f8f6-154">设备的说明</span><span class="sxs-lookup"><span data-stu-id="3f8f6-154">The description of the device</span></span>|
|<span data-ttu-id="3f8f6-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="3f8f6-155">enrollmentState</span></span>|[<span data-ttu-id="3f8f6-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="3f8f6-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="3f8f6-157">Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-157">The state of the device in Intune.</span></span> <span data-ttu-id="3f8f6-158">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="3f8f6-159">platform</span><span class="sxs-lookup"><span data-stu-id="3f8f6-159">platform</span></span>|[<span data-ttu-id="3f8f6-160">平台</span><span class="sxs-lookup"><span data-stu-id="3f8f6-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="3f8f6-161">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-161">The platform of the Device.</span></span> <span data-ttu-id="3f8f6-162">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f8f6-163">关系</span><span class="sxs-lookup"><span data-stu-id="3f8f6-163">Relationships</span></span>
<span data-ttu-id="3f8f6-164">无</span><span class="sxs-lookup"><span data-stu-id="3f8f6-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f8f6-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f8f6-165">JSON Representation</span></span>
<span data-ttu-id="3f8f6-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f8f6-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```




