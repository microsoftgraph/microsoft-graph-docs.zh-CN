---
title: 更新 appleUserInitiatedEnrollmentProfile
description: 更新 appleUserInitiatedEnrollmentProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca6dda640ceaadb4420a41cf4bfd0e147f3d29f2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146060"
---
# <a name="update-appleuserinitiatedenrollmentprofile"></a><span data-ttu-id="f6c3d-103">更新 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="f6c3d-103">Update appleUserInitiatedEnrollmentProfile</span></span>

<span data-ttu-id="f6c3d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6c3d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6c3d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6c3d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6c3d-107">更新 [appleUserInitiatedEnrollmentProfile 对象](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-107">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6c3d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f6c3d-108">Prerequisites</span></span>
<span data-ttu-id="f6c3d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6c3d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6c3d-111">Permission type</span></span>|<span data-ttu-id="f6c3d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6c3d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6c3d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6c3d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6c3d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c3d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f6c3d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6c3d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6c3d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-116">Not supported.</span></span>|
|<span data-ttu-id="f6c3d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6c3d-117">Application</span></span>|<span data-ttu-id="f6c3d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c3d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6c3d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6c3d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="f6c3d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6c3d-120">Request headers</span></span>
|<span data-ttu-id="f6c3d-121">标头</span><span class="sxs-lookup"><span data-stu-id="f6c3d-121">Header</span></span>|<span data-ttu-id="f6c3d-122">值</span><span class="sxs-lookup"><span data-stu-id="f6c3d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6c3d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6c3d-123">Authorization</span></span>|<span data-ttu-id="f6c3d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6c3d-125">接受</span><span class="sxs-lookup"><span data-stu-id="f6c3d-125">Accept</span></span>|<span data-ttu-id="f6c3d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6c3d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6c3d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6c3d-127">Request body</span></span>
<span data-ttu-id="f6c3d-128">在请求正文中，提供 [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-128">In the request body, supply a JSON representation for the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

<span data-ttu-id="f6c3d-129">下表显示创建 [appleUserInitiatedEnrollmentProfile 时所需的属性](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-129">The following table shows the properties that are required when you create the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>

|<span data-ttu-id="f6c3d-130">属性</span><span class="sxs-lookup"><span data-stu-id="f6c3d-130">Property</span></span>|<span data-ttu-id="f6c3d-131">类型</span><span class="sxs-lookup"><span data-stu-id="f6c3d-131">Type</span></span>|<span data-ttu-id="f6c3d-132">说明</span><span class="sxs-lookup"><span data-stu-id="f6c3d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6c3d-133">defaultEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f6c3d-133">defaultEnrollmentType</span></span>|[<span data-ttu-id="f6c3d-134">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f6c3d-134">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="f6c3d-135">默认配置文件注册类型。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-135">The default profile enrollment type.</span></span> <span data-ttu-id="f6c3d-136">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-136">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="f6c3d-137">availableEnrollmentTypeOptions</span><span class="sxs-lookup"><span data-stu-id="f6c3d-137">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="f6c3d-138">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f6c3d-138">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="f6c3d-139">可用注册类型选项列表</span><span class="sxs-lookup"><span data-stu-id="f6c3d-139">List of available enrollment type options</span></span>|
|<span data-ttu-id="f6c3d-140">id</span><span class="sxs-lookup"><span data-stu-id="f6c3d-140">id</span></span>|<span data-ttu-id="f6c3d-141">String</span><span class="sxs-lookup"><span data-stu-id="f6c3d-141">String</span></span>|<span data-ttu-id="f6c3d-142">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="f6c3d-142">The GUID for the object</span></span>|
|<span data-ttu-id="f6c3d-143">displayName</span><span class="sxs-lookup"><span data-stu-id="f6c3d-143">displayName</span></span>|<span data-ttu-id="f6c3d-144">String</span><span class="sxs-lookup"><span data-stu-id="f6c3d-144">String</span></span>|<span data-ttu-id="f6c3d-145">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="f6c3d-145">Name of the profile</span></span>|
|<span data-ttu-id="f6c3d-146">说明</span><span class="sxs-lookup"><span data-stu-id="f6c3d-146">description</span></span>|<span data-ttu-id="f6c3d-147">String</span><span class="sxs-lookup"><span data-stu-id="f6c3d-147">String</span></span>|<span data-ttu-id="f6c3d-148">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="f6c3d-148">Description of the profile</span></span>|
|<span data-ttu-id="f6c3d-149">priority</span><span class="sxs-lookup"><span data-stu-id="f6c3d-149">priority</span></span>|<span data-ttu-id="f6c3d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f6c3d-150">Int32</span></span>|<span data-ttu-id="f6c3d-151">优先级，0 为最高</span><span class="sxs-lookup"><span data-stu-id="f6c3d-151">Priority, 0 is highest</span></span>|
|<span data-ttu-id="f6c3d-152">平台</span><span class="sxs-lookup"><span data-stu-id="f6c3d-152">platform</span></span>|[<span data-ttu-id="f6c3d-153">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="f6c3d-153">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="f6c3d-154">设备平台。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-154">The platform of the Device.</span></span> <span data-ttu-id="f6c3d-155">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-155">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="f6c3d-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6c3d-156">createdDateTime</span></span>|<span data-ttu-id="f6c3d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6c3d-157">DateTimeOffset</span></span>|<span data-ttu-id="f6c3d-158">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="f6c3d-158">Profile creation time</span></span>|
|<span data-ttu-id="f6c3d-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6c3d-159">lastModifiedDateTime</span></span>|<span data-ttu-id="f6c3d-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6c3d-160">DateTimeOffset</span></span>|<span data-ttu-id="f6c3d-161">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="f6c3d-161">Profile last modified time</span></span>|



## <a name="response"></a><span data-ttu-id="f6c3d-162">响应</span><span class="sxs-lookup"><span data-stu-id="f6c3d-162">Response</span></span>
<span data-ttu-id="f6c3d-163">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-163">If successful, this method returns a `200 OK` response code and an updated [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6c3d-164">示例</span><span class="sxs-lookup"><span data-stu-id="f6c3d-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6c3d-165">请求</span><span class="sxs-lookup"><span data-stu-id="f6c3d-165">Request</span></span>
<span data-ttu-id="f6c3d-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f6c3d-167">响应</span><span class="sxs-lookup"><span data-stu-id="f6c3d-167">Response</span></span>
<span data-ttu-id="f6c3d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f6c3d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




