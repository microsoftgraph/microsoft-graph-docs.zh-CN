---
title: 更新 importedDeviceIdentityResult
description: 更新 importedDeviceIdentityResult 对象的属性。
ms.openlocfilehash: f6b875d19e789010a1a130dcb31ef115acb07cfc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044436"
---
# <a name="update-importeddeviceidentityresult"></a><span data-ttu-id="9ec4b-103">更新 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="9ec4b-103">Update importedDeviceIdentityResult</span></span>

> <span data-ttu-id="9ec4b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ec4b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ec4b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ec4b-107">更新[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-107">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9ec4b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9ec4b-108">Prerequisites</span></span>
<span data-ttu-id="9ec4b-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9ec4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ec4b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ec4b-111">Permission type</span></span>|<span data-ttu-id="9ec4b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9ec4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ec4b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ec4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ec4b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ec4b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9ec4b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ec4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ec4b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-116">Not supported.</span></span>|
|<span data-ttu-id="9ec4b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ec4b-117">Application</span></span>|<span data-ttu-id="9ec4b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ec4b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ec4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="9ec4b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ec4b-120">Request headers</span></span>
|<span data-ttu-id="9ec4b-121">标头</span><span class="sxs-lookup"><span data-stu-id="9ec4b-121">Header</span></span>|<span data-ttu-id="9ec4b-122">值</span><span class="sxs-lookup"><span data-stu-id="9ec4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ec4b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ec4b-123">Authorization</span></span>|<span data-ttu-id="9ec4b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ec4b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9ec4b-125">Accept</span></span>|<span data-ttu-id="9ec4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ec4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ec4b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ec4b-127">Request body</span></span>
<span data-ttu-id="9ec4b-128">在请求正文中，提供[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-128">In the request body, supply a JSON representation for the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

<span data-ttu-id="9ec4b-129">下表显示时创建[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-129">The following table shows the properties that are required when you create the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>

|<span data-ttu-id="9ec4b-130">属性</span><span class="sxs-lookup"><span data-stu-id="9ec4b-130">Property</span></span>|<span data-ttu-id="9ec4b-131">类型</span><span class="sxs-lookup"><span data-stu-id="9ec4b-131">Type</span></span>|<span data-ttu-id="9ec4b-132">说明</span><span class="sxs-lookup"><span data-stu-id="9ec4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ec4b-133">id</span><span class="sxs-lookup"><span data-stu-id="9ec4b-133">id</span></span>|<span data-ttu-id="9ec4b-134">字符串</span><span class="sxs-lookup"><span data-stu-id="9ec4b-134">String</span></span>|<span data-ttu-id="9ec4b-135">来自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)导入的设备的标识继承的 id</span><span class="sxs-lookup"><span data-stu-id="9ec4b-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="9ec4b-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="9ec4b-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="9ec4b-137">字符串</span><span class="sxs-lookup"><span data-stu-id="9ec4b-137">String</span></span>|<span data-ttu-id="9ec4b-138">导入设备标识符继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="9ec4b-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="9ec4b-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="9ec4b-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="9ec4b-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="9ec4b-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="9ec4b-141">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)导入设备标识继承的类型。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="9ec4b-142">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="9ec4b-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ec4b-143">lastModifiedDateTime</span></span>|<span data-ttu-id="9ec4b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ec4b-144">DateTimeOffset</span></span>|<span data-ttu-id="9ec4b-145">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)的说明继承的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="9ec4b-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="9ec4b-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ec4b-146">createdDateTime</span></span>|<span data-ttu-id="9ec4b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ec4b-147">DateTimeOffset</span></span>|<span data-ttu-id="9ec4b-148">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)创建设备继承的日期时间</span><span class="sxs-lookup"><span data-stu-id="9ec4b-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="9ec4b-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ec4b-149">lastContactedDateTime</span></span>|<span data-ttu-id="9ec4b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ec4b-150">DateTimeOffset</span></span>|<span data-ttu-id="9ec4b-151">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)设备继承的最后一个联系日期时间</span><span class="sxs-lookup"><span data-stu-id="9ec4b-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="9ec4b-152">说明</span><span class="sxs-lookup"><span data-stu-id="9ec4b-152">description</span></span>|<span data-ttu-id="9ec4b-153">字符串</span><span class="sxs-lookup"><span data-stu-id="9ec4b-153">String</span></span>|<span data-ttu-id="9ec4b-154">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)设备继承说明</span><span class="sxs-lookup"><span data-stu-id="9ec4b-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="9ec4b-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="9ec4b-155">enrollmentState</span></span>|[<span data-ttu-id="9ec4b-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="9ec4b-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="9ec4b-157">从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)中 Intune 继承的设备的状态。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="9ec4b-158">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="9ec4b-159">platform</span><span class="sxs-lookup"><span data-stu-id="9ec4b-159">platform</span></span>|[<span data-ttu-id="9ec4b-160">平台</span><span class="sxs-lookup"><span data-stu-id="9ec4b-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="9ec4b-161">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-161">The platform of the Device.</span></span> <span data-ttu-id="9ec4b-162">继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="9ec4b-163">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="9ec4b-164">状态</span><span class="sxs-lookup"><span data-stu-id="9ec4b-164">status</span></span>|<span data-ttu-id="9ec4b-165">布尔</span><span class="sxs-lookup"><span data-stu-id="9ec4b-165">Boolean</span></span>|<span data-ttu-id="9ec4b-166">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="9ec4b-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="9ec4b-167">响应</span><span class="sxs-lookup"><span data-stu-id="9ec4b-167">Response</span></span>
<span data-ttu-id="9ec4b-168">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-168">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ec4b-169">示例</span><span class="sxs-lookup"><span data-stu-id="9ec4b-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="9ec4b-170">请求</span><span class="sxs-lookup"><span data-stu-id="9ec4b-170">Request</span></span>
<span data-ttu-id="9ec4b-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 354

{
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="9ec4b-172">响应</span><span class="sxs-lookup"><span data-stu-id="9ec4b-172">Response</span></span>
<span data-ttu-id="9ec4b-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9ec4b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





