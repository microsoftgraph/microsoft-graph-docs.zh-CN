---
title: 更新 appleUserInitiatedEnrollmentProfile
description: 更新 appleUserInitiatedEnrollmentProfile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e26399495ccc1062113e943495d8007f80a0d37f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944088"
---
# <a name="update-appleuserinitiatedenrollmentprofile"></a><span data-ttu-id="eca38-103">更新 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="eca38-103">Update appleUserInitiatedEnrollmentProfile</span></span>

> <span data-ttu-id="eca38-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eca38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eca38-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eca38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eca38-106">更新[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eca38-106">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eca38-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="eca38-107">Prerequisites</span></span>
<span data-ttu-id="eca38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eca38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eca38-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eca38-110">Permission type</span></span>|<span data-ttu-id="eca38-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eca38-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eca38-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eca38-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eca38-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eca38-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eca38-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eca38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eca38-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eca38-115">Not supported.</span></span>|
|<span data-ttu-id="eca38-116">Application</span><span class="sxs-lookup"><span data-stu-id="eca38-116">Application</span></span>|<span data-ttu-id="eca38-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eca38-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eca38-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eca38-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="eca38-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eca38-119">Request headers</span></span>
|<span data-ttu-id="eca38-120">标头</span><span class="sxs-lookup"><span data-stu-id="eca38-120">Header</span></span>|<span data-ttu-id="eca38-121">值</span><span class="sxs-lookup"><span data-stu-id="eca38-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eca38-122">授权</span><span class="sxs-lookup"><span data-stu-id="eca38-122">Authorization</span></span>|<span data-ttu-id="eca38-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eca38-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eca38-124">接受</span><span class="sxs-lookup"><span data-stu-id="eca38-124">Accept</span></span>|<span data-ttu-id="eca38-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eca38-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eca38-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="eca38-126">Request body</span></span>
<span data-ttu-id="eca38-127">在请求正文中，提供[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eca38-127">In the request body, supply a JSON representation for the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

<span data-ttu-id="eca38-128">下表显示创建[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eca38-128">The following table shows the properties that are required when you create the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>

|<span data-ttu-id="eca38-129">属性</span><span class="sxs-lookup"><span data-stu-id="eca38-129">Property</span></span>|<span data-ttu-id="eca38-130">类型</span><span class="sxs-lookup"><span data-stu-id="eca38-130">Type</span></span>|<span data-ttu-id="eca38-131">说明</span><span class="sxs-lookup"><span data-stu-id="eca38-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eca38-132">defaultEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="eca38-132">defaultEnrollmentType</span></span>|[<span data-ttu-id="eca38-133">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="eca38-133">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="eca38-134">默认配置文件注册类型。</span><span class="sxs-lookup"><span data-stu-id="eca38-134">The default profile enrollment type.</span></span> <span data-ttu-id="eca38-135">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="eca38-135">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="eca38-136">availableEnrollmentTypeOptions</span><span class="sxs-lookup"><span data-stu-id="eca38-136">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="eca38-137">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md)集合</span><span class="sxs-lookup"><span data-stu-id="eca38-137">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="eca38-138">可用注册类型选项的列表</span><span class="sxs-lookup"><span data-stu-id="eca38-138">List of available enrollment type options</span></span>|
|<span data-ttu-id="eca38-139">id</span><span class="sxs-lookup"><span data-stu-id="eca38-139">id</span></span>|<span data-ttu-id="eca38-140">字符串</span><span class="sxs-lookup"><span data-stu-id="eca38-140">String</span></span>|<span data-ttu-id="eca38-141">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="eca38-141">The GUID for the object</span></span>|
|<span data-ttu-id="eca38-142">displayName</span><span class="sxs-lookup"><span data-stu-id="eca38-142">displayName</span></span>|<span data-ttu-id="eca38-143">String</span><span class="sxs-lookup"><span data-stu-id="eca38-143">String</span></span>|<span data-ttu-id="eca38-144">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="eca38-144">Name of the profile</span></span>|
|<span data-ttu-id="eca38-145">说明</span><span class="sxs-lookup"><span data-stu-id="eca38-145">description</span></span>|<span data-ttu-id="eca38-146">String</span><span class="sxs-lookup"><span data-stu-id="eca38-146">String</span></span>|<span data-ttu-id="eca38-147">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="eca38-147">Description of the profile</span></span>|
|<span data-ttu-id="eca38-148">priority</span><span class="sxs-lookup"><span data-stu-id="eca38-148">priority</span></span>|<span data-ttu-id="eca38-149">Int32</span><span class="sxs-lookup"><span data-stu-id="eca38-149">Int32</span></span>|<span data-ttu-id="eca38-150">优先级，0为最高</span><span class="sxs-lookup"><span data-stu-id="eca38-150">Priority, 0 is highest</span></span>|
|<span data-ttu-id="eca38-151">platform</span><span class="sxs-lookup"><span data-stu-id="eca38-151">platform</span></span>|[<span data-ttu-id="eca38-152">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="eca38-152">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="eca38-153">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="eca38-153">The platform of the Device.</span></span> <span data-ttu-id="eca38-154">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="eca38-154">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="eca38-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eca38-155">createdDateTime</span></span>|<span data-ttu-id="eca38-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eca38-156">DateTimeOffset</span></span>|<span data-ttu-id="eca38-157">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="eca38-157">Profile creation time</span></span>|
|<span data-ttu-id="eca38-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eca38-158">lastModifiedDateTime</span></span>|<span data-ttu-id="eca38-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eca38-159">DateTimeOffset</span></span>|<span data-ttu-id="eca38-160">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="eca38-160">Profile last modified time</span></span>|



## <a name="response"></a><span data-ttu-id="eca38-161">响应</span><span class="sxs-lookup"><span data-stu-id="eca38-161">Response</span></span>
<span data-ttu-id="eca38-162">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eca38-162">If successful, this method returns a `200 OK` response code and an updated [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eca38-163">示例</span><span class="sxs-lookup"><span data-stu-id="eca38-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="eca38-164">请求</span><span class="sxs-lookup"><span data-stu-id="eca38-164">Request</span></span>
<span data-ttu-id="eca38-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eca38-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
Content-type: application/json
Content-length: 439

{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "device",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "company",
      "enrollmentType": "device"
    }
  ],
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "platform": "androidForWork"
}
```

### <a name="response"></a><span data-ttu-id="eca38-166">响应</span><span class="sxs-lookup"><span data-stu-id="eca38-166">Response</span></span>
<span data-ttu-id="eca38-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eca38-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "device",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "company",
      "enrollmentType": "device"
    }
  ],
  "id": "5a11d98e-d98e-5a11-8ed9-115a8ed9115a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "platform": "androidForWork",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





