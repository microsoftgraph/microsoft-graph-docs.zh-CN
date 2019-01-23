---
title: 更新 circularGeofenceManagementCondition
description: 更新 circularGeofenceManagementCondition 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e329aeeb62844d85742673db93e3fb2549680456
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424600"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="981f5-103">更新 circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="981f5-103">Update circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="981f5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="981f5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="981f5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="981f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="981f5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="981f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="981f5-107">更新[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="981f5-107">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="981f5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="981f5-108">Prerequisites</span></span>
<span data-ttu-id="981f5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="981f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="981f5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="981f5-111">Permission type</span></span>|<span data-ttu-id="981f5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="981f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="981f5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="981f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="981f5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="981f5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="981f5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="981f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="981f5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="981f5-116">Not supported.</span></span>|
|<span data-ttu-id="981f5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="981f5-117">Application</span></span>|<span data-ttu-id="981f5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="981f5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="981f5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="981f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="981f5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="981f5-120">Request headers</span></span>
|<span data-ttu-id="981f5-121">标头</span><span class="sxs-lookup"><span data-stu-id="981f5-121">Header</span></span>|<span data-ttu-id="981f5-122">值</span><span class="sxs-lookup"><span data-stu-id="981f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="981f5-123">授权</span><span class="sxs-lookup"><span data-stu-id="981f5-123">Authorization</span></span>|<span data-ttu-id="981f5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="981f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="981f5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="981f5-125">Accept</span></span>|<span data-ttu-id="981f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="981f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="981f5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="981f5-127">Request body</span></span>
<span data-ttu-id="981f5-128">在请求正文中，提供[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="981f5-128">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="981f5-129">下表显示时创建[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="981f5-129">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="981f5-130">属性</span><span class="sxs-lookup"><span data-stu-id="981f5-130">Property</span></span>|<span data-ttu-id="981f5-131">类型</span><span class="sxs-lookup"><span data-stu-id="981f5-131">Type</span></span>|<span data-ttu-id="981f5-132">说明</span><span class="sxs-lookup"><span data-stu-id="981f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="981f5-133">id</span><span class="sxs-lookup"><span data-stu-id="981f5-133">id</span></span>|<span data-ttu-id="981f5-134">String</span><span class="sxs-lookup"><span data-stu-id="981f5-134">String</span></span>|<span data-ttu-id="981f5-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="981f5-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="981f5-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="981f5-136">System generated value assigned when created.</span></span> <span data-ttu-id="981f5-137">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="981f5-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="981f5-138">唯一名称</span><span class="sxs-lookup"><span data-stu-id="981f5-138">uniqueName</span></span>|<span data-ttu-id="981f5-139">String</span><span class="sxs-lookup"><span data-stu-id="981f5-139">String</span></span>|<span data-ttu-id="981f5-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="981f5-140">Unique name for the management condition.</span></span> <span data-ttu-id="981f5-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="981f5-141">Used in management condition expressions.</span></span> <span data-ttu-id="981f5-142">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="981f5-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="981f5-143">displayName</span><span class="sxs-lookup"><span data-stu-id="981f5-143">displayName</span></span>|<span data-ttu-id="981f5-144">String</span><span class="sxs-lookup"><span data-stu-id="981f5-144">String</span></span>|<span data-ttu-id="981f5-145">管理员定义管理条件的名称。</span><span class="sxs-lookup"><span data-stu-id="981f5-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="981f5-146">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="981f5-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="981f5-147">说明</span><span class="sxs-lookup"><span data-stu-id="981f5-147">description</span></span>|<span data-ttu-id="981f5-148">String</span><span class="sxs-lookup"><span data-stu-id="981f5-148">String</span></span>|<span data-ttu-id="981f5-149">管理员定义的管理条件说明。</span><span class="sxs-lookup"><span data-stu-id="981f5-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="981f5-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="981f5-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="981f5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="981f5-151">createdDateTime</span></span>|<span data-ttu-id="981f5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="981f5-152">DateTimeOffset</span></span>|<span data-ttu-id="981f5-153">创建管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="981f5-153">The time the management condition was created.</span></span> <span data-ttu-id="981f5-154">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="981f5-154">Generated service side.</span></span> <span data-ttu-id="981f5-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="981f5-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="981f5-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="981f5-156">modifiedDateTime</span></span>|<span data-ttu-id="981f5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="981f5-157">DateTimeOffset</span></span>|<span data-ttu-id="981f5-158">管理条件上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="981f5-158">The time the management condition was last modified.</span></span> <span data-ttu-id="981f5-159">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="981f5-159">Updated service side.</span></span> <span data-ttu-id="981f5-160">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="981f5-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="981f5-161">eTag</span><span class="sxs-lookup"><span data-stu-id="981f5-161">eTag</span></span>|<span data-ttu-id="981f5-162">String</span><span class="sxs-lookup"><span data-stu-id="981f5-162">String</span></span>|<span data-ttu-id="981f5-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="981f5-163">ETag of the management condition.</span></span> <span data-ttu-id="981f5-164">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="981f5-164">Updated service side.</span></span> <span data-ttu-id="981f5-165">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="981f5-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="981f5-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="981f5-166">applicablePlatforms</span></span>|<span data-ttu-id="981f5-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="981f5-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="981f5-168">此管理条件适用的平台。</span><span class="sxs-lookup"><span data-stu-id="981f5-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="981f5-169">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="981f5-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="981f5-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="981f5-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="981f5-171">latitude</span><span class="sxs-lookup"><span data-stu-id="981f5-171">latitude</span></span>|<span data-ttu-id="981f5-172">Double</span><span class="sxs-lookup"><span data-stu-id="981f5-172">Double</span></span>|<span data-ttu-id="981f5-173">中度之间-90 到 + 90 非独占的纬度。</span><span class="sxs-lookup"><span data-stu-id="981f5-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="981f5-174">longitude</span><span class="sxs-lookup"><span data-stu-id="981f5-174">longitude</span></span>|<span data-ttu-id="981f5-175">Double</span><span class="sxs-lookup"><span data-stu-id="981f5-175">Double</span></span>|<span data-ttu-id="981f5-176">中度-180 和 180 非独占之间的经度。</span><span class="sxs-lookup"><span data-stu-id="981f5-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="981f5-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="981f5-177">radiusInMeters</span></span>|<span data-ttu-id="981f5-178">单精度</span><span class="sxs-lookup"><span data-stu-id="981f5-178">Single</span></span>|<span data-ttu-id="981f5-179">米半径。</span><span class="sxs-lookup"><span data-stu-id="981f5-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="981f5-180">响应</span><span class="sxs-lookup"><span data-stu-id="981f5-180">Response</span></span>
<span data-ttu-id="981f5-181">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="981f5-181">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="981f5-182">示例</span><span class="sxs-lookup"><span data-stu-id="981f5-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="981f5-183">请求</span><span class="sxs-lookup"><span data-stu-id="981f5-183">Request</span></span>
<span data-ttu-id="981f5-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="981f5-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="981f5-185">响应</span><span class="sxs-lookup"><span data-stu-id="981f5-185">Response</span></span>
<span data-ttu-id="981f5-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="981f5-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




