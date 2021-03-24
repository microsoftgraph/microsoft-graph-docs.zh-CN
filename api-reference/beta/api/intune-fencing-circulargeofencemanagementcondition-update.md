---
title: 更新 circularGeofenceManagementCondition
description: 更新 circularGeofenceManagementCondition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af17c331bde66baef8f6f5b53fa454928da06cfe
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149833"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="03162-103">更新 circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="03162-103">Update circularGeofenceManagementCondition</span></span>

<span data-ttu-id="03162-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03162-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03162-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03162-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03162-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03162-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03162-107">更新 [circularGeofenceManagementCondition 对象](../resources/intune-fencing-circulargeofencemanagementcondition.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="03162-107">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03162-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="03162-108">Prerequisites</span></span>
<span data-ttu-id="03162-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03162-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03162-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="03162-111">Permission type</span></span>|<span data-ttu-id="03162-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03162-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03162-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03162-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03162-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03162-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03162-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03162-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03162-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="03162-116">Not supported.</span></span>|
|<span data-ttu-id="03162-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="03162-117">Application</span></span>|<span data-ttu-id="03162-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03162-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03162-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03162-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="03162-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="03162-120">Request headers</span></span>
|<span data-ttu-id="03162-121">标头</span><span class="sxs-lookup"><span data-stu-id="03162-121">Header</span></span>|<span data-ttu-id="03162-122">值</span><span class="sxs-lookup"><span data-stu-id="03162-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03162-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03162-123">Authorization</span></span>|<span data-ttu-id="03162-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03162-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03162-125">接受</span><span class="sxs-lookup"><span data-stu-id="03162-125">Accept</span></span>|<span data-ttu-id="03162-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03162-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03162-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="03162-127">Request body</span></span>
<span data-ttu-id="03162-128">在请求正文中，提供 [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03162-128">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="03162-129">下表显示创建 [circularGeofenceManagementCondition 时所需的属性](../resources/intune-fencing-circulargeofencemanagementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="03162-129">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="03162-130">属性</span><span class="sxs-lookup"><span data-stu-id="03162-130">Property</span></span>|<span data-ttu-id="03162-131">类型</span><span class="sxs-lookup"><span data-stu-id="03162-131">Type</span></span>|<span data-ttu-id="03162-132">说明</span><span class="sxs-lookup"><span data-stu-id="03162-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03162-133">id</span><span class="sxs-lookup"><span data-stu-id="03162-133">id</span></span>|<span data-ttu-id="03162-134">String</span><span class="sxs-lookup"><span data-stu-id="03162-134">String</span></span>|<span data-ttu-id="03162-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="03162-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="03162-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="03162-136">System generated value assigned when created.</span></span> <span data-ttu-id="03162-137">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="03162-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="03162-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="03162-138">uniqueName</span></span>|<span data-ttu-id="03162-139">String</span><span class="sxs-lookup"><span data-stu-id="03162-139">String</span></span>|<span data-ttu-id="03162-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="03162-140">Unique name for the management condition.</span></span> <span data-ttu-id="03162-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="03162-141">Used in management condition expressions.</span></span> <span data-ttu-id="03162-142">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="03162-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="03162-143">displayName</span><span class="sxs-lookup"><span data-stu-id="03162-143">displayName</span></span>|<span data-ttu-id="03162-144">String</span><span class="sxs-lookup"><span data-stu-id="03162-144">String</span></span>|<span data-ttu-id="03162-145">管理员定义的管理条件名称。</span><span class="sxs-lookup"><span data-stu-id="03162-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="03162-146">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="03162-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="03162-147">说明</span><span class="sxs-lookup"><span data-stu-id="03162-147">description</span></span>|<span data-ttu-id="03162-148">String</span><span class="sxs-lookup"><span data-stu-id="03162-148">String</span></span>|<span data-ttu-id="03162-149">管理员定义的管理条件说明。</span><span class="sxs-lookup"><span data-stu-id="03162-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="03162-150">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="03162-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="03162-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03162-151">createdDateTime</span></span>|<span data-ttu-id="03162-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03162-152">DateTimeOffset</span></span>|<span data-ttu-id="03162-153">创建管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="03162-153">The time the management condition was created.</span></span> <span data-ttu-id="03162-154">生成的服务器端。</span><span class="sxs-lookup"><span data-stu-id="03162-154">Generated service side.</span></span> <span data-ttu-id="03162-155">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="03162-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="03162-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03162-156">modifiedDateTime</span></span>|<span data-ttu-id="03162-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03162-157">DateTimeOffset</span></span>|<span data-ttu-id="03162-158">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="03162-158">The time the management condition was last modified.</span></span> <span data-ttu-id="03162-159">更新的服务器端。</span><span class="sxs-lookup"><span data-stu-id="03162-159">Updated service side.</span></span> <span data-ttu-id="03162-160">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="03162-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="03162-161">eTag</span><span class="sxs-lookup"><span data-stu-id="03162-161">eTag</span></span>|<span data-ttu-id="03162-162">String</span><span class="sxs-lookup"><span data-stu-id="03162-162">String</span></span>|<span data-ttu-id="03162-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="03162-163">ETag of the management condition.</span></span> <span data-ttu-id="03162-164">更新的服务器端。</span><span class="sxs-lookup"><span data-stu-id="03162-164">Updated service side.</span></span> <span data-ttu-id="03162-165">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="03162-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="03162-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="03162-166">applicablePlatforms</span></span>|<span data-ttu-id="03162-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="03162-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="03162-168">此管理条件的适用平台。</span><span class="sxs-lookup"><span data-stu-id="03162-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="03162-169">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="03162-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="03162-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="03162-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="03162-171">latitude</span><span class="sxs-lookup"><span data-stu-id="03162-171">latitude</span></span>|<span data-ttu-id="03162-172">Double</span><span class="sxs-lookup"><span data-stu-id="03162-172">Double</span></span>|<span data-ttu-id="03162-173">纬度（以度数表示），介于 -90 和 +90 之间（含这两者）。</span><span class="sxs-lookup"><span data-stu-id="03162-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="03162-174">longitude</span><span class="sxs-lookup"><span data-stu-id="03162-174">longitude</span></span>|<span data-ttu-id="03162-175">Double</span><span class="sxs-lookup"><span data-stu-id="03162-175">Double</span></span>|<span data-ttu-id="03162-176">以度数表示的经度，介于 -180 和 +180 之间（含这两者）。</span><span class="sxs-lookup"><span data-stu-id="03162-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="03162-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="03162-177">radiusInMeters</span></span>|<span data-ttu-id="03162-178">单一</span><span class="sxs-lookup"><span data-stu-id="03162-178">Single</span></span>|<span data-ttu-id="03162-179">以米为单位的半径。</span><span class="sxs-lookup"><span data-stu-id="03162-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="03162-180">响应</span><span class="sxs-lookup"><span data-stu-id="03162-180">Response</span></span>
<span data-ttu-id="03162-181">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03162-181">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03162-182">示例</span><span class="sxs-lookup"><span data-stu-id="03162-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="03162-183">请求</span><span class="sxs-lookup"><span data-stu-id="03162-183">Request</span></span>
<span data-ttu-id="03162-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03162-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": 2.6666666666666665,
  "longitude": 3.0,
  "radiusInMeters": 4.666666666666667
}
```

### <a name="response"></a><span data-ttu-id="03162-185">响应</span><span class="sxs-lookup"><span data-stu-id="03162-185">Response</span></span>
<span data-ttu-id="03162-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03162-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "id": "30ee27b6-27b6-30ee-b627-ee30b627ee30",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": 2.6666666666666665,
  "longitude": 3.0,
  "radiusInMeters": 4.666666666666667
}
```




