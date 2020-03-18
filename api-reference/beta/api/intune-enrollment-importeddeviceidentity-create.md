---
title: 创建 importedDeviceIdentity
description: 创建新的 importedDeviceIdentity 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7cc1b85ba8c8bf81bd2fc45fd95f889327f31da6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42805233"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="1cbf8-103">创建 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="1cbf8-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="1cbf8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cbf8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cbf8-106">创建新的[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-106">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1cbf8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1cbf8-107">Prerequisites</span></span>
<span data-ttu-id="1cbf8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cbf8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1cbf8-110">Permission type</span></span>|<span data-ttu-id="1cbf8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1cbf8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cbf8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1cbf8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1cbf8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cbf8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1cbf8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1cbf8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cbf8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-115">Not supported.</span></span>|
|<span data-ttu-id="1cbf8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1cbf8-116">Application</span></span>|<span data-ttu-id="1cbf8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cbf8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cbf8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1cbf8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="1cbf8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1cbf8-119">Request headers</span></span>
|<span data-ttu-id="1cbf8-120">标头</span><span class="sxs-lookup"><span data-stu-id="1cbf8-120">Header</span></span>|<span data-ttu-id="1cbf8-121">值</span><span class="sxs-lookup"><span data-stu-id="1cbf8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cbf8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cbf8-122">Authorization</span></span>|<span data-ttu-id="1cbf8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cbf8-124">接受</span><span class="sxs-lookup"><span data-stu-id="1cbf8-124">Accept</span></span>|<span data-ttu-id="1cbf8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1cbf8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cbf8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1cbf8-126">Request body</span></span>
<span data-ttu-id="1cbf8-127">在请求正文中，提供 importedDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-127">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="1cbf8-128">下表显示创建 importedDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-128">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="1cbf8-129">属性</span><span class="sxs-lookup"><span data-stu-id="1cbf8-129">Property</span></span>|<span data-ttu-id="1cbf8-130">类型</span><span class="sxs-lookup"><span data-stu-id="1cbf8-130">Type</span></span>|<span data-ttu-id="1cbf8-131">说明</span><span class="sxs-lookup"><span data-stu-id="1cbf8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cbf8-132">id</span><span class="sxs-lookup"><span data-stu-id="1cbf8-132">id</span></span>|<span data-ttu-id="1cbf8-133">字符串</span><span class="sxs-lookup"><span data-stu-id="1cbf8-133">String</span></span>|<span data-ttu-id="1cbf8-134">导入的设备标识的 Id</span><span class="sxs-lookup"><span data-stu-id="1cbf8-134">Id of the imported device identity</span></span>|
|<span data-ttu-id="1cbf8-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1cbf8-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="1cbf8-136">String</span><span class="sxs-lookup"><span data-stu-id="1cbf8-136">String</span></span>|<span data-ttu-id="1cbf8-137">导入的设备标识符</span><span class="sxs-lookup"><span data-stu-id="1cbf8-137">Imported Device Identifier</span></span>|
|<span data-ttu-id="1cbf8-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="1cbf8-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="1cbf8-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="1cbf8-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="1cbf8-140">导入的设备标识的类型。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-140">Type of Imported Device Identity.</span></span> <span data-ttu-id="1cbf8-141">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="1cbf8-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cbf8-142">lastModifiedDateTime</span></span>|<span data-ttu-id="1cbf8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cbf8-143">DateTimeOffset</span></span>|<span data-ttu-id="1cbf8-144">说明的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="1cbf8-144">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="1cbf8-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1cbf8-145">createdDateTime</span></span>|<span data-ttu-id="1cbf8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cbf8-146">DateTimeOffset</span></span>|<span data-ttu-id="1cbf8-147">设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="1cbf8-147">Created Date Time of the device</span></span>|
|<span data-ttu-id="1cbf8-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cbf8-148">lastContactedDateTime</span></span>|<span data-ttu-id="1cbf8-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cbf8-149">DateTimeOffset</span></span>|<span data-ttu-id="1cbf8-150">设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="1cbf8-150">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="1cbf8-151">说明</span><span class="sxs-lookup"><span data-stu-id="1cbf8-151">description</span></span>|<span data-ttu-id="1cbf8-152">String</span><span class="sxs-lookup"><span data-stu-id="1cbf8-152">String</span></span>|<span data-ttu-id="1cbf8-153">设备的说明</span><span class="sxs-lookup"><span data-stu-id="1cbf8-153">The description of the device</span></span>|
|<span data-ttu-id="1cbf8-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="1cbf8-154">enrollmentState</span></span>|[<span data-ttu-id="1cbf8-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="1cbf8-155">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="1cbf8-156">Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-156">The state of the device in Intune.</span></span> <span data-ttu-id="1cbf8-157">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="1cbf8-158">platform</span><span class="sxs-lookup"><span data-stu-id="1cbf8-158">platform</span></span>|[<span data-ttu-id="1cbf8-159">平台</span><span class="sxs-lookup"><span data-stu-id="1cbf8-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="1cbf8-160">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-160">The platform of the Device.</span></span> <span data-ttu-id="1cbf8-161">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="1cbf8-162">响应</span><span class="sxs-lookup"><span data-stu-id="1cbf8-162">Response</span></span>
<span data-ttu-id="1cbf8-163">如果成功，此方法在响应`201 Created`正文中返回响应代码和[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-163">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cbf8-164">示例</span><span class="sxs-lookup"><span data-stu-id="1cbf8-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cbf8-165">请求</span><span class="sxs-lookup"><span data-stu-id="1cbf8-165">Request</span></span>
<span data-ttu-id="1cbf8-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="1cbf8-167">响应</span><span class="sxs-lookup"><span data-stu-id="1cbf8-167">Response</span></span>
<span data-ttu-id="1cbf8-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1cbf8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




