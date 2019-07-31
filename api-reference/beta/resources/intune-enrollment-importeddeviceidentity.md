---
title: importedDeviceIdentity 资源类型
description: ImportedDeviceIdentity 资源表示已为预注册配置预暂存的设备的唯一硬件标识。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 24b1e939053a49deca34c89bf61750493495bb8c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999134"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="2cffc-103">importedDeviceIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="2cffc-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="2cffc-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2cffc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cffc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2cffc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cffc-106">ImportedDeviceIdentity 资源表示已为预注册配置预暂存的设备的唯一硬件标识。</span><span class="sxs-lookup"><span data-stu-id="2cffc-106">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="2cffc-107">方法</span><span class="sxs-lookup"><span data-stu-id="2cffc-107">Methods</span></span>
|<span data-ttu-id="2cffc-108">方法</span><span class="sxs-lookup"><span data-stu-id="2cffc-108">Method</span></span>|<span data-ttu-id="2cffc-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2cffc-109">Return Type</span></span>|<span data-ttu-id="2cffc-110">说明</span><span class="sxs-lookup"><span data-stu-id="2cffc-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2cffc-111">列出 importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="2cffc-111">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="2cffc-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="2cffc-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="2cffc-113">列出[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2cffc-113">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="2cffc-114">获取 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2cffc-114">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="2cffc-115">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2cffc-115">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="2cffc-116">读取[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2cffc-116">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="2cffc-117">创建 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2cffc-117">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="2cffc-118">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2cffc-118">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="2cffc-119">创建新的[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2cffc-119">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="2cffc-120">删除 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2cffc-120">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="2cffc-121">无</span><span class="sxs-lookup"><span data-stu-id="2cffc-121">None</span></span>|<span data-ttu-id="2cffc-122">删除[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="2cffc-122">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="2cffc-123">更新 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2cffc-123">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="2cffc-124">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2cffc-124">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="2cffc-125">更新[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2cffc-125">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="2cffc-126">importDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="2cffc-126">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="2cffc-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="2cffc-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="2cffc-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2cffc-128">Not yet documented</span></span>|
|[<span data-ttu-id="2cffc-129">searchExistingIdentities 操作</span><span class="sxs-lookup"><span data-stu-id="2cffc-129">searchExistingIdentities action</span></span>](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|<span data-ttu-id="2cffc-130">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="2cffc-130">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="2cffc-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2cffc-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2cffc-132">属性</span><span class="sxs-lookup"><span data-stu-id="2cffc-132">Properties</span></span>
|<span data-ttu-id="2cffc-133">属性</span><span class="sxs-lookup"><span data-stu-id="2cffc-133">Property</span></span>|<span data-ttu-id="2cffc-134">类型</span><span class="sxs-lookup"><span data-stu-id="2cffc-134">Type</span></span>|<span data-ttu-id="2cffc-135">说明</span><span class="sxs-lookup"><span data-stu-id="2cffc-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cffc-136">id</span><span class="sxs-lookup"><span data-stu-id="2cffc-136">id</span></span>|<span data-ttu-id="2cffc-137">字符串</span><span class="sxs-lookup"><span data-stu-id="2cffc-137">String</span></span>|<span data-ttu-id="2cffc-138">导入的设备标识的 Id</span><span class="sxs-lookup"><span data-stu-id="2cffc-138">Id of the imported device identity</span></span>|
|<span data-ttu-id="2cffc-139">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="2cffc-139">importedDeviceIdentifier</span></span>|<span data-ttu-id="2cffc-140">String</span><span class="sxs-lookup"><span data-stu-id="2cffc-140">String</span></span>|<span data-ttu-id="2cffc-141">导入的设备标识符</span><span class="sxs-lookup"><span data-stu-id="2cffc-141">Imported Device Identifier</span></span>|
|<span data-ttu-id="2cffc-142">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="2cffc-142">importedDeviceIdentityType</span></span>|[<span data-ttu-id="2cffc-143">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="2cffc-143">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="2cffc-144">导入的设备标识的类型。</span><span class="sxs-lookup"><span data-stu-id="2cffc-144">Type of Imported Device Identity.</span></span> <span data-ttu-id="2cffc-145">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="2cffc-145">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="2cffc-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2cffc-146">lastModifiedDateTime</span></span>|<span data-ttu-id="2cffc-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cffc-147">DateTimeOffset</span></span>|<span data-ttu-id="2cffc-148">说明的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="2cffc-148">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="2cffc-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2cffc-149">createdDateTime</span></span>|<span data-ttu-id="2cffc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cffc-150">DateTimeOffset</span></span>|<span data-ttu-id="2cffc-151">设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="2cffc-151">Created Date Time of the device</span></span>|
|<span data-ttu-id="2cffc-152">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="2cffc-152">lastContactedDateTime</span></span>|<span data-ttu-id="2cffc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cffc-153">DateTimeOffset</span></span>|<span data-ttu-id="2cffc-154">设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="2cffc-154">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="2cffc-155">说明</span><span class="sxs-lookup"><span data-stu-id="2cffc-155">description</span></span>|<span data-ttu-id="2cffc-156">String</span><span class="sxs-lookup"><span data-stu-id="2cffc-156">String</span></span>|<span data-ttu-id="2cffc-157">设备的说明</span><span class="sxs-lookup"><span data-stu-id="2cffc-157">The description of the device</span></span>|
|<span data-ttu-id="2cffc-158">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="2cffc-158">enrollmentState</span></span>|[<span data-ttu-id="2cffc-159">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="2cffc-159">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="2cffc-160">Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="2cffc-160">The state of the device in Intune.</span></span> <span data-ttu-id="2cffc-161">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="2cffc-161">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="2cffc-162">platform</span><span class="sxs-lookup"><span data-stu-id="2cffc-162">platform</span></span>|[<span data-ttu-id="2cffc-163">平台</span><span class="sxs-lookup"><span data-stu-id="2cffc-163">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="2cffc-164">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="2cffc-164">The platform of the Device.</span></span> <span data-ttu-id="2cffc-165">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="2cffc-165">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cffc-166">关系</span><span class="sxs-lookup"><span data-stu-id="2cffc-166">Relationships</span></span>
<span data-ttu-id="2cffc-167">无</span><span class="sxs-lookup"><span data-stu-id="2cffc-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cffc-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cffc-168">JSON Representation</span></span>
<span data-ttu-id="2cffc-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2cffc-169">Here is a JSON representation of the resource.</span></span>
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





