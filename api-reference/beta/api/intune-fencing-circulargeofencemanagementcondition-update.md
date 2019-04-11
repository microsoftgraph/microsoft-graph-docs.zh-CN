---
title: 更新 circularGeofenceManagementCondition
description: 更新 circularGeofenceManagementCondition 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa9c306ad3e79967223af5c55a628c84c34978b4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776568"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="12adf-103">更新 circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="12adf-103">Update circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="12adf-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12adf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12adf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12adf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12adf-106">更新[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="12adf-106">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12adf-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="12adf-107">Prerequisites</span></span>
<span data-ttu-id="12adf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12adf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12adf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="12adf-110">Permission type</span></span>|<span data-ttu-id="12adf-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12adf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12adf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12adf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12adf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12adf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12adf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12adf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12adf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="12adf-115">Not supported.</span></span>|
|<span data-ttu-id="12adf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="12adf-116">Application</span></span>|<span data-ttu-id="12adf-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="12adf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12adf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12adf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="12adf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="12adf-119">Request headers</span></span>
|<span data-ttu-id="12adf-120">标头</span><span class="sxs-lookup"><span data-stu-id="12adf-120">Header</span></span>|<span data-ttu-id="12adf-121">值</span><span class="sxs-lookup"><span data-stu-id="12adf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12adf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12adf-122">Authorization</span></span>|<span data-ttu-id="12adf-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12adf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12adf-124">接受</span><span class="sxs-lookup"><span data-stu-id="12adf-124">Accept</span></span>|<span data-ttu-id="12adf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12adf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12adf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="12adf-126">Request body</span></span>
<span data-ttu-id="12adf-127">在请求正文中, 提供[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12adf-127">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="12adf-128">下表显示创建[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12adf-128">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="12adf-129">属性</span><span class="sxs-lookup"><span data-stu-id="12adf-129">Property</span></span>|<span data-ttu-id="12adf-130">类型</span><span class="sxs-lookup"><span data-stu-id="12adf-130">Type</span></span>|<span data-ttu-id="12adf-131">说明</span><span class="sxs-lookup"><span data-stu-id="12adf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12adf-132">id</span><span class="sxs-lookup"><span data-stu-id="12adf-132">id</span></span>|<span data-ttu-id="12adf-133">String</span><span class="sxs-lookup"><span data-stu-id="12adf-133">String</span></span>|<span data-ttu-id="12adf-134">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="12adf-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="12adf-135">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="12adf-135">System generated value assigned when created.</span></span> <span data-ttu-id="12adf-136">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="12adf-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="12adf-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="12adf-137">uniqueName</span></span>|<span data-ttu-id="12adf-138">String</span><span class="sxs-lookup"><span data-stu-id="12adf-138">String</span></span>|<span data-ttu-id="12adf-139">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="12adf-139">Unique name for the management condition.</span></span> <span data-ttu-id="12adf-140">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="12adf-140">Used in management condition expressions.</span></span> <span data-ttu-id="12adf-141">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="12adf-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="12adf-142">displayName</span><span class="sxs-lookup"><span data-stu-id="12adf-142">displayName</span></span>|<span data-ttu-id="12adf-143">String</span><span class="sxs-lookup"><span data-stu-id="12adf-143">String</span></span>|<span data-ttu-id="12adf-144">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="12adf-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="12adf-145">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="12adf-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="12adf-146">description</span><span class="sxs-lookup"><span data-stu-id="12adf-146">description</span></span>|<span data-ttu-id="12adf-147">字符串</span><span class="sxs-lookup"><span data-stu-id="12adf-147">String</span></span>|<span data-ttu-id="12adf-148">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="12adf-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="12adf-149">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="12adf-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="12adf-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12adf-150">createdDateTime</span></span>|<span data-ttu-id="12adf-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12adf-151">DateTimeOffset</span></span>|<span data-ttu-id="12adf-152">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="12adf-152">The time the management condition was created.</span></span> <span data-ttu-id="12adf-153">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="12adf-153">Generated service side.</span></span> <span data-ttu-id="12adf-154">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="12adf-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="12adf-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12adf-155">modifiedDateTime</span></span>|<span data-ttu-id="12adf-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12adf-156">DateTimeOffset</span></span>|<span data-ttu-id="12adf-157">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="12adf-157">The time the management condition was last modified.</span></span> <span data-ttu-id="12adf-158">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="12adf-158">Updated service side.</span></span> <span data-ttu-id="12adf-159">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="12adf-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="12adf-160">eTag</span><span class="sxs-lookup"><span data-stu-id="12adf-160">eTag</span></span>|<span data-ttu-id="12adf-161">String</span><span class="sxs-lookup"><span data-stu-id="12adf-161">String</span></span>|<span data-ttu-id="12adf-162">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="12adf-162">ETag of the management condition.</span></span> <span data-ttu-id="12adf-163">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="12adf-163">Updated service side.</span></span> <span data-ttu-id="12adf-164">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="12adf-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="12adf-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="12adf-165">applicablePlatforms</span></span>|<span data-ttu-id="12adf-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="12adf-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="12adf-167">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="12adf-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="12adf-168">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="12adf-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="12adf-169">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="12adf-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="12adf-170">latitude</span><span class="sxs-lookup"><span data-stu-id="12adf-170">latitude</span></span>|<span data-ttu-id="12adf-171">双精度</span><span class="sxs-lookup"><span data-stu-id="12adf-171">Double</span></span>|<span data-ttu-id="12adf-172">以度为单位的纬度, 介于-90 和 + 90 之间 (含)。</span><span class="sxs-lookup"><span data-stu-id="12adf-172">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="12adf-173">longitude</span><span class="sxs-lookup"><span data-stu-id="12adf-173">longitude</span></span>|<span data-ttu-id="12adf-174">Double</span><span class="sxs-lookup"><span data-stu-id="12adf-174">Double</span></span>|<span data-ttu-id="12adf-175">以度为单位的经度, 介于-180 和 + 180 之间 (含)。</span><span class="sxs-lookup"><span data-stu-id="12adf-175">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="12adf-176">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="12adf-176">radiusInMeters</span></span>|<span data-ttu-id="12adf-177">单精度</span><span class="sxs-lookup"><span data-stu-id="12adf-177">Single</span></span>|<span data-ttu-id="12adf-178">以米为单位的半径。</span><span class="sxs-lookup"><span data-stu-id="12adf-178">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="12adf-179">响应</span><span class="sxs-lookup"><span data-stu-id="12adf-179">Response</span></span>
<span data-ttu-id="12adf-180">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="12adf-180">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12adf-181">示例</span><span class="sxs-lookup"><span data-stu-id="12adf-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="12adf-182">请求</span><span class="sxs-lookup"><span data-stu-id="12adf-182">Request</span></span>
<span data-ttu-id="12adf-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12adf-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 444

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```

### <a name="response"></a><span data-ttu-id="12adf-184">响应</span><span class="sxs-lookup"><span data-stu-id="12adf-184">Response</span></span>
<span data-ttu-id="12adf-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12adf-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 612

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
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```





