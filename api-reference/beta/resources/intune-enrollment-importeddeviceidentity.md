---
title: importedDeviceIdentity 资源类型
description: ImportedDeviceIdentity 资源表示预注册配置已预暂存设备的唯一的硬件标识。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c151257a95d1161e07de17ed6d9fc01fc021146e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421443"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="f463c-103">importedDeviceIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="f463c-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="f463c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f463c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f463c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f463c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f463c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f463c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f463c-107">ImportedDeviceIdentity 资源表示预注册配置已预暂存设备的唯一的硬件标识。</span><span class="sxs-lookup"><span data-stu-id="f463c-107">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="f463c-108">方法</span><span class="sxs-lookup"><span data-stu-id="f463c-108">Methods</span></span>
|<span data-ttu-id="f463c-109">方法</span><span class="sxs-lookup"><span data-stu-id="f463c-109">Method</span></span>|<span data-ttu-id="f463c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f463c-110">Return Type</span></span>|<span data-ttu-id="f463c-111">说明</span><span class="sxs-lookup"><span data-stu-id="f463c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f463c-112">列表 importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="f463c-112">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="f463c-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="f463c-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="f463c-114">列出属性和[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="f463c-114">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="f463c-115">获取 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f463c-115">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="f463c-116">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f463c-116">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="f463c-117">读取属性和[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="f463c-117">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="f463c-118">创建 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f463c-118">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="f463c-119">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f463c-119">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="f463c-120">创建新的[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f463c-120">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="f463c-121">删除 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f463c-121">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="f463c-122">无</span><span class="sxs-lookup"><span data-stu-id="f463c-122">None</span></span>|<span data-ttu-id="f463c-123">删除[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="f463c-123">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="f463c-124">更新 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f463c-124">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="f463c-125">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f463c-125">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="f463c-126">更新[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f463c-126">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="f463c-127">importDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="f463c-127">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="f463c-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="f463c-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="f463c-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f463c-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f463c-130">属性</span><span class="sxs-lookup"><span data-stu-id="f463c-130">Properties</span></span>
|<span data-ttu-id="f463c-131">属性</span><span class="sxs-lookup"><span data-stu-id="f463c-131">Property</span></span>|<span data-ttu-id="f463c-132">类型</span><span class="sxs-lookup"><span data-stu-id="f463c-132">Type</span></span>|<span data-ttu-id="f463c-133">说明</span><span class="sxs-lookup"><span data-stu-id="f463c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f463c-134">id</span><span class="sxs-lookup"><span data-stu-id="f463c-134">id</span></span>|<span data-ttu-id="f463c-135">String</span><span class="sxs-lookup"><span data-stu-id="f463c-135">String</span></span>|<span data-ttu-id="f463c-136">导入的设备标识的 id</span><span class="sxs-lookup"><span data-stu-id="f463c-136">Id of the imported device identity</span></span>|
|<span data-ttu-id="f463c-137">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f463c-137">importedDeviceIdentifier</span></span>|<span data-ttu-id="f463c-138">String</span><span class="sxs-lookup"><span data-stu-id="f463c-138">String</span></span>|<span data-ttu-id="f463c-139">导入的设备标识符</span><span class="sxs-lookup"><span data-stu-id="f463c-139">Imported Device Identifier</span></span>|
|<span data-ttu-id="f463c-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="f463c-140">importedDeviceIdentityType</span></span>|[<span data-ttu-id="f463c-141">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="f463c-141">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="f463c-142">导入的设备的标识的类型。</span><span class="sxs-lookup"><span data-stu-id="f463c-142">Type of Imported Device Identity.</span></span> <span data-ttu-id="f463c-143">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="f463c-143">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="f463c-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f463c-144">lastModifiedDateTime</span></span>|<span data-ttu-id="f463c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f463c-145">DateTimeOffset</span></span>|<span data-ttu-id="f463c-146">上次修改日期时间的说明</span><span class="sxs-lookup"><span data-stu-id="f463c-146">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="f463c-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f463c-147">createdDateTime</span></span>|<span data-ttu-id="f463c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f463c-148">DateTimeOffset</span></span>|<span data-ttu-id="f463c-149">设备的创建的日期时间</span><span class="sxs-lookup"><span data-stu-id="f463c-149">Created Date Time of the device</span></span>|
|<span data-ttu-id="f463c-150">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="f463c-150">lastContactedDateTime</span></span>|<span data-ttu-id="f463c-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f463c-151">DateTimeOffset</span></span>|<span data-ttu-id="f463c-152">设备的最后一个联系日期时间</span><span class="sxs-lookup"><span data-stu-id="f463c-152">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="f463c-153">说明</span><span class="sxs-lookup"><span data-stu-id="f463c-153">description</span></span>|<span data-ttu-id="f463c-154">String</span><span class="sxs-lookup"><span data-stu-id="f463c-154">String</span></span>|<span data-ttu-id="f463c-155">设备的说明</span><span class="sxs-lookup"><span data-stu-id="f463c-155">The description of the device</span></span>|
|<span data-ttu-id="f463c-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="f463c-156">enrollmentState</span></span>|[<span data-ttu-id="f463c-157">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="f463c-157">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="f463c-158">在 Intune 设备的状态。</span><span class="sxs-lookup"><span data-stu-id="f463c-158">The state of the device in Intune.</span></span> <span data-ttu-id="f463c-159">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="f463c-159">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="f463c-160">platform</span><span class="sxs-lookup"><span data-stu-id="f463c-160">platform</span></span>|[<span data-ttu-id="f463c-161">平台</span><span class="sxs-lookup"><span data-stu-id="f463c-161">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="f463c-162">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="f463c-162">The platform of the Device.</span></span> <span data-ttu-id="f463c-163">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="f463c-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f463c-164">关系</span><span class="sxs-lookup"><span data-stu-id="f463c-164">Relationships</span></span>
<span data-ttu-id="f463c-165">无</span><span class="sxs-lookup"><span data-stu-id="f463c-165">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f463c-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f463c-166">JSON Representation</span></span>
<span data-ttu-id="f463c-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f463c-167">Here is a JSON representation of the resource.</span></span>
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




