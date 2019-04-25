---
title: 创建 importedDeviceIdentity
description: 创建新的 importedDeviceIdentity 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0be79099f755963eb039bc4f280200fe346e99ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532896"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="d5102-103">创建 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d5102-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="d5102-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d5102-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5102-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5102-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5102-106">创建新的[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d5102-106">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5102-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d5102-107">Prerequisites</span></span>
<span data-ttu-id="d5102-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5102-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5102-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5102-110">Permission type</span></span>|<span data-ttu-id="d5102-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d5102-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5102-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5102-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d5102-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5102-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d5102-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5102-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5102-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5102-115">Not supported.</span></span>|
|<span data-ttu-id="d5102-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5102-116">Application</span></span>|<span data-ttu-id="d5102-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5102-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5102-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5102-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="d5102-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5102-119">Request headers</span></span>
|<span data-ttu-id="d5102-120">标头</span><span class="sxs-lookup"><span data-stu-id="d5102-120">Header</span></span>|<span data-ttu-id="d5102-121">值</span><span class="sxs-lookup"><span data-stu-id="d5102-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5102-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5102-122">Authorization</span></span>|<span data-ttu-id="d5102-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d5102-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5102-124">接受</span><span class="sxs-lookup"><span data-stu-id="d5102-124">Accept</span></span>|<span data-ttu-id="d5102-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d5102-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5102-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5102-126">Request body</span></span>
<span data-ttu-id="d5102-127">在请求正文中, 提供 importedDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5102-127">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="d5102-128">下表显示创建 importedDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d5102-128">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="d5102-129">属性</span><span class="sxs-lookup"><span data-stu-id="d5102-129">Property</span></span>|<span data-ttu-id="d5102-130">类型</span><span class="sxs-lookup"><span data-stu-id="d5102-130">Type</span></span>|<span data-ttu-id="d5102-131">说明</span><span class="sxs-lookup"><span data-stu-id="d5102-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5102-132">id</span><span class="sxs-lookup"><span data-stu-id="d5102-132">id</span></span>|<span data-ttu-id="d5102-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d5102-133">String</span></span>|<span data-ttu-id="d5102-134">导入的设备标识的 Id</span><span class="sxs-lookup"><span data-stu-id="d5102-134">Id of the imported device identity</span></span>|
|<span data-ttu-id="d5102-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="d5102-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="d5102-136">String</span><span class="sxs-lookup"><span data-stu-id="d5102-136">String</span></span>|<span data-ttu-id="d5102-137">导入的设备标识符</span><span class="sxs-lookup"><span data-stu-id="d5102-137">Imported Device Identifier</span></span>|
|<span data-ttu-id="d5102-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="d5102-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="d5102-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="d5102-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="d5102-140">导入的设备标识的类型。</span><span class="sxs-lookup"><span data-stu-id="d5102-140">Type of Imported Device Identity.</span></span> <span data-ttu-id="d5102-141">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="d5102-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="d5102-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5102-142">lastModifiedDateTime</span></span>|<span data-ttu-id="d5102-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5102-143">DateTimeOffset</span></span>|<span data-ttu-id="d5102-144">说明的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="d5102-144">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="d5102-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5102-145">createdDateTime</span></span>|<span data-ttu-id="d5102-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5102-146">DateTimeOffset</span></span>|<span data-ttu-id="d5102-147">设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="d5102-147">Created Date Time of the device</span></span>|
|<span data-ttu-id="d5102-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5102-148">lastContactedDateTime</span></span>|<span data-ttu-id="d5102-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5102-149">DateTimeOffset</span></span>|<span data-ttu-id="d5102-150">设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="d5102-150">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="d5102-151">description</span><span class="sxs-lookup"><span data-stu-id="d5102-151">description</span></span>|<span data-ttu-id="d5102-152">String</span><span class="sxs-lookup"><span data-stu-id="d5102-152">String</span></span>|<span data-ttu-id="d5102-153">设备的说明</span><span class="sxs-lookup"><span data-stu-id="d5102-153">The description of the device</span></span>|
|<span data-ttu-id="d5102-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d5102-154">enrollmentState</span></span>|[<span data-ttu-id="d5102-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d5102-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="d5102-156">Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="d5102-156">The state of the device in Intune.</span></span> <span data-ttu-id="d5102-157">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="d5102-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="d5102-158">platform</span><span class="sxs-lookup"><span data-stu-id="d5102-158">platform</span></span>|[<span data-ttu-id="d5102-159">平台</span><span class="sxs-lookup"><span data-stu-id="d5102-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="d5102-160">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="d5102-160">The platform of the Device.</span></span> <span data-ttu-id="d5102-161">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="d5102-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="d5102-162">响应</span><span class="sxs-lookup"><span data-stu-id="d5102-162">Response</span></span>
<span data-ttu-id="d5102-163">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d5102-163">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5102-164">示例</span><span class="sxs-lookup"><span data-stu-id="d5102-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5102-165">请求</span><span class="sxs-lookup"><span data-stu-id="d5102-165">Request</span></span>
<span data-ttu-id="d5102-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5102-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d5102-167">响应</span><span class="sxs-lookup"><span data-stu-id="d5102-167">Response</span></span>
<span data-ttu-id="d5102-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5102-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





