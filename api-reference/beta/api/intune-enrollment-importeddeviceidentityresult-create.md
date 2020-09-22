---
title: 创建 importedDeviceIdentityResult
description: 创建新的 importedDeviceIdentityResult 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10c39468a4966c5eb18dd61ec5b66512be43c2e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48068614"
---
# <a name="create-importeddeviceidentityresult"></a><span data-ttu-id="718b9-103">创建 importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="718b9-103">Create importedDeviceIdentityResult</span></span>

<span data-ttu-id="718b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="718b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="718b9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="718b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="718b9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="718b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="718b9-107">创建新的 [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="718b9-107">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="718b9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="718b9-108">Prerequisites</span></span>
<span data-ttu-id="718b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="718b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="718b9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="718b9-111">Permission type</span></span>|<span data-ttu-id="718b9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="718b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="718b9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="718b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="718b9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="718b9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="718b9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="718b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="718b9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="718b9-116">Not supported.</span></span>|
|<span data-ttu-id="718b9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="718b9-117">Application</span></span>|<span data-ttu-id="718b9-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="718b9-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="718b9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="718b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="718b9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="718b9-120">Request headers</span></span>
|<span data-ttu-id="718b9-121">标头</span><span class="sxs-lookup"><span data-stu-id="718b9-121">Header</span></span>|<span data-ttu-id="718b9-122">值</span><span class="sxs-lookup"><span data-stu-id="718b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="718b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="718b9-123">Authorization</span></span>|<span data-ttu-id="718b9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="718b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="718b9-125">接受</span><span class="sxs-lookup"><span data-stu-id="718b9-125">Accept</span></span>|<span data-ttu-id="718b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="718b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="718b9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="718b9-127">Request body</span></span>
<span data-ttu-id="718b9-128">在请求正文中，提供 importedDeviceIdentityResult 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="718b9-128">In the request body, supply a JSON representation for the importedDeviceIdentityResult object.</span></span>

<span data-ttu-id="718b9-129">下表显示创建 importedDeviceIdentityResult 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="718b9-129">The following table shows the properties that are required when you create the importedDeviceIdentityResult.</span></span>

|<span data-ttu-id="718b9-130">属性</span><span class="sxs-lookup"><span data-stu-id="718b9-130">Property</span></span>|<span data-ttu-id="718b9-131">类型</span><span class="sxs-lookup"><span data-stu-id="718b9-131">Type</span></span>|<span data-ttu-id="718b9-132">说明</span><span class="sxs-lookup"><span data-stu-id="718b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="718b9-133">id</span><span class="sxs-lookup"><span data-stu-id="718b9-133">id</span></span>|<span data-ttu-id="718b9-134">String</span><span class="sxs-lookup"><span data-stu-id="718b9-134">String</span></span>|<span data-ttu-id="718b9-135">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识的 Id</span><span class="sxs-lookup"><span data-stu-id="718b9-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="718b9-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="718b9-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="718b9-137">String</span><span class="sxs-lookup"><span data-stu-id="718b9-137">String</span></span>|<span data-ttu-id="718b9-138">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识符</span><span class="sxs-lookup"><span data-stu-id="718b9-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="718b9-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="718b9-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="718b9-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="718b9-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="718b9-141">从 [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识的类型。</span><span class="sxs-lookup"><span data-stu-id="718b9-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="718b9-142">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="718b9-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="718b9-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="718b9-143">lastModifiedDateTime</span></span>|<span data-ttu-id="718b9-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="718b9-144">DateTimeOffset</span></span>|<span data-ttu-id="718b9-145">继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)的说明的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="718b9-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="718b9-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="718b9-146">createdDateTime</span></span>|<span data-ttu-id="718b9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="718b9-147">DateTimeOffset</span></span>|<span data-ttu-id="718b9-148">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="718b9-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="718b9-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="718b9-149">lastContactedDateTime</span></span>|<span data-ttu-id="718b9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="718b9-150">DateTimeOffset</span></span>|<span data-ttu-id="718b9-151">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的上次联系日期时间</span><span class="sxs-lookup"><span data-stu-id="718b9-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="718b9-152">说明</span><span class="sxs-lookup"><span data-stu-id="718b9-152">description</span></span>|<span data-ttu-id="718b9-153">String</span><span class="sxs-lookup"><span data-stu-id="718b9-153">String</span></span>|<span data-ttu-id="718b9-154">从[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的说明</span><span class="sxs-lookup"><span data-stu-id="718b9-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="718b9-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="718b9-155">enrollmentState</span></span>|[<span data-ttu-id="718b9-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="718b9-156">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="718b9-157">Intune 中的设备的状态继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="718b9-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="718b9-158">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="718b9-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="718b9-159">平台</span><span class="sxs-lookup"><span data-stu-id="718b9-159">platform</span></span>|[<span data-ttu-id="718b9-160">平台</span><span class="sxs-lookup"><span data-stu-id="718b9-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="718b9-161">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="718b9-161">The platform of the Device.</span></span> <span data-ttu-id="718b9-162">继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。</span><span class="sxs-lookup"><span data-stu-id="718b9-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="718b9-163">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="718b9-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="718b9-164">状态</span><span class="sxs-lookup"><span data-stu-id="718b9-164">status</span></span>|<span data-ttu-id="718b9-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="718b9-165">Boolean</span></span>|<span data-ttu-id="718b9-166">导入的设备标识的状态</span><span class="sxs-lookup"><span data-stu-id="718b9-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="718b9-167">响应</span><span class="sxs-lookup"><span data-stu-id="718b9-167">Response</span></span>
<span data-ttu-id="718b9-168">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="718b9-168">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="718b9-169">示例</span><span class="sxs-lookup"><span data-stu-id="718b9-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="718b9-170">请求</span><span class="sxs-lookup"><span data-stu-id="718b9-170">Request</span></span>
<span data-ttu-id="718b9-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="718b9-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="718b9-172">响应</span><span class="sxs-lookup"><span data-stu-id="718b9-172">Response</span></span>
<span data-ttu-id="718b9-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="718b9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






