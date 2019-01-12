---
title: 更新 circularGeofenceManagementCondition
description: 更新 circularGeofenceManagementCondition 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 45c6e1d491b652a31ba7e36eac9fb82eef1b235f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963953"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="69c6c-103">更新 circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="69c6c-103">Update circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="69c6c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="69c6c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69c6c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="69c6c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69c6c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="69c6c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69c6c-107">更新[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="69c6c-107">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69c6c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="69c6c-108">Prerequisites</span></span>
<span data-ttu-id="69c6c-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="69c6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69c6c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="69c6c-111">Permission type</span></span>|<span data-ttu-id="69c6c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="69c6c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69c6c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69c6c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69c6c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69c6c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69c6c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69c6c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69c6c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="69c6c-116">Not supported.</span></span>|
|<span data-ttu-id="69c6c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="69c6c-117">Application</span></span>|<span data-ttu-id="69c6c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="69c6c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69c6c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69c6c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="69c6c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="69c6c-120">Request headers</span></span>
|<span data-ttu-id="69c6c-121">标头</span><span class="sxs-lookup"><span data-stu-id="69c6c-121">Header</span></span>|<span data-ttu-id="69c6c-122">值</span><span class="sxs-lookup"><span data-stu-id="69c6c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69c6c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69c6c-123">Authorization</span></span>|<span data-ttu-id="69c6c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="69c6c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69c6c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="69c6c-125">Accept</span></span>|<span data-ttu-id="69c6c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69c6c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69c6c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="69c6c-127">Request body</span></span>
<span data-ttu-id="69c6c-128">在请求正文中，提供[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69c6c-128">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="69c6c-129">下表显示时创建[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="69c6c-129">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="69c6c-130">属性</span><span class="sxs-lookup"><span data-stu-id="69c6c-130">Property</span></span>|<span data-ttu-id="69c6c-131">类型</span><span class="sxs-lookup"><span data-stu-id="69c6c-131">Type</span></span>|<span data-ttu-id="69c6c-132">说明</span><span class="sxs-lookup"><span data-stu-id="69c6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69c6c-133">id</span><span class="sxs-lookup"><span data-stu-id="69c6c-133">id</span></span>|<span data-ttu-id="69c6c-134">字符串</span><span class="sxs-lookup"><span data-stu-id="69c6c-134">String</span></span>|<span data-ttu-id="69c6c-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="69c6c-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="69c6c-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="69c6c-136">System generated value assigned when created.</span></span> <span data-ttu-id="69c6c-137">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="69c6c-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="69c6c-138">唯一名称</span><span class="sxs-lookup"><span data-stu-id="69c6c-138">uniqueName</span></span>|<span data-ttu-id="69c6c-139">字符串</span><span class="sxs-lookup"><span data-stu-id="69c6c-139">String</span></span>|<span data-ttu-id="69c6c-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="69c6c-140">Unique name for the management condition.</span></span> <span data-ttu-id="69c6c-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="69c6c-141">Used in management condition expressions.</span></span> <span data-ttu-id="69c6c-142">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="69c6c-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="69c6c-143">displayName</span><span class="sxs-lookup"><span data-stu-id="69c6c-143">displayName</span></span>|<span data-ttu-id="69c6c-144">字符串</span><span class="sxs-lookup"><span data-stu-id="69c6c-144">String</span></span>|<span data-ttu-id="69c6c-145">管理员定义管理条件的名称。</span><span class="sxs-lookup"><span data-stu-id="69c6c-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="69c6c-146">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="69c6c-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="69c6c-147">说明</span><span class="sxs-lookup"><span data-stu-id="69c6c-147">description</span></span>|<span data-ttu-id="69c6c-148">字符串</span><span class="sxs-lookup"><span data-stu-id="69c6c-148">String</span></span>|<span data-ttu-id="69c6c-149">管理员定义的管理条件说明。</span><span class="sxs-lookup"><span data-stu-id="69c6c-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="69c6c-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="69c6c-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="69c6c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69c6c-151">createdDateTime</span></span>|<span data-ttu-id="69c6c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69c6c-152">DateTimeOffset</span></span>|<span data-ttu-id="69c6c-153">创建管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="69c6c-153">The time the management condition was created.</span></span> <span data-ttu-id="69c6c-154">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="69c6c-154">Generated service side.</span></span> <span data-ttu-id="69c6c-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="69c6c-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="69c6c-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69c6c-156">modifiedDateTime</span></span>|<span data-ttu-id="69c6c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69c6c-157">DateTimeOffset</span></span>|<span data-ttu-id="69c6c-158">管理条件上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="69c6c-158">The time the management condition was last modified.</span></span> <span data-ttu-id="69c6c-159">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="69c6c-159">Updated service side.</span></span> <span data-ttu-id="69c6c-160">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="69c6c-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="69c6c-161">eTag</span><span class="sxs-lookup"><span data-stu-id="69c6c-161">eTag</span></span>|<span data-ttu-id="69c6c-162">String</span><span class="sxs-lookup"><span data-stu-id="69c6c-162">String</span></span>|<span data-ttu-id="69c6c-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="69c6c-163">ETag of the management condition.</span></span> <span data-ttu-id="69c6c-164">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="69c6c-164">Updated service side.</span></span> <span data-ttu-id="69c6c-165">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="69c6c-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="69c6c-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="69c6c-166">applicablePlatforms</span></span>|<span data-ttu-id="69c6c-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="69c6c-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="69c6c-168">此管理条件适用的平台。</span><span class="sxs-lookup"><span data-stu-id="69c6c-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="69c6c-169">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="69c6c-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="69c6c-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="69c6c-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="69c6c-171">latitude</span><span class="sxs-lookup"><span data-stu-id="69c6c-171">latitude</span></span>|<span data-ttu-id="69c6c-172">Double</span><span class="sxs-lookup"><span data-stu-id="69c6c-172">Double</span></span>|<span data-ttu-id="69c6c-173">中度之间-90 到 + 90 非独占的纬度。</span><span class="sxs-lookup"><span data-stu-id="69c6c-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="69c6c-174">longitude</span><span class="sxs-lookup"><span data-stu-id="69c6c-174">longitude</span></span>|<span data-ttu-id="69c6c-175">Double</span><span class="sxs-lookup"><span data-stu-id="69c6c-175">Double</span></span>|<span data-ttu-id="69c6c-176">中度-180 和 180 非独占之间的经度。</span><span class="sxs-lookup"><span data-stu-id="69c6c-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="69c6c-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="69c6c-177">radiusInMeters</span></span>|<span data-ttu-id="69c6c-178">Single</span><span class="sxs-lookup"><span data-stu-id="69c6c-178">Single</span></span>|<span data-ttu-id="69c6c-179">米半径。</span><span class="sxs-lookup"><span data-stu-id="69c6c-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="69c6c-180">响应</span><span class="sxs-lookup"><span data-stu-id="69c6c-180">Response</span></span>
<span data-ttu-id="69c6c-181">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="69c6c-181">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69c6c-182">示例</span><span class="sxs-lookup"><span data-stu-id="69c6c-182">Example</span></span>
### <a name="request"></a><span data-ttu-id="69c6c-183">请求</span><span class="sxs-lookup"><span data-stu-id="69c6c-183">Request</span></span>
<span data-ttu-id="69c6c-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69c6c-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 370

{
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

### <a name="response"></a><span data-ttu-id="69c6c-185">响应</span><span class="sxs-lookup"><span data-stu-id="69c6c-185">Response</span></span>
<span data-ttu-id="69c6c-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69c6c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





