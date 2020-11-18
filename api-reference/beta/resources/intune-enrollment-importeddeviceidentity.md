---
title: importedDeviceIdentity 资源类型
description: ImportedDeviceIdentity 资源表示已为预注册配置预暂存的设备的唯一硬件标识。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 62e63e398bb04ca201ab5f61ff3fbe029dafcaab
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49198120"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="8e2a8-103">importedDeviceIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e2a8-103">importedDeviceIdentity resource type</span></span>

<span data-ttu-id="8e2a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e2a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e2a8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e2a8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e2a8-107">ImportedDeviceIdentity 资源表示已为预注册配置预暂存的设备的唯一硬件标识。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-107">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="8e2a8-108">方法</span><span class="sxs-lookup"><span data-stu-id="8e2a8-108">Methods</span></span>
|<span data-ttu-id="8e2a8-109">方法</span><span class="sxs-lookup"><span data-stu-id="8e2a8-109">Method</span></span>|<span data-ttu-id="8e2a8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8e2a8-110">Return Type</span></span>|<span data-ttu-id="8e2a8-111">说明</span><span class="sxs-lookup"><span data-stu-id="8e2a8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8e2a8-112">列出 importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="8e2a8-112">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="8e2a8-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8e2a8-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="8e2a8-114">列出 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-114">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="8e2a8-115">获取 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="8e2a8-115">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="8e2a8-116">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="8e2a8-116">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="8e2a8-117">读取 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-117">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="8e2a8-118">创建 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="8e2a8-118">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="8e2a8-119">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="8e2a8-119">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="8e2a8-120">创建新的 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-120">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="8e2a8-121">删除 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="8e2a8-121">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="8e2a8-122">无</span><span class="sxs-lookup"><span data-stu-id="8e2a8-122">None</span></span>|<span data-ttu-id="8e2a8-123">删除 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-123">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="8e2a8-124">更新 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="8e2a8-124">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="8e2a8-125">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="8e2a8-125">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="8e2a8-126">更新 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-126">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="8e2a8-127">importDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="8e2a8-127">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="8e2a8-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8e2a8-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="8e2a8-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8e2a8-129">Not yet documented</span></span>|
|[<span data-ttu-id="8e2a8-130">searchExistingIdentities 操作</span><span class="sxs-lookup"><span data-stu-id="8e2a8-130">searchExistingIdentities action</span></span>](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|<span data-ttu-id="8e2a8-131">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8e2a8-131">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="8e2a8-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8e2a8-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8e2a8-133">属性</span><span class="sxs-lookup"><span data-stu-id="8e2a8-133">Properties</span></span>
|<span data-ttu-id="8e2a8-134">属性</span><span class="sxs-lookup"><span data-stu-id="8e2a8-134">Property</span></span>|<span data-ttu-id="8e2a8-135">类型</span><span class="sxs-lookup"><span data-stu-id="8e2a8-135">Type</span></span>|<span data-ttu-id="8e2a8-136">说明</span><span class="sxs-lookup"><span data-stu-id="8e2a8-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e2a8-137">id</span><span class="sxs-lookup"><span data-stu-id="8e2a8-137">id</span></span>|<span data-ttu-id="8e2a8-138">String</span><span class="sxs-lookup"><span data-stu-id="8e2a8-138">String</span></span>|<span data-ttu-id="8e2a8-139">导入的设备标识的 Id</span><span class="sxs-lookup"><span data-stu-id="8e2a8-139">Id of the imported device identity</span></span>|
|<span data-ttu-id="8e2a8-140">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="8e2a8-140">importedDeviceIdentifier</span></span>|<span data-ttu-id="8e2a8-141">String</span><span class="sxs-lookup"><span data-stu-id="8e2a8-141">String</span></span>|<span data-ttu-id="8e2a8-142">导入的设备标识符</span><span class="sxs-lookup"><span data-stu-id="8e2a8-142">Imported Device Identifier</span></span>|
|<span data-ttu-id="8e2a8-143">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="8e2a8-143">importedDeviceIdentityType</span></span>|[<span data-ttu-id="8e2a8-144">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="8e2a8-144">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="8e2a8-145">导入的设备标识的类型。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-145">Type of Imported Device Identity.</span></span> <span data-ttu-id="8e2a8-146">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-146">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="8e2a8-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e2a8-147">lastModifiedDateTime</span></span>|<span data-ttu-id="8e2a8-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e2a8-148">DateTimeOffset</span></span>|<span data-ttu-id="8e2a8-149">说明的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="8e2a8-149">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="8e2a8-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e2a8-150">createdDateTime</span></span>|<span data-ttu-id="8e2a8-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e2a8-151">DateTimeOffset</span></span>|<span data-ttu-id="8e2a8-152">设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="8e2a8-152">Created Date Time of the device</span></span>|
|<span data-ttu-id="8e2a8-153">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e2a8-153">lastContactedDateTime</span></span>|<span data-ttu-id="8e2a8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e2a8-154">DateTimeOffset</span></span>|<span data-ttu-id="8e2a8-155">设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="8e2a8-155">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="8e2a8-156">description</span><span class="sxs-lookup"><span data-stu-id="8e2a8-156">description</span></span>|<span data-ttu-id="8e2a8-157">String</span><span class="sxs-lookup"><span data-stu-id="8e2a8-157">String</span></span>|<span data-ttu-id="8e2a8-158">设备的说明</span><span class="sxs-lookup"><span data-stu-id="8e2a8-158">The description of the device</span></span>|
|<span data-ttu-id="8e2a8-159">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="8e2a8-159">enrollmentState</span></span>|[<span data-ttu-id="8e2a8-160">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="8e2a8-160">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="8e2a8-161">Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-161">The state of the device in Intune.</span></span> <span data-ttu-id="8e2a8-162">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-162">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="8e2a8-163">平台</span><span class="sxs-lookup"><span data-stu-id="8e2a8-163">platform</span></span>|[<span data-ttu-id="8e2a8-164">平台</span><span class="sxs-lookup"><span data-stu-id="8e2a8-164">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="8e2a8-165">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-165">The platform of the Device.</span></span> <span data-ttu-id="8e2a8-166">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-166">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e2a8-167">关系</span><span class="sxs-lookup"><span data-stu-id="8e2a8-167">Relationships</span></span>
<span data-ttu-id="8e2a8-168">无</span><span class="sxs-lookup"><span data-stu-id="8e2a8-168">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e2a8-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e2a8-169">JSON Representation</span></span>
<span data-ttu-id="8e2a8-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e2a8-170">Here is a JSON representation of the resource.</span></span>
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




