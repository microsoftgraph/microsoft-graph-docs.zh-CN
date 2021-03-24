---
title: 更新 importedDeviceIdentityResult
description: 更新 importedDeviceIdentityResult 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 36f71f2d4d1494e459e2cf9f9867d354a931a2f1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142217"
---
# <a name="update-importeddeviceidentityresult"></a><span data-ttu-id="8ef13-103">更新 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="8ef13-103">Update importedDeviceIdentityResult</span></span>

<span data-ttu-id="8ef13-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ef13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ef13-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8ef13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ef13-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ef13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ef13-107">更新 [importedDeviceIdentityResult 对象](../resources/intune-enrollment-importeddeviceidentityresult.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="8ef13-107">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ef13-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8ef13-108">Prerequisites</span></span>
<span data-ttu-id="8ef13-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ef13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ef13-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ef13-111">Permission type</span></span>|<span data-ttu-id="8ef13-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ef13-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ef13-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ef13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ef13-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ef13-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8ef13-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ef13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ef13-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ef13-116">Not supported.</span></span>|
|<span data-ttu-id="8ef13-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ef13-117">Application</span></span>|<span data-ttu-id="8ef13-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ef13-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ef13-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ef13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="8ef13-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ef13-120">Request headers</span></span>
|<span data-ttu-id="8ef13-121">标头</span><span class="sxs-lookup"><span data-stu-id="8ef13-121">Header</span></span>|<span data-ttu-id="8ef13-122">值</span><span class="sxs-lookup"><span data-stu-id="8ef13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ef13-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ef13-123">Authorization</span></span>|<span data-ttu-id="8ef13-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8ef13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ef13-125">接受</span><span class="sxs-lookup"><span data-stu-id="8ef13-125">Accept</span></span>|<span data-ttu-id="8ef13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ef13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ef13-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ef13-127">Request body</span></span>
<span data-ttu-id="8ef13-128">在请求正文中，提供 [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ef13-128">In the request body, supply a JSON representation for the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

<span data-ttu-id="8ef13-129">下表显示创建 [importedDeviceIdentityResult 时所需的属性](../resources/intune-enrollment-importeddeviceidentityresult.md)。</span><span class="sxs-lookup"><span data-stu-id="8ef13-129">The following table shows the properties that are required when you create the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>

|<span data-ttu-id="8ef13-130">属性</span><span class="sxs-lookup"><span data-stu-id="8ef13-130">Property</span></span>|<span data-ttu-id="8ef13-131">类型</span><span class="sxs-lookup"><span data-stu-id="8ef13-131">Type</span></span>|<span data-ttu-id="8ef13-132">说明</span><span class="sxs-lookup"><span data-stu-id="8ef13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ef13-133">id</span><span class="sxs-lookup"><span data-stu-id="8ef13-133">id</span></span>|<span data-ttu-id="8ef13-134">String</span><span class="sxs-lookup"><span data-stu-id="8ef13-134">String</span></span>|<span data-ttu-id="8ef13-135">导入的设备标识的 ID 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="8ef13-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="8ef13-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="8ef13-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="8ef13-137">String</span><span class="sxs-lookup"><span data-stu-id="8ef13-137">String</span></span>|<span data-ttu-id="8ef13-138">导入的设备标识符 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="8ef13-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="8ef13-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="8ef13-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="8ef13-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="8ef13-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="8ef13-141">导入的设备标识的类型 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="8ef13-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="8ef13-142">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="8ef13-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="8ef13-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ef13-143">lastModifiedDateTime</span></span>|<span data-ttu-id="8ef13-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ef13-144">DateTimeOffset</span></span>|<span data-ttu-id="8ef13-145">说明的 Last Modified DateTime 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="8ef13-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="8ef13-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ef13-146">createdDateTime</span></span>|<span data-ttu-id="8ef13-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ef13-147">DateTimeOffset</span></span>|<span data-ttu-id="8ef13-148">设备的创建日期时间 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="8ef13-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="8ef13-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ef13-149">lastContactedDateTime</span></span>|<span data-ttu-id="8ef13-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ef13-150">DateTimeOffset</span></span>|<span data-ttu-id="8ef13-151">设备的上次联系日期时间 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="8ef13-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="8ef13-152">说明</span><span class="sxs-lookup"><span data-stu-id="8ef13-152">description</span></span>|<span data-ttu-id="8ef13-153">String</span><span class="sxs-lookup"><span data-stu-id="8ef13-153">String</span></span>|<span data-ttu-id="8ef13-154">设备描述 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="8ef13-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="8ef13-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="8ef13-155">enrollmentState</span></span>|[<span data-ttu-id="8ef13-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="8ef13-156">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="8ef13-157">Intune 中的设备状态 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="8ef13-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="8ef13-158">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="8ef13-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="8ef13-159">平台</span><span class="sxs-lookup"><span data-stu-id="8ef13-159">platform</span></span>|[<span data-ttu-id="8ef13-160">平台</span><span class="sxs-lookup"><span data-stu-id="8ef13-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="8ef13-161">设备平台。</span><span class="sxs-lookup"><span data-stu-id="8ef13-161">The platform of the Device.</span></span> <span data-ttu-id="8ef13-162">继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="8ef13-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="8ef13-163">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="8ef13-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="8ef13-164">状态</span><span class="sxs-lookup"><span data-stu-id="8ef13-164">status</span></span>|<span data-ttu-id="8ef13-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ef13-165">Boolean</span></span>|<span data-ttu-id="8ef13-166">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="8ef13-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="8ef13-167">响应</span><span class="sxs-lookup"><span data-stu-id="8ef13-167">Response</span></span>
<span data-ttu-id="8ef13-168">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ef13-168">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ef13-169">示例</span><span class="sxs-lookup"><span data-stu-id="8ef13-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ef13-170">请求</span><span class="sxs-lookup"><span data-stu-id="8ef13-170">Request</span></span>
<span data-ttu-id="8ef13-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ef13-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8ef13-172">响应</span><span class="sxs-lookup"><span data-stu-id="8ef13-172">Response</span></span>
<span data-ttu-id="8ef13-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ef13-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




