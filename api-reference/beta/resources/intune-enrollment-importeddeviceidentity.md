---
title: importedDeviceIdentity 资源类型
description: ImportedDeviceIdentity 资源表示预注册配置已预暂存设备的唯一的硬件标识。
ms.openlocfilehash: a327840ce38dfd0d075ef37c7e92ef0e83b2054c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048953"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="39b60-103">importedDeviceIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="39b60-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="39b60-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="39b60-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39b60-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="39b60-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39b60-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="39b60-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39b60-107">ImportedDeviceIdentity 资源表示预注册配置已预暂存设备的唯一的硬件标识。</span><span class="sxs-lookup"><span data-stu-id="39b60-107">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="39b60-108">方法</span><span class="sxs-lookup"><span data-stu-id="39b60-108">Methods</span></span>
|<span data-ttu-id="39b60-109">方法</span><span class="sxs-lookup"><span data-stu-id="39b60-109">Method</span></span>|<span data-ttu-id="39b60-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="39b60-110">Return Type</span></span>|<span data-ttu-id="39b60-111">说明</span><span class="sxs-lookup"><span data-stu-id="39b60-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39b60-112">列表 importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="39b60-112">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="39b60-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="39b60-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="39b60-114">列出属性和[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="39b60-114">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="39b60-115">获取 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="39b60-115">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="39b60-116">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="39b60-116">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="39b60-117">读取属性和[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="39b60-117">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="39b60-118">创建 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="39b60-118">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="39b60-119">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="39b60-119">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="39b60-120">创建新的[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="39b60-120">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="39b60-121">删除 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="39b60-121">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="39b60-122">无</span><span class="sxs-lookup"><span data-stu-id="39b60-122">None</span></span>|<span data-ttu-id="39b60-123">删除[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="39b60-123">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="39b60-124">更新 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="39b60-124">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="39b60-125">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="39b60-125">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="39b60-126">更新[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="39b60-126">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="39b60-127">importDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="39b60-127">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="39b60-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="39b60-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="39b60-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="39b60-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="39b60-130">属性</span><span class="sxs-lookup"><span data-stu-id="39b60-130">Properties</span></span>
|<span data-ttu-id="39b60-131">属性</span><span class="sxs-lookup"><span data-stu-id="39b60-131">Property</span></span>|<span data-ttu-id="39b60-132">类型</span><span class="sxs-lookup"><span data-stu-id="39b60-132">Type</span></span>|<span data-ttu-id="39b60-133">说明</span><span class="sxs-lookup"><span data-stu-id="39b60-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39b60-134">id</span><span class="sxs-lookup"><span data-stu-id="39b60-134">id</span></span>|<span data-ttu-id="39b60-135">字符串</span><span class="sxs-lookup"><span data-stu-id="39b60-135">String</span></span>|<span data-ttu-id="39b60-136">导入的设备标识的 id</span><span class="sxs-lookup"><span data-stu-id="39b60-136">Id of the imported device identity</span></span>|
|<span data-ttu-id="39b60-137">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="39b60-137">importedDeviceIdentifier</span></span>|<span data-ttu-id="39b60-138">字符串</span><span class="sxs-lookup"><span data-stu-id="39b60-138">String</span></span>|<span data-ttu-id="39b60-139">导入的设备标识符</span><span class="sxs-lookup"><span data-stu-id="39b60-139">Imported Device Identifier</span></span>|
|<span data-ttu-id="39b60-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="39b60-140">importedDeviceIdentityType</span></span>|[<span data-ttu-id="39b60-141">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="39b60-141">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="39b60-142">导入的设备的标识的类型。</span><span class="sxs-lookup"><span data-stu-id="39b60-142">Type of Imported Device Identity.</span></span> <span data-ttu-id="39b60-143">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="39b60-143">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="39b60-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39b60-144">lastModifiedDateTime</span></span>|<span data-ttu-id="39b60-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39b60-145">DateTimeOffset</span></span>|<span data-ttu-id="39b60-146">上次修改日期时间的说明</span><span class="sxs-lookup"><span data-stu-id="39b60-146">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="39b60-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39b60-147">createdDateTime</span></span>|<span data-ttu-id="39b60-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39b60-148">DateTimeOffset</span></span>|<span data-ttu-id="39b60-149">设备的创建的日期时间</span><span class="sxs-lookup"><span data-stu-id="39b60-149">Created Date Time of the device</span></span>|
|<span data-ttu-id="39b60-150">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="39b60-150">lastContactedDateTime</span></span>|<span data-ttu-id="39b60-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39b60-151">DateTimeOffset</span></span>|<span data-ttu-id="39b60-152">设备的最后一个联系日期时间</span><span class="sxs-lookup"><span data-stu-id="39b60-152">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="39b60-153">说明</span><span class="sxs-lookup"><span data-stu-id="39b60-153">description</span></span>|<span data-ttu-id="39b60-154">字符串</span><span class="sxs-lookup"><span data-stu-id="39b60-154">String</span></span>|<span data-ttu-id="39b60-155">设备的说明</span><span class="sxs-lookup"><span data-stu-id="39b60-155">The description of the device</span></span>|
|<span data-ttu-id="39b60-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="39b60-156">enrollmentState</span></span>|[<span data-ttu-id="39b60-157">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="39b60-157">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="39b60-158">在 Intune 设备的状态。</span><span class="sxs-lookup"><span data-stu-id="39b60-158">The state of the device in Intune.</span></span> <span data-ttu-id="39b60-159">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="39b60-159">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="39b60-160">platform</span><span class="sxs-lookup"><span data-stu-id="39b60-160">platform</span></span>|[<span data-ttu-id="39b60-161">平台</span><span class="sxs-lookup"><span data-stu-id="39b60-161">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="39b60-162">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="39b60-162">The platform of the Device.</span></span> <span data-ttu-id="39b60-163">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="39b60-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39b60-164">Relationships</span><span class="sxs-lookup"><span data-stu-id="39b60-164">Relationships</span></span>
<span data-ttu-id="39b60-165">无</span><span class="sxs-lookup"><span data-stu-id="39b60-165">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="39b60-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39b60-166">JSON Representation</span></span>
<span data-ttu-id="39b60-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39b60-167">Here is a JSON representation of the resource.</span></span>
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





