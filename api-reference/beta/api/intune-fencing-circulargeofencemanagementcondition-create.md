---
title: 创建 circularGeofenceManagementCondition
description: 创建新的 circularGeofenceManagementCondition 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1bf0ba061ff22502ffbdd28c9c2bac3e7fb6c181
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452073"
---
# <a name="create-circulargeofencemanagementcondition"></a><span data-ttu-id="1579f-103">创建 circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="1579f-103">Create circularGeofenceManagementCondition</span></span>

<span data-ttu-id="1579f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1579f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1579f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1579f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1579f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1579f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1579f-107">创建新的[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1579f-107">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1579f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1579f-108">Prerequisites</span></span>
<span data-ttu-id="1579f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1579f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1579f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1579f-111">Permission type</span></span>|<span data-ttu-id="1579f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1579f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1579f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1579f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1579f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1579f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1579f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1579f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1579f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1579f-116">Not supported.</span></span>|
|<span data-ttu-id="1579f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1579f-117">Application</span></span>|<span data-ttu-id="1579f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1579f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1579f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1579f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="1579f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1579f-120">Request headers</span></span>
|<span data-ttu-id="1579f-121">标头</span><span class="sxs-lookup"><span data-stu-id="1579f-121">Header</span></span>|<span data-ttu-id="1579f-122">值</span><span class="sxs-lookup"><span data-stu-id="1579f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1579f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1579f-123">Authorization</span></span>|<span data-ttu-id="1579f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1579f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1579f-125">接受</span><span class="sxs-lookup"><span data-stu-id="1579f-125">Accept</span></span>|<span data-ttu-id="1579f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1579f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1579f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1579f-127">Request body</span></span>
<span data-ttu-id="1579f-128">在请求正文中，提供 circularGeofenceManagementCondition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1579f-128">In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.</span></span>

<span data-ttu-id="1579f-129">下表显示创建 circularGeofenceManagementCondition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1579f-129">The following table shows the properties that are required when you create the circularGeofenceManagementCondition.</span></span>

|<span data-ttu-id="1579f-130">属性</span><span class="sxs-lookup"><span data-stu-id="1579f-130">Property</span></span>|<span data-ttu-id="1579f-131">类型</span><span class="sxs-lookup"><span data-stu-id="1579f-131">Type</span></span>|<span data-ttu-id="1579f-132">说明</span><span class="sxs-lookup"><span data-stu-id="1579f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1579f-133">id</span><span class="sxs-lookup"><span data-stu-id="1579f-133">id</span></span>|<span data-ttu-id="1579f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="1579f-134">String</span></span>|<span data-ttu-id="1579f-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1579f-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="1579f-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="1579f-136">System generated value assigned when created.</span></span> <span data-ttu-id="1579f-137">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1579f-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1579f-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="1579f-138">uniqueName</span></span>|<span data-ttu-id="1579f-139">String</span><span class="sxs-lookup"><span data-stu-id="1579f-139">String</span></span>|<span data-ttu-id="1579f-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="1579f-140">Unique name for the management condition.</span></span> <span data-ttu-id="1579f-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="1579f-141">Used in management condition expressions.</span></span> <span data-ttu-id="1579f-142">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1579f-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1579f-143">displayName</span><span class="sxs-lookup"><span data-stu-id="1579f-143">displayName</span></span>|<span data-ttu-id="1579f-144">String</span><span class="sxs-lookup"><span data-stu-id="1579f-144">String</span></span>|<span data-ttu-id="1579f-145">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="1579f-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="1579f-146">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1579f-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1579f-147">description</span><span class="sxs-lookup"><span data-stu-id="1579f-147">description</span></span>|<span data-ttu-id="1579f-148">字符串</span><span class="sxs-lookup"><span data-stu-id="1579f-148">String</span></span>|<span data-ttu-id="1579f-149">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="1579f-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="1579f-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1579f-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1579f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1579f-151">createdDateTime</span></span>|<span data-ttu-id="1579f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1579f-152">DateTimeOffset</span></span>|<span data-ttu-id="1579f-153">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="1579f-153">The time the management condition was created.</span></span> <span data-ttu-id="1579f-154">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="1579f-154">Generated service side.</span></span> <span data-ttu-id="1579f-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1579f-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1579f-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1579f-156">modifiedDateTime</span></span>|<span data-ttu-id="1579f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1579f-157">DateTimeOffset</span></span>|<span data-ttu-id="1579f-158">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="1579f-158">The time the management condition was last modified.</span></span> <span data-ttu-id="1579f-159">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="1579f-159">Updated service side.</span></span> <span data-ttu-id="1579f-160">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1579f-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1579f-161">eTag</span><span class="sxs-lookup"><span data-stu-id="1579f-161">eTag</span></span>|<span data-ttu-id="1579f-162">String</span><span class="sxs-lookup"><span data-stu-id="1579f-162">String</span></span>|<span data-ttu-id="1579f-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="1579f-163">ETag of the management condition.</span></span> <span data-ttu-id="1579f-164">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="1579f-164">Updated service side.</span></span> <span data-ttu-id="1579f-165">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1579f-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1579f-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="1579f-166">applicablePlatforms</span></span>|<span data-ttu-id="1579f-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="1579f-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="1579f-168">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="1579f-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="1579f-169">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="1579f-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="1579f-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="1579f-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="1579f-171">latitude</span><span class="sxs-lookup"><span data-stu-id="1579f-171">latitude</span></span>|<span data-ttu-id="1579f-172">双精度</span><span class="sxs-lookup"><span data-stu-id="1579f-172">Double</span></span>|<span data-ttu-id="1579f-173">以度为单位的纬度，介于-90 和 + 90 之间（含）。</span><span class="sxs-lookup"><span data-stu-id="1579f-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="1579f-174">longitude</span><span class="sxs-lookup"><span data-stu-id="1579f-174">longitude</span></span>|<span data-ttu-id="1579f-175">Double</span><span class="sxs-lookup"><span data-stu-id="1579f-175">Double</span></span>|<span data-ttu-id="1579f-176">以度为单位的经度，介于-180 和 + 180 之间（含）。</span><span class="sxs-lookup"><span data-stu-id="1579f-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="1579f-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="1579f-177">radiusInMeters</span></span>|<span data-ttu-id="1579f-178">单精度</span><span class="sxs-lookup"><span data-stu-id="1579f-178">Single</span></span>|<span data-ttu-id="1579f-179">以米为单位的半径。</span><span class="sxs-lookup"><span data-stu-id="1579f-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="1579f-180">响应</span><span class="sxs-lookup"><span data-stu-id="1579f-180">Response</span></span>
<span data-ttu-id="1579f-181">如果成功，此方法在响应`201 Created`正文中返回响应代码和[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1579f-181">If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1579f-182">示例</span><span class="sxs-lookup"><span data-stu-id="1579f-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="1579f-183">请求</span><span class="sxs-lookup"><span data-stu-id="1579f-183">Request</span></span>
<span data-ttu-id="1579f-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1579f-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
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

### <a name="response"></a><span data-ttu-id="1579f-185">响应</span><span class="sxs-lookup"><span data-stu-id="1579f-185">Response</span></span>
<span data-ttu-id="1579f-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1579f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



