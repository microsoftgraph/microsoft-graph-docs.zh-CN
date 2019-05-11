---
title: 更新 importedDeviceIdentityResult
description: 更新 importedDeviceIdentityResult 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f746a8a57910e42de3355c9bd0b65c73f1a2c95
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908360"
---
# <a name="update-importeddeviceidentityresult"></a><span data-ttu-id="eb9b7-103">更新 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="eb9b7-103">Update importedDeviceIdentityResult</span></span>

> <span data-ttu-id="eb9b7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb9b7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb9b7-106">更新[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-106">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb9b7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="eb9b7-107">Prerequisites</span></span>
<span data-ttu-id="eb9b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb9b7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb9b7-110">Permission type</span></span>|<span data-ttu-id="eb9b7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eb9b7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb9b7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb9b7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb9b7-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb9b7-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eb9b7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb9b7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb9b7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-115">Not supported.</span></span>|
|<span data-ttu-id="eb9b7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb9b7-116">Application</span></span>|<span data-ttu-id="eb9b7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb9b7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb9b7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="eb9b7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb9b7-119">Request headers</span></span>
|<span data-ttu-id="eb9b7-120">标头</span><span class="sxs-lookup"><span data-stu-id="eb9b7-120">Header</span></span>|<span data-ttu-id="eb9b7-121">值</span><span class="sxs-lookup"><span data-stu-id="eb9b7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb9b7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb9b7-122">Authorization</span></span>|<span data-ttu-id="eb9b7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb9b7-124">接受</span><span class="sxs-lookup"><span data-stu-id="eb9b7-124">Accept</span></span>|<span data-ttu-id="eb9b7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb9b7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb9b7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb9b7-126">Request body</span></span>
<span data-ttu-id="eb9b7-127">在请求正文中, 提供[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-127">In the request body, supply a JSON representation for the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

<span data-ttu-id="eb9b7-128">下表显示创建[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-128">The following table shows the properties that are required when you create the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>

|<span data-ttu-id="eb9b7-129">属性</span><span class="sxs-lookup"><span data-stu-id="eb9b7-129">Property</span></span>|<span data-ttu-id="eb9b7-130">类型</span><span class="sxs-lookup"><span data-stu-id="eb9b7-130">Type</span></span>|<span data-ttu-id="eb9b7-131">说明</span><span class="sxs-lookup"><span data-stu-id="eb9b7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb9b7-132">id</span><span class="sxs-lookup"><span data-stu-id="eb9b7-132">id</span></span>|<span data-ttu-id="eb9b7-133">字符串</span><span class="sxs-lookup"><span data-stu-id="eb9b7-133">String</span></span>|<span data-ttu-id="eb9b7-134">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识的 Id</span><span class="sxs-lookup"><span data-stu-id="eb9b7-134">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="eb9b7-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="eb9b7-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="eb9b7-136">String</span><span class="sxs-lookup"><span data-stu-id="eb9b7-136">String</span></span>|<span data-ttu-id="eb9b7-137">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识符</span><span class="sxs-lookup"><span data-stu-id="eb9b7-137">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="eb9b7-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="eb9b7-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="eb9b7-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="eb9b7-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="eb9b7-140">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识的类型。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-140">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="eb9b7-141">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="eb9b7-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb9b7-142">lastModifiedDateTime</span></span>|<span data-ttu-id="eb9b7-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb9b7-143">DateTimeOffset</span></span>|<span data-ttu-id="eb9b7-144">继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)的说明的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="eb9b7-144">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="eb9b7-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb9b7-145">createdDateTime</span></span>|<span data-ttu-id="eb9b7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb9b7-146">DateTimeOffset</span></span>|<span data-ttu-id="eb9b7-147">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="eb9b7-147">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="eb9b7-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb9b7-148">lastContactedDateTime</span></span>|<span data-ttu-id="eb9b7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb9b7-149">DateTimeOffset</span></span>|<span data-ttu-id="eb9b7-150">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="eb9b7-150">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="eb9b7-151">说明</span><span class="sxs-lookup"><span data-stu-id="eb9b7-151">description</span></span>|<span data-ttu-id="eb9b7-152">String</span><span class="sxs-lookup"><span data-stu-id="eb9b7-152">String</span></span>|<span data-ttu-id="eb9b7-153">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的说明</span><span class="sxs-lookup"><span data-stu-id="eb9b7-153">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="eb9b7-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="eb9b7-154">enrollmentState</span></span>|[<span data-ttu-id="eb9b7-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="eb9b7-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="eb9b7-156">Intune 中的设备的状态继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-156">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="eb9b7-157">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="eb9b7-158">platform</span><span class="sxs-lookup"><span data-stu-id="eb9b7-158">platform</span></span>|[<span data-ttu-id="eb9b7-159">平台</span><span class="sxs-lookup"><span data-stu-id="eb9b7-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="eb9b7-160">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-160">The platform of the Device.</span></span> <span data-ttu-id="eb9b7-161">继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-161">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="eb9b7-162">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="eb9b7-163">status</span><span class="sxs-lookup"><span data-stu-id="eb9b7-163">status</span></span>|<span data-ttu-id="eb9b7-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb9b7-164">Boolean</span></span>|<span data-ttu-id="eb9b7-165">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="eb9b7-165">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="eb9b7-166">响应</span><span class="sxs-lookup"><span data-stu-id="eb9b7-166">Response</span></span>
<span data-ttu-id="eb9b7-167">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-167">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb9b7-168">示例</span><span class="sxs-lookup"><span data-stu-id="eb9b7-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb9b7-169">请求</span><span class="sxs-lookup"><span data-stu-id="eb9b7-169">Request</span></span>
<span data-ttu-id="eb9b7-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="eb9b7-171">响应</span><span class="sxs-lookup"><span data-stu-id="eb9b7-171">Response</span></span>
<span data-ttu-id="eb9b7-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eb9b7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```




