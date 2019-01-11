---
title: 创建 importedDeviceIdentity
description: 创建新的 importedDeviceIdentity 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e3a6ca16d9bfa4a79d723816544e9a7bcf3f77df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870523"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="626cd-103">创建 importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="626cd-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="626cd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="626cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="626cd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="626cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="626cd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="626cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="626cd-107">创建新的[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="626cd-107">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="626cd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="626cd-108">Prerequisites</span></span>
<span data-ttu-id="626cd-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="626cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="626cd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="626cd-111">Permission type</span></span>|<span data-ttu-id="626cd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="626cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="626cd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="626cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="626cd-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="626cd-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="626cd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="626cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="626cd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="626cd-116">Not supported.</span></span>|
|<span data-ttu-id="626cd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="626cd-117">Application</span></span>|<span data-ttu-id="626cd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="626cd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="626cd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="626cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="626cd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="626cd-120">Request headers</span></span>
|<span data-ttu-id="626cd-121">标头</span><span class="sxs-lookup"><span data-stu-id="626cd-121">Header</span></span>|<span data-ttu-id="626cd-122">值</span><span class="sxs-lookup"><span data-stu-id="626cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="626cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="626cd-123">Authorization</span></span>|<span data-ttu-id="626cd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="626cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="626cd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="626cd-125">Accept</span></span>|<span data-ttu-id="626cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="626cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="626cd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="626cd-127">Request body</span></span>
<span data-ttu-id="626cd-128">在请求正文中，提供 importedDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="626cd-128">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="626cd-129">下表显示时创建 importedDeviceIdentity 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="626cd-129">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="626cd-130">属性</span><span class="sxs-lookup"><span data-stu-id="626cd-130">Property</span></span>|<span data-ttu-id="626cd-131">类型</span><span class="sxs-lookup"><span data-stu-id="626cd-131">Type</span></span>|<span data-ttu-id="626cd-132">说明</span><span class="sxs-lookup"><span data-stu-id="626cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="626cd-133">id</span><span class="sxs-lookup"><span data-stu-id="626cd-133">id</span></span>|<span data-ttu-id="626cd-134">字符串</span><span class="sxs-lookup"><span data-stu-id="626cd-134">String</span></span>|<span data-ttu-id="626cd-135">导入的设备标识的 id</span><span class="sxs-lookup"><span data-stu-id="626cd-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="626cd-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="626cd-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="626cd-137">字符串</span><span class="sxs-lookup"><span data-stu-id="626cd-137">String</span></span>|<span data-ttu-id="626cd-138">导入的设备标识符</span><span class="sxs-lookup"><span data-stu-id="626cd-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="626cd-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="626cd-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="626cd-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="626cd-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="626cd-141">导入的设备的标识的类型。</span><span class="sxs-lookup"><span data-stu-id="626cd-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="626cd-142">可取值为：`unknown`、`imei`、`serialNumber`。</span><span class="sxs-lookup"><span data-stu-id="626cd-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="626cd-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="626cd-143">lastModifiedDateTime</span></span>|<span data-ttu-id="626cd-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="626cd-144">DateTimeOffset</span></span>|<span data-ttu-id="626cd-145">上次修改日期时间的说明</span><span class="sxs-lookup"><span data-stu-id="626cd-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="626cd-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="626cd-146">createdDateTime</span></span>|<span data-ttu-id="626cd-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="626cd-147">DateTimeOffset</span></span>|<span data-ttu-id="626cd-148">设备的创建的日期时间</span><span class="sxs-lookup"><span data-stu-id="626cd-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="626cd-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="626cd-149">lastContactedDateTime</span></span>|<span data-ttu-id="626cd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="626cd-150">DateTimeOffset</span></span>|<span data-ttu-id="626cd-151">设备的最后一个联系日期时间</span><span class="sxs-lookup"><span data-stu-id="626cd-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="626cd-152">说明</span><span class="sxs-lookup"><span data-stu-id="626cd-152">description</span></span>|<span data-ttu-id="626cd-153">字符串</span><span class="sxs-lookup"><span data-stu-id="626cd-153">String</span></span>|<span data-ttu-id="626cd-154">设备的说明</span><span class="sxs-lookup"><span data-stu-id="626cd-154">The description of the device</span></span>|
|<span data-ttu-id="626cd-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="626cd-155">enrollmentState</span></span>|[<span data-ttu-id="626cd-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="626cd-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="626cd-157">在 Intune 设备的状态。</span><span class="sxs-lookup"><span data-stu-id="626cd-157">The state of the device in Intune.</span></span> <span data-ttu-id="626cd-158">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="626cd-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="626cd-159">platform</span><span class="sxs-lookup"><span data-stu-id="626cd-159">platform</span></span>|[<span data-ttu-id="626cd-160">平台</span><span class="sxs-lookup"><span data-stu-id="626cd-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="626cd-161">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="626cd-161">The platform of the Device.</span></span> <span data-ttu-id="626cd-162">可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="626cd-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="626cd-163">响应</span><span class="sxs-lookup"><span data-stu-id="626cd-163">Response</span></span>
<span data-ttu-id="626cd-164">如果成功，此方法返回`201 Created`响应代码和响应正文中的[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="626cd-164">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="626cd-165">示例</span><span class="sxs-lookup"><span data-stu-id="626cd-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="626cd-166">请求</span><span class="sxs-lookup"><span data-stu-id="626cd-166">Request</span></span>
<span data-ttu-id="626cd-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="626cd-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
Content-type: application/json
Content-length: 396

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="626cd-168">响应</span><span class="sxs-lookup"><span data-stu-id="626cd-168">Response</span></span>
<span data-ttu-id="626cd-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="626cd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





