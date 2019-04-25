---
title: importedDeviceIdentity 资源类型
description: importedDeviceIdentity 资源表示已为预注册配置预暂存的设备的唯一硬件标识。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7cc903fa1b30177f037493fe090ebfde31831b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550726"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="190c9-103">importedDeviceIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="190c9-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="190c9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="190c9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="190c9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="190c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="190c9-106">importedDeviceIdentity 资源表示已为预注册配置预暂存的设备的唯一硬件标识。</span><span class="sxs-lookup"><span data-stu-id="190c9-106">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="190c9-107">方法</span><span class="sxs-lookup"><span data-stu-id="190c9-107">Methods</span></span>
|<span data-ttu-id="190c9-108">方法</span><span class="sxs-lookup"><span data-stu-id="190c9-108">Method</span></span>|<span data-ttu-id="190c9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="190c9-109">Return Type</span></span>|<span data-ttu-id="190c9-110">说明</span><span class="sxs-lookup"><span data-stu-id="190c9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="190c9-111">列出 importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="190c9-111">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="190c9-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="190c9-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="190c9-113">列出[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="190c9-113">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="190c9-114">获取 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="190c9-114">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="190c9-115">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="190c9-115">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="190c9-116">读取[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="190c9-116">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="190c9-117">创建 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="190c9-117">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="190c9-118">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="190c9-118">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="190c9-119">创建新的[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="190c9-119">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="190c9-120">删除 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="190c9-120">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="190c9-121">无</span><span class="sxs-lookup"><span data-stu-id="190c9-121">None</span></span>|<span data-ttu-id="190c9-122">删除[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="190c9-122">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="190c9-123">更新 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="190c9-123">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="190c9-124">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="190c9-124">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="190c9-125">更新[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="190c9-125">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="190c9-126">importDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="190c9-126">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="190c9-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="190c9-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="190c9-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="190c9-128">Not yet documented</span></span>|
|[<span data-ttu-id="190c9-129">searchExistingIdentities 操作</span><span class="sxs-lookup"><span data-stu-id="190c9-129">searchExistingIdentities action</span></span>](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|<span data-ttu-id="190c9-130">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="190c9-130">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="190c9-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="190c9-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="190c9-132">属性</span><span class="sxs-lookup"><span data-stu-id="190c9-132">Properties</span></span>
|<span data-ttu-id="190c9-133">属性</span><span class="sxs-lookup"><span data-stu-id="190c9-133">Property</span></span>|<span data-ttu-id="190c9-134">类型</span><span class="sxs-lookup"><span data-stu-id="190c9-134">Type</span></span>|<span data-ttu-id="190c9-135">说明</span><span class="sxs-lookup"><span data-stu-id="190c9-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="190c9-136">id</span><span class="sxs-lookup"><span data-stu-id="190c9-136">id</span></span>|<span data-ttu-id="190c9-137">字符串</span><span class="sxs-lookup"><span data-stu-id="190c9-137">String</span></span>|<span data-ttu-id="190c9-138">导入的设备标识的 Id</span><span class="sxs-lookup"><span data-stu-id="190c9-138">Id of the imported device identity</span></span>|
|<span data-ttu-id="190c9-139">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="190c9-139">importedDeviceIdentifier</span></span>|<span data-ttu-id="190c9-140">String</span><span class="sxs-lookup"><span data-stu-id="190c9-140">String</span></span>|<span data-ttu-id="190c9-141">导入的设备标识符</span><span class="sxs-lookup"><span data-stu-id="190c9-141">Imported Device Identifier</span></span>|
|<span data-ttu-id="190c9-142">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="190c9-142">importedDeviceIdentityType</span></span>|[<span data-ttu-id="190c9-143">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="190c9-143">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="190c9-144">导入的设备标识的类型。</span><span class="sxs-lookup"><span data-stu-id="190c9-144">Type of Imported Device Identity.</span></span> <span data-ttu-id="190c9-145">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="190c9-145">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="190c9-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="190c9-146">lastModifiedDateTime</span></span>|<span data-ttu-id="190c9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="190c9-147">DateTimeOffset</span></span>|<span data-ttu-id="190c9-148">说明的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="190c9-148">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="190c9-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="190c9-149">createdDateTime</span></span>|<span data-ttu-id="190c9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="190c9-150">DateTimeOffset</span></span>|<span data-ttu-id="190c9-151">设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="190c9-151">Created Date Time of the device</span></span>|
|<span data-ttu-id="190c9-152">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="190c9-152">lastContactedDateTime</span></span>|<span data-ttu-id="190c9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="190c9-153">DateTimeOffset</span></span>|<span data-ttu-id="190c9-154">设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="190c9-154">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="190c9-155">description</span><span class="sxs-lookup"><span data-stu-id="190c9-155">description</span></span>|<span data-ttu-id="190c9-156">String</span><span class="sxs-lookup"><span data-stu-id="190c9-156">String</span></span>|<span data-ttu-id="190c9-157">设备的说明</span><span class="sxs-lookup"><span data-stu-id="190c9-157">The description of the device</span></span>|
|<span data-ttu-id="190c9-158">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="190c9-158">enrollmentState</span></span>|[<span data-ttu-id="190c9-159">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="190c9-159">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="190c9-160">Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="190c9-160">The state of the device in Intune.</span></span> <span data-ttu-id="190c9-161">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="190c9-161">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="190c9-162">platform</span><span class="sxs-lookup"><span data-stu-id="190c9-162">platform</span></span>|[<span data-ttu-id="190c9-163">平台</span><span class="sxs-lookup"><span data-stu-id="190c9-163">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="190c9-164">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="190c9-164">The platform of the Device.</span></span> <span data-ttu-id="190c9-165">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="190c9-165">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="190c9-166">关系</span><span class="sxs-lookup"><span data-stu-id="190c9-166">Relationships</span></span>
<span data-ttu-id="190c9-167">无</span><span class="sxs-lookup"><span data-stu-id="190c9-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="190c9-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="190c9-168">JSON Representation</span></span>
<span data-ttu-id="190c9-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="190c9-169">Here is a JSON representation of the resource.</span></span>
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





