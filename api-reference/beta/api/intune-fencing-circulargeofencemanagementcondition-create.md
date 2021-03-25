---
title: 创建 circularGeofenceManagementCondition
description: 创建新的 circularGeofenceManagementCondition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 882dce92202dc0db2fbb2ca31aeb8fa52162ba4d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157560"
---
# <a name="create-circulargeofencemanagementcondition"></a><span data-ttu-id="0d56c-103">创建 circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="0d56c-103">Create circularGeofenceManagementCondition</span></span>

<span data-ttu-id="0d56c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d56c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d56c-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0d56c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d56c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0d56c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d56c-107">创建新的 [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0d56c-107">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d56c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0d56c-108">Prerequisites</span></span>
<span data-ttu-id="0d56c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d56c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d56c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d56c-111">Permission type</span></span>|<span data-ttu-id="0d56c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d56c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d56c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d56c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d56c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d56c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d56c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d56c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d56c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d56c-116">Not supported.</span></span>|
|<span data-ttu-id="0d56c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d56c-117">Application</span></span>|<span data-ttu-id="0d56c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d56c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d56c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d56c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="0d56c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d56c-120">Request headers</span></span>
|<span data-ttu-id="0d56c-121">标头</span><span class="sxs-lookup"><span data-stu-id="0d56c-121">Header</span></span>|<span data-ttu-id="0d56c-122">值</span><span class="sxs-lookup"><span data-stu-id="0d56c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d56c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d56c-123">Authorization</span></span>|<span data-ttu-id="0d56c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0d56c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d56c-125">接受</span><span class="sxs-lookup"><span data-stu-id="0d56c-125">Accept</span></span>|<span data-ttu-id="0d56c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d56c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d56c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d56c-127">Request body</span></span>
<span data-ttu-id="0d56c-128">在请求正文中，提供 circularGeofenceManagementCondition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d56c-128">In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.</span></span>

<span data-ttu-id="0d56c-129">下表显示创建 circularGeofenceManagementCondition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0d56c-129">The following table shows the properties that are required when you create the circularGeofenceManagementCondition.</span></span>

|<span data-ttu-id="0d56c-130">属性</span><span class="sxs-lookup"><span data-stu-id="0d56c-130">Property</span></span>|<span data-ttu-id="0d56c-131">类型</span><span class="sxs-lookup"><span data-stu-id="0d56c-131">Type</span></span>|<span data-ttu-id="0d56c-132">说明</span><span class="sxs-lookup"><span data-stu-id="0d56c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d56c-133">id</span><span class="sxs-lookup"><span data-stu-id="0d56c-133">id</span></span>|<span data-ttu-id="0d56c-134">String</span><span class="sxs-lookup"><span data-stu-id="0d56c-134">String</span></span>|<span data-ttu-id="0d56c-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0d56c-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="0d56c-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="0d56c-136">System generated value assigned when created.</span></span> <span data-ttu-id="0d56c-137">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0d56c-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0d56c-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="0d56c-138">uniqueName</span></span>|<span data-ttu-id="0d56c-139">String</span><span class="sxs-lookup"><span data-stu-id="0d56c-139">String</span></span>|<span data-ttu-id="0d56c-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="0d56c-140">Unique name for the management condition.</span></span> <span data-ttu-id="0d56c-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="0d56c-141">Used in management condition expressions.</span></span> <span data-ttu-id="0d56c-142">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0d56c-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0d56c-143">displayName</span><span class="sxs-lookup"><span data-stu-id="0d56c-143">displayName</span></span>|<span data-ttu-id="0d56c-144">String</span><span class="sxs-lookup"><span data-stu-id="0d56c-144">String</span></span>|<span data-ttu-id="0d56c-145">管理员定义的管理条件名称。</span><span class="sxs-lookup"><span data-stu-id="0d56c-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="0d56c-146">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0d56c-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0d56c-147">说明</span><span class="sxs-lookup"><span data-stu-id="0d56c-147">description</span></span>|<span data-ttu-id="0d56c-148">String</span><span class="sxs-lookup"><span data-stu-id="0d56c-148">String</span></span>|<span data-ttu-id="0d56c-149">管理员定义的管理条件说明。</span><span class="sxs-lookup"><span data-stu-id="0d56c-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="0d56c-150">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0d56c-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0d56c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d56c-151">createdDateTime</span></span>|<span data-ttu-id="0d56c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d56c-152">DateTimeOffset</span></span>|<span data-ttu-id="0d56c-153">创建管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="0d56c-153">The time the management condition was created.</span></span> <span data-ttu-id="0d56c-154">生成的服务器端。</span><span class="sxs-lookup"><span data-stu-id="0d56c-154">Generated service side.</span></span> <span data-ttu-id="0d56c-155">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0d56c-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0d56c-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d56c-156">modifiedDateTime</span></span>|<span data-ttu-id="0d56c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d56c-157">DateTimeOffset</span></span>|<span data-ttu-id="0d56c-158">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="0d56c-158">The time the management condition was last modified.</span></span> <span data-ttu-id="0d56c-159">更新的服务器端。</span><span class="sxs-lookup"><span data-stu-id="0d56c-159">Updated service side.</span></span> <span data-ttu-id="0d56c-160">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0d56c-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0d56c-161">eTag</span><span class="sxs-lookup"><span data-stu-id="0d56c-161">eTag</span></span>|<span data-ttu-id="0d56c-162">String</span><span class="sxs-lookup"><span data-stu-id="0d56c-162">String</span></span>|<span data-ttu-id="0d56c-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="0d56c-163">ETag of the management condition.</span></span> <span data-ttu-id="0d56c-164">更新的服务器端。</span><span class="sxs-lookup"><span data-stu-id="0d56c-164">Updated service side.</span></span> <span data-ttu-id="0d56c-165">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0d56c-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0d56c-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="0d56c-166">applicablePlatforms</span></span>|<span data-ttu-id="0d56c-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d56c-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="0d56c-168">此管理条件的适用平台。</span><span class="sxs-lookup"><span data-stu-id="0d56c-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="0d56c-169">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="0d56c-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="0d56c-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="0d56c-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="0d56c-171">latitude</span><span class="sxs-lookup"><span data-stu-id="0d56c-171">latitude</span></span>|<span data-ttu-id="0d56c-172">Double</span><span class="sxs-lookup"><span data-stu-id="0d56c-172">Double</span></span>|<span data-ttu-id="0d56c-173">纬度（以度数表示），介于 -90 和 +90 之间（含这两者）。</span><span class="sxs-lookup"><span data-stu-id="0d56c-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="0d56c-174">longitude</span><span class="sxs-lookup"><span data-stu-id="0d56c-174">longitude</span></span>|<span data-ttu-id="0d56c-175">Double</span><span class="sxs-lookup"><span data-stu-id="0d56c-175">Double</span></span>|<span data-ttu-id="0d56c-176">以度数表示的经度，介于 -180 和 +180 之间（含这两者）。</span><span class="sxs-lookup"><span data-stu-id="0d56c-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="0d56c-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="0d56c-177">radiusInMeters</span></span>|<span data-ttu-id="0d56c-178">单一</span><span class="sxs-lookup"><span data-stu-id="0d56c-178">Single</span></span>|<span data-ttu-id="0d56c-179">以米为单位的半径。</span><span class="sxs-lookup"><span data-stu-id="0d56c-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="0d56c-180">响应</span><span class="sxs-lookup"><span data-stu-id="0d56c-180">Response</span></span>
<span data-ttu-id="0d56c-181">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0d56c-181">If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d56c-182">示例</span><span class="sxs-lookup"><span data-stu-id="0d56c-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d56c-183">请求</span><span class="sxs-lookup"><span data-stu-id="0d56c-183">Request</span></span>
<span data-ttu-id="0d56c-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0d56c-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d56c-185">响应</span><span class="sxs-lookup"><span data-stu-id="0d56c-185">Response</span></span>
<span data-ttu-id="0d56c-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0d56c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




