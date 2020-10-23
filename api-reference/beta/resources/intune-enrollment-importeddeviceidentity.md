---
title: importedDeviceIdentity 资源类型
description: ImportedDeviceIdentity 资源表示已为预注册配置预暂存的设备的唯一硬件标识。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d8190bd48d49658267f4a0103ff80dbcadc6af58
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727314"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="108eb-103">importedDeviceIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="108eb-103">importedDeviceIdentity resource type</span></span>

<span data-ttu-id="108eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="108eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="108eb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="108eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="108eb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="108eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="108eb-107">ImportedDeviceIdentity 资源表示已为预注册配置预暂存的设备的唯一硬件标识。</span><span class="sxs-lookup"><span data-stu-id="108eb-107">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="108eb-108">Methods</span><span class="sxs-lookup"><span data-stu-id="108eb-108">Methods</span></span>
|<span data-ttu-id="108eb-109">方法</span><span class="sxs-lookup"><span data-stu-id="108eb-109">Method</span></span>|<span data-ttu-id="108eb-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="108eb-110">Return Type</span></span>|<span data-ttu-id="108eb-111">说明</span><span class="sxs-lookup"><span data-stu-id="108eb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="108eb-112">列出 importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="108eb-112">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="108eb-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="108eb-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="108eb-114">列出 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="108eb-114">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="108eb-115">获取 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="108eb-115">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="108eb-116">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="108eb-116">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="108eb-117">读取 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="108eb-117">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="108eb-118">创建 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="108eb-118">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="108eb-119">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="108eb-119">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="108eb-120">创建新的 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="108eb-120">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="108eb-121">删除 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="108eb-121">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="108eb-122">无</span><span class="sxs-lookup"><span data-stu-id="108eb-122">None</span></span>|<span data-ttu-id="108eb-123">删除 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="108eb-123">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="108eb-124">更新 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="108eb-124">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="108eb-125">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="108eb-125">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="108eb-126">更新 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="108eb-126">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="108eb-127">importDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="108eb-127">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="108eb-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="108eb-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="108eb-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="108eb-129">Not yet documented</span></span>|
|[<span data-ttu-id="108eb-130">searchExistingIdentities 操作</span><span class="sxs-lookup"><span data-stu-id="108eb-130">searchExistingIdentities action</span></span>](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|<span data-ttu-id="108eb-131">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="108eb-131">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="108eb-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="108eb-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="108eb-133">属性</span><span class="sxs-lookup"><span data-stu-id="108eb-133">Properties</span></span>
|<span data-ttu-id="108eb-134">属性</span><span class="sxs-lookup"><span data-stu-id="108eb-134">Property</span></span>|<span data-ttu-id="108eb-135">类型</span><span class="sxs-lookup"><span data-stu-id="108eb-135">Type</span></span>|<span data-ttu-id="108eb-136">说明</span><span class="sxs-lookup"><span data-stu-id="108eb-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="108eb-137">id</span><span class="sxs-lookup"><span data-stu-id="108eb-137">id</span></span>|<span data-ttu-id="108eb-138">String</span><span class="sxs-lookup"><span data-stu-id="108eb-138">String</span></span>|<span data-ttu-id="108eb-139">导入的设备标识的 Id</span><span class="sxs-lookup"><span data-stu-id="108eb-139">Id of the imported device identity</span></span>|
|<span data-ttu-id="108eb-140">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="108eb-140">importedDeviceIdentifier</span></span>|<span data-ttu-id="108eb-141">String</span><span class="sxs-lookup"><span data-stu-id="108eb-141">String</span></span>|<span data-ttu-id="108eb-142">导入的设备标识符</span><span class="sxs-lookup"><span data-stu-id="108eb-142">Imported Device Identifier</span></span>|
|<span data-ttu-id="108eb-143">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="108eb-143">importedDeviceIdentityType</span></span>|[<span data-ttu-id="108eb-144">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="108eb-144">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="108eb-145">导入的设备标识的类型。</span><span class="sxs-lookup"><span data-stu-id="108eb-145">Type of Imported Device Identity.</span></span> <span data-ttu-id="108eb-146">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="108eb-146">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="108eb-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="108eb-147">lastModifiedDateTime</span></span>|<span data-ttu-id="108eb-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="108eb-148">DateTimeOffset</span></span>|<span data-ttu-id="108eb-149">说明的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="108eb-149">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="108eb-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="108eb-150">createdDateTime</span></span>|<span data-ttu-id="108eb-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="108eb-151">DateTimeOffset</span></span>|<span data-ttu-id="108eb-152">设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="108eb-152">Created Date Time of the device</span></span>|
|<span data-ttu-id="108eb-153">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="108eb-153">lastContactedDateTime</span></span>|<span data-ttu-id="108eb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="108eb-154">DateTimeOffset</span></span>|<span data-ttu-id="108eb-155">设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="108eb-155">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="108eb-156">说明</span><span class="sxs-lookup"><span data-stu-id="108eb-156">description</span></span>|<span data-ttu-id="108eb-157">String</span><span class="sxs-lookup"><span data-stu-id="108eb-157">String</span></span>|<span data-ttu-id="108eb-158">设备的说明</span><span class="sxs-lookup"><span data-stu-id="108eb-158">The description of the device</span></span>|
|<span data-ttu-id="108eb-159">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="108eb-159">enrollmentState</span></span>|[<span data-ttu-id="108eb-160">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="108eb-160">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="108eb-161">Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="108eb-161">The state of the device in Intune.</span></span> <span data-ttu-id="108eb-162">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="108eb-162">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="108eb-163">平台</span><span class="sxs-lookup"><span data-stu-id="108eb-163">platform</span></span>|[<span data-ttu-id="108eb-164">平台</span><span class="sxs-lookup"><span data-stu-id="108eb-164">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="108eb-165">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="108eb-165">The platform of the Device.</span></span> <span data-ttu-id="108eb-166">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="108eb-166">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="108eb-167">关系</span><span class="sxs-lookup"><span data-stu-id="108eb-167">Relationships</span></span>
<span data-ttu-id="108eb-168">无</span><span class="sxs-lookup"><span data-stu-id="108eb-168">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="108eb-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="108eb-169">JSON Representation</span></span>
<span data-ttu-id="108eb-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="108eb-170">Here is a JSON representation of the resource.</span></span>
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





