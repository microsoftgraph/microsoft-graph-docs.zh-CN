---
title: 更新 importedDeviceIdentity
description: 更新 importedDeviceIdentity 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: abc82d0f5305c2cefcc76283e8836d8dacf6e626
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420386"
---
# <a name="update-importeddeviceidentity"></a><span data-ttu-id="8efb7-103">更新 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="8efb7-103">Update importedDeviceIdentity</span></span>

> <span data-ttu-id="8efb7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="8efb7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8efb7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8efb7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8efb7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8efb7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8efb7-107">更新[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8efb7-107">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8efb7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8efb7-108">Prerequisites</span></span>
<span data-ttu-id="8efb7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8efb7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8efb7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8efb7-111">Permission type</span></span>|<span data-ttu-id="8efb7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8efb7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8efb7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8efb7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8efb7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8efb7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8efb7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8efb7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8efb7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8efb7-116">Not supported.</span></span>|
|<span data-ttu-id="8efb7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8efb7-117">Application</span></span>|<span data-ttu-id="8efb7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8efb7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8efb7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8efb7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="8efb7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8efb7-120">Request headers</span></span>
|<span data-ttu-id="8efb7-121">标头</span><span class="sxs-lookup"><span data-stu-id="8efb7-121">Header</span></span>|<span data-ttu-id="8efb7-122">值</span><span class="sxs-lookup"><span data-stu-id="8efb7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8efb7-123">授权</span><span class="sxs-lookup"><span data-stu-id="8efb7-123">Authorization</span></span>|<span data-ttu-id="8efb7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8efb7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8efb7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8efb7-125">Accept</span></span>|<span data-ttu-id="8efb7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8efb7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8efb7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8efb7-127">Request body</span></span>
<span data-ttu-id="8efb7-128">在请求正文中，提供[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8efb7-128">In the request body, supply a JSON representation for the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>

<span data-ttu-id="8efb7-129">下表显示时创建[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8efb7-129">The following table shows the properties that are required when you create the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>

|<span data-ttu-id="8efb7-130">属性</span><span class="sxs-lookup"><span data-stu-id="8efb7-130">Property</span></span>|<span data-ttu-id="8efb7-131">类型</span><span class="sxs-lookup"><span data-stu-id="8efb7-131">Type</span></span>|<span data-ttu-id="8efb7-132">说明</span><span class="sxs-lookup"><span data-stu-id="8efb7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8efb7-133">id</span><span class="sxs-lookup"><span data-stu-id="8efb7-133">id</span></span>|<span data-ttu-id="8efb7-134">String</span><span class="sxs-lookup"><span data-stu-id="8efb7-134">String</span></span>|<span data-ttu-id="8efb7-135">导入的设备标识的 id</span><span class="sxs-lookup"><span data-stu-id="8efb7-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="8efb7-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="8efb7-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="8efb7-137">String</span><span class="sxs-lookup"><span data-stu-id="8efb7-137">String</span></span>|<span data-ttu-id="8efb7-138">导入的设备标识符</span><span class="sxs-lookup"><span data-stu-id="8efb7-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="8efb7-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="8efb7-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="8efb7-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="8efb7-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="8efb7-141">导入的设备的标识的类型。</span><span class="sxs-lookup"><span data-stu-id="8efb7-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="8efb7-142">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="8efb7-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="8efb7-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8efb7-143">lastModifiedDateTime</span></span>|<span data-ttu-id="8efb7-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8efb7-144">DateTimeOffset</span></span>|<span data-ttu-id="8efb7-145">上次修改日期时间的说明</span><span class="sxs-lookup"><span data-stu-id="8efb7-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="8efb7-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8efb7-146">createdDateTime</span></span>|<span data-ttu-id="8efb7-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8efb7-147">DateTimeOffset</span></span>|<span data-ttu-id="8efb7-148">设备的创建的日期时间</span><span class="sxs-lookup"><span data-stu-id="8efb7-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="8efb7-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="8efb7-149">lastContactedDateTime</span></span>|<span data-ttu-id="8efb7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8efb7-150">DateTimeOffset</span></span>|<span data-ttu-id="8efb7-151">设备的最后一个联系日期时间</span><span class="sxs-lookup"><span data-stu-id="8efb7-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="8efb7-152">说明</span><span class="sxs-lookup"><span data-stu-id="8efb7-152">description</span></span>|<span data-ttu-id="8efb7-153">String</span><span class="sxs-lookup"><span data-stu-id="8efb7-153">String</span></span>|<span data-ttu-id="8efb7-154">设备的说明</span><span class="sxs-lookup"><span data-stu-id="8efb7-154">The description of the device</span></span>|
|<span data-ttu-id="8efb7-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="8efb7-155">enrollmentState</span></span>|[<span data-ttu-id="8efb7-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="8efb7-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="8efb7-157">在 Intune 设备的状态。</span><span class="sxs-lookup"><span data-stu-id="8efb7-157">The state of the device in Intune.</span></span> <span data-ttu-id="8efb7-158">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="8efb7-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="8efb7-159">platform</span><span class="sxs-lookup"><span data-stu-id="8efb7-159">platform</span></span>|[<span data-ttu-id="8efb7-160">平台</span><span class="sxs-lookup"><span data-stu-id="8efb7-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="8efb7-161">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="8efb7-161">The platform of the Device.</span></span> <span data-ttu-id="8efb7-162">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="8efb7-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="8efb7-163">响应</span><span class="sxs-lookup"><span data-stu-id="8efb7-163">Response</span></span>
<span data-ttu-id="8efb7-164">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8efb7-164">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8efb7-165">示例</span><span class="sxs-lookup"><span data-stu-id="8efb7-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="8efb7-166">请求</span><span class="sxs-lookup"><span data-stu-id="8efb7-166">Request</span></span>
<span data-ttu-id="8efb7-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8efb7-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8efb7-168">响应</span><span class="sxs-lookup"><span data-stu-id="8efb7-168">Response</span></span>
<span data-ttu-id="8efb7-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8efb7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




