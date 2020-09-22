---
title: 更新 importedDeviceIdentity
description: 更新 importedDeviceIdentity 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 880eb50a27344c6d35fde99a3c40127525a771ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48068635"
---
# <a name="update-importeddeviceidentity"></a><span data-ttu-id="d79ba-103">更新 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d79ba-103">Update importedDeviceIdentity</span></span>

<span data-ttu-id="d79ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d79ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d79ba-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d79ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d79ba-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d79ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d79ba-107">更新 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d79ba-107">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d79ba-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d79ba-108">Prerequisites</span></span>
<span data-ttu-id="d79ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d79ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d79ba-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d79ba-111">Permission type</span></span>|<span data-ttu-id="d79ba-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d79ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d79ba-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d79ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d79ba-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d79ba-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d79ba-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d79ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d79ba-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d79ba-116">Not supported.</span></span>|
|<span data-ttu-id="d79ba-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d79ba-117">Application</span></span>|<span data-ttu-id="d79ba-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d79ba-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d79ba-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d79ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="d79ba-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d79ba-120">Request headers</span></span>
|<span data-ttu-id="d79ba-121">标头</span><span class="sxs-lookup"><span data-stu-id="d79ba-121">Header</span></span>|<span data-ttu-id="d79ba-122">值</span><span class="sxs-lookup"><span data-stu-id="d79ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d79ba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d79ba-123">Authorization</span></span>|<span data-ttu-id="d79ba-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d79ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d79ba-125">接受</span><span class="sxs-lookup"><span data-stu-id="d79ba-125">Accept</span></span>|<span data-ttu-id="d79ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d79ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d79ba-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d79ba-127">Request body</span></span>
<span data-ttu-id="d79ba-128">在请求正文中，提供 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d79ba-128">In the request body, supply a JSON representation for the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

<span data-ttu-id="d79ba-129">下表显示创建 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d79ba-129">The following table shows the properties that are required when you create the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>

|<span data-ttu-id="d79ba-130">属性</span><span class="sxs-lookup"><span data-stu-id="d79ba-130">Property</span></span>|<span data-ttu-id="d79ba-131">类型</span><span class="sxs-lookup"><span data-stu-id="d79ba-131">Type</span></span>|<span data-ttu-id="d79ba-132">说明</span><span class="sxs-lookup"><span data-stu-id="d79ba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d79ba-133">id</span><span class="sxs-lookup"><span data-stu-id="d79ba-133">id</span></span>|<span data-ttu-id="d79ba-134">String</span><span class="sxs-lookup"><span data-stu-id="d79ba-134">String</span></span>|<span data-ttu-id="d79ba-135">导入的设备标识的 Id</span><span class="sxs-lookup"><span data-stu-id="d79ba-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="d79ba-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="d79ba-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="d79ba-137">String</span><span class="sxs-lookup"><span data-stu-id="d79ba-137">String</span></span>|<span data-ttu-id="d79ba-138">导入的设备标识符</span><span class="sxs-lookup"><span data-stu-id="d79ba-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="d79ba-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="d79ba-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="d79ba-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="d79ba-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="d79ba-141">导入的设备标识的类型。</span><span class="sxs-lookup"><span data-stu-id="d79ba-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="d79ba-142">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="d79ba-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="d79ba-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d79ba-143">lastModifiedDateTime</span></span>|<span data-ttu-id="d79ba-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d79ba-144">DateTimeOffset</span></span>|<span data-ttu-id="d79ba-145">说明的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="d79ba-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="d79ba-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d79ba-146">createdDateTime</span></span>|<span data-ttu-id="d79ba-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d79ba-147">DateTimeOffset</span></span>|<span data-ttu-id="d79ba-148">设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="d79ba-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="d79ba-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="d79ba-149">lastContactedDateTime</span></span>|<span data-ttu-id="d79ba-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d79ba-150">DateTimeOffset</span></span>|<span data-ttu-id="d79ba-151">设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="d79ba-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="d79ba-152">说明</span><span class="sxs-lookup"><span data-stu-id="d79ba-152">description</span></span>|<span data-ttu-id="d79ba-153">String</span><span class="sxs-lookup"><span data-stu-id="d79ba-153">String</span></span>|<span data-ttu-id="d79ba-154">设备的说明</span><span class="sxs-lookup"><span data-stu-id="d79ba-154">The description of the device</span></span>|
|<span data-ttu-id="d79ba-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d79ba-155">enrollmentState</span></span>|[<span data-ttu-id="d79ba-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d79ba-156">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="d79ba-157">Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="d79ba-157">The state of the device in Intune.</span></span> <span data-ttu-id="d79ba-158">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="d79ba-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="d79ba-159">平台</span><span class="sxs-lookup"><span data-stu-id="d79ba-159">platform</span></span>|[<span data-ttu-id="d79ba-160">平台</span><span class="sxs-lookup"><span data-stu-id="d79ba-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="d79ba-161">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="d79ba-161">The platform of the Device.</span></span> <span data-ttu-id="d79ba-162">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="d79ba-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="d79ba-163">响应</span><span class="sxs-lookup"><span data-stu-id="d79ba-163">Response</span></span>
<span data-ttu-id="d79ba-164">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d79ba-164">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d79ba-165">示例</span><span class="sxs-lookup"><span data-stu-id="d79ba-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="d79ba-166">请求</span><span class="sxs-lookup"><span data-stu-id="d79ba-166">Request</span></span>
<span data-ttu-id="d79ba-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d79ba-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 332

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="d79ba-168">响应</span><span class="sxs-lookup"><span data-stu-id="d79ba-168">Response</span></span>
<span data-ttu-id="d79ba-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d79ba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```






