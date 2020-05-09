---
title: 创建 circularGeofenceManagementCondition
description: 创建新的 circularGeofenceManagementCondition 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 76159bf269522433cd3f3dc905d913c71cc4a3ed
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177609"
---
# <a name="create-circulargeofencemanagementcondition"></a><span data-ttu-id="d5bfa-103">创建 circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="d5bfa-103">Create circularGeofenceManagementCondition</span></span>

<span data-ttu-id="d5bfa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5bfa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5bfa-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5bfa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5bfa-107">创建新的[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-107">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5bfa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d5bfa-108">Prerequisites</span></span>
<span data-ttu-id="d5bfa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5bfa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5bfa-111">Permission type</span></span>|<span data-ttu-id="d5bfa-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d5bfa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5bfa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5bfa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5bfa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5bfa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d5bfa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5bfa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5bfa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-116">Not supported.</span></span>|
|<span data-ttu-id="d5bfa-117">Application</span><span class="sxs-lookup"><span data-stu-id="d5bfa-117">Application</span></span>|<span data-ttu-id="d5bfa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5bfa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5bfa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5bfa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="d5bfa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5bfa-120">Request headers</span></span>
|<span data-ttu-id="d5bfa-121">标头</span><span class="sxs-lookup"><span data-stu-id="d5bfa-121">Header</span></span>|<span data-ttu-id="d5bfa-122">值</span><span class="sxs-lookup"><span data-stu-id="d5bfa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5bfa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5bfa-123">Authorization</span></span>|<span data-ttu-id="d5bfa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5bfa-125">接受</span><span class="sxs-lookup"><span data-stu-id="d5bfa-125">Accept</span></span>|<span data-ttu-id="d5bfa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5bfa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5bfa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5bfa-127">Request body</span></span>
<span data-ttu-id="d5bfa-128">在请求正文中，提供 circularGeofenceManagementCondition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-128">In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.</span></span>

<span data-ttu-id="d5bfa-129">下表显示创建 circularGeofenceManagementCondition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-129">The following table shows the properties that are required when you create the circularGeofenceManagementCondition.</span></span>

|<span data-ttu-id="d5bfa-130">属性</span><span class="sxs-lookup"><span data-stu-id="d5bfa-130">Property</span></span>|<span data-ttu-id="d5bfa-131">类型</span><span class="sxs-lookup"><span data-stu-id="d5bfa-131">Type</span></span>|<span data-ttu-id="d5bfa-132">说明</span><span class="sxs-lookup"><span data-stu-id="d5bfa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5bfa-133">id</span><span class="sxs-lookup"><span data-stu-id="d5bfa-133">id</span></span>|<span data-ttu-id="d5bfa-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d5bfa-134">String</span></span>|<span data-ttu-id="d5bfa-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="d5bfa-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-136">System generated value assigned when created.</span></span> <span data-ttu-id="d5bfa-137">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5bfa-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d5bfa-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="d5bfa-138">uniqueName</span></span>|<span data-ttu-id="d5bfa-139">字符串</span><span class="sxs-lookup"><span data-stu-id="d5bfa-139">String</span></span>|<span data-ttu-id="d5bfa-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-140">Unique name for the management condition.</span></span> <span data-ttu-id="d5bfa-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-141">Used in management condition expressions.</span></span> <span data-ttu-id="d5bfa-142">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5bfa-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d5bfa-143">displayName</span><span class="sxs-lookup"><span data-stu-id="d5bfa-143">displayName</span></span>|<span data-ttu-id="d5bfa-144">String</span><span class="sxs-lookup"><span data-stu-id="d5bfa-144">String</span></span>|<span data-ttu-id="d5bfa-145">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="d5bfa-146">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5bfa-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d5bfa-147">说明</span><span class="sxs-lookup"><span data-stu-id="d5bfa-147">description</span></span>|<span data-ttu-id="d5bfa-148">字符串</span><span class="sxs-lookup"><span data-stu-id="d5bfa-148">String</span></span>|<span data-ttu-id="d5bfa-149">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="d5bfa-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5bfa-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d5bfa-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5bfa-151">createdDateTime</span></span>|<span data-ttu-id="d5bfa-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5bfa-152">DateTimeOffset</span></span>|<span data-ttu-id="d5bfa-153">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-153">The time the management condition was created.</span></span> <span data-ttu-id="d5bfa-154">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-154">Generated service side.</span></span> <span data-ttu-id="d5bfa-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5bfa-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d5bfa-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5bfa-156">modifiedDateTime</span></span>|<span data-ttu-id="d5bfa-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5bfa-157">DateTimeOffset</span></span>|<span data-ttu-id="d5bfa-158">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-158">The time the management condition was last modified.</span></span> <span data-ttu-id="d5bfa-159">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-159">Updated service side.</span></span> <span data-ttu-id="d5bfa-160">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5bfa-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d5bfa-161">eTag</span><span class="sxs-lookup"><span data-stu-id="d5bfa-161">eTag</span></span>|<span data-ttu-id="d5bfa-162">String</span><span class="sxs-lookup"><span data-stu-id="d5bfa-162">String</span></span>|<span data-ttu-id="d5bfa-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-163">ETag of the management condition.</span></span> <span data-ttu-id="d5bfa-164">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-164">Updated service side.</span></span> <span data-ttu-id="d5bfa-165">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5bfa-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d5bfa-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="d5bfa-166">applicablePlatforms</span></span>|<span data-ttu-id="d5bfa-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="d5bfa-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="d5bfa-168">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="d5bfa-169">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="d5bfa-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="d5bfa-171">latitude</span><span class="sxs-lookup"><span data-stu-id="d5bfa-171">latitude</span></span>|<span data-ttu-id="d5bfa-172">双精度</span><span class="sxs-lookup"><span data-stu-id="d5bfa-172">Double</span></span>|<span data-ttu-id="d5bfa-173">以度为单位的纬度，介于-90 和 + 90 之间（含）。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="d5bfa-174">longitude</span><span class="sxs-lookup"><span data-stu-id="d5bfa-174">longitude</span></span>|<span data-ttu-id="d5bfa-175">Double</span><span class="sxs-lookup"><span data-stu-id="d5bfa-175">Double</span></span>|<span data-ttu-id="d5bfa-176">以度为单位的经度，介于-180 和 + 180 之间（含）。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="d5bfa-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="d5bfa-177">radiusInMeters</span></span>|<span data-ttu-id="d5bfa-178">单一</span><span class="sxs-lookup"><span data-stu-id="d5bfa-178">Single</span></span>|<span data-ttu-id="d5bfa-179">以米为单位的半径。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="d5bfa-180">响应</span><span class="sxs-lookup"><span data-stu-id="d5bfa-180">Response</span></span>
<span data-ttu-id="d5bfa-181">如果成功，此方法在响应`201 Created`正文中返回响应代码和[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-181">If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5bfa-182">示例</span><span class="sxs-lookup"><span data-stu-id="d5bfa-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5bfa-183">请求</span><span class="sxs-lookup"><span data-stu-id="d5bfa-183">Request</span></span>
<span data-ttu-id="d5bfa-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
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

### <a name="response"></a><span data-ttu-id="d5bfa-185">响应</span><span class="sxs-lookup"><span data-stu-id="d5bfa-185">Response</span></span>
<span data-ttu-id="d5bfa-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5bfa-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



