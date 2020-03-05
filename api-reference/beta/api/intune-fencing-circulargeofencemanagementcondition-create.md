---
title: 创建 circularGeofenceManagementCondition
description: 创建新的 circularGeofenceManagementCondition 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fcae78759cfd13042d4baef6958f1c3cb835f2ce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465938"
---
# <a name="create-circulargeofencemanagementcondition"></a><span data-ttu-id="ffdc1-103">创建 circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="ffdc1-103">Create circularGeofenceManagementCondition</span></span>

<span data-ttu-id="ffdc1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ffdc1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ffdc1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffdc1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffdc1-107">创建新的[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-107">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffdc1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ffdc1-108">Prerequisites</span></span>
<span data-ttu-id="ffdc1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffdc1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ffdc1-111">Permission type</span></span>|<span data-ttu-id="ffdc1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ffdc1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffdc1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ffdc1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffdc1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffdc1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ffdc1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ffdc1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffdc1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-116">Not supported.</span></span>|
|<span data-ttu-id="ffdc1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ffdc1-117">Application</span></span>|<span data-ttu-id="ffdc1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffdc1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffdc1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffdc1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="ffdc1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ffdc1-120">Request headers</span></span>
|<span data-ttu-id="ffdc1-121">标头</span><span class="sxs-lookup"><span data-stu-id="ffdc1-121">Header</span></span>|<span data-ttu-id="ffdc1-122">值</span><span class="sxs-lookup"><span data-stu-id="ffdc1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffdc1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffdc1-123">Authorization</span></span>|<span data-ttu-id="ffdc1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffdc1-125">接受</span><span class="sxs-lookup"><span data-stu-id="ffdc1-125">Accept</span></span>|<span data-ttu-id="ffdc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffdc1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffdc1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ffdc1-127">Request body</span></span>
<span data-ttu-id="ffdc1-128">在请求正文中，提供 circularGeofenceManagementCondition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-128">In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.</span></span>

<span data-ttu-id="ffdc1-129">下表显示创建 circularGeofenceManagementCondition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-129">The following table shows the properties that are required when you create the circularGeofenceManagementCondition.</span></span>

|<span data-ttu-id="ffdc1-130">属性</span><span class="sxs-lookup"><span data-stu-id="ffdc1-130">Property</span></span>|<span data-ttu-id="ffdc1-131">类型</span><span class="sxs-lookup"><span data-stu-id="ffdc1-131">Type</span></span>|<span data-ttu-id="ffdc1-132">说明</span><span class="sxs-lookup"><span data-stu-id="ffdc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffdc1-133">id</span><span class="sxs-lookup"><span data-stu-id="ffdc1-133">id</span></span>|<span data-ttu-id="ffdc1-134">字符串</span><span class="sxs-lookup"><span data-stu-id="ffdc1-134">String</span></span>|<span data-ttu-id="ffdc1-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="ffdc1-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-136">System generated value assigned when created.</span></span> <span data-ttu-id="ffdc1-137">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ffdc1-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ffdc1-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="ffdc1-138">uniqueName</span></span>|<span data-ttu-id="ffdc1-139">String</span><span class="sxs-lookup"><span data-stu-id="ffdc1-139">String</span></span>|<span data-ttu-id="ffdc1-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-140">Unique name for the management condition.</span></span> <span data-ttu-id="ffdc1-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-141">Used in management condition expressions.</span></span> <span data-ttu-id="ffdc1-142">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ffdc1-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ffdc1-143">displayName</span><span class="sxs-lookup"><span data-stu-id="ffdc1-143">displayName</span></span>|<span data-ttu-id="ffdc1-144">String</span><span class="sxs-lookup"><span data-stu-id="ffdc1-144">String</span></span>|<span data-ttu-id="ffdc1-145">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="ffdc1-146">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ffdc1-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ffdc1-147">说明</span><span class="sxs-lookup"><span data-stu-id="ffdc1-147">description</span></span>|<span data-ttu-id="ffdc1-148">字符串</span><span class="sxs-lookup"><span data-stu-id="ffdc1-148">String</span></span>|<span data-ttu-id="ffdc1-149">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="ffdc1-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ffdc1-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ffdc1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffdc1-151">createdDateTime</span></span>|<span data-ttu-id="ffdc1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffdc1-152">DateTimeOffset</span></span>|<span data-ttu-id="ffdc1-153">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-153">The time the management condition was created.</span></span> <span data-ttu-id="ffdc1-154">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-154">Generated service side.</span></span> <span data-ttu-id="ffdc1-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ffdc1-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ffdc1-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffdc1-156">modifiedDateTime</span></span>|<span data-ttu-id="ffdc1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffdc1-157">DateTimeOffset</span></span>|<span data-ttu-id="ffdc1-158">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-158">The time the management condition was last modified.</span></span> <span data-ttu-id="ffdc1-159">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-159">Updated service side.</span></span> <span data-ttu-id="ffdc1-160">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ffdc1-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ffdc1-161">eTag</span><span class="sxs-lookup"><span data-stu-id="ffdc1-161">eTag</span></span>|<span data-ttu-id="ffdc1-162">String</span><span class="sxs-lookup"><span data-stu-id="ffdc1-162">String</span></span>|<span data-ttu-id="ffdc1-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-163">ETag of the management condition.</span></span> <span data-ttu-id="ffdc1-164">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-164">Updated service side.</span></span> <span data-ttu-id="ffdc1-165">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ffdc1-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ffdc1-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="ffdc1-166">applicablePlatforms</span></span>|<span data-ttu-id="ffdc1-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="ffdc1-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="ffdc1-168">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="ffdc1-169">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="ffdc1-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="ffdc1-171">latitude</span><span class="sxs-lookup"><span data-stu-id="ffdc1-171">latitude</span></span>|<span data-ttu-id="ffdc1-172">双精度</span><span class="sxs-lookup"><span data-stu-id="ffdc1-172">Double</span></span>|<span data-ttu-id="ffdc1-173">以度为单位的纬度，介于-90 和 + 90 之间（含）。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="ffdc1-174">longitude</span><span class="sxs-lookup"><span data-stu-id="ffdc1-174">longitude</span></span>|<span data-ttu-id="ffdc1-175">Double</span><span class="sxs-lookup"><span data-stu-id="ffdc1-175">Double</span></span>|<span data-ttu-id="ffdc1-176">以度为单位的经度，介于-180 和 + 180 之间（含）。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="ffdc1-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="ffdc1-177">radiusInMeters</span></span>|<span data-ttu-id="ffdc1-178">单精度</span><span class="sxs-lookup"><span data-stu-id="ffdc1-178">Single</span></span>|<span data-ttu-id="ffdc1-179">以米为单位的半径。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="ffdc1-180">响应</span><span class="sxs-lookup"><span data-stu-id="ffdc1-180">Response</span></span>
<span data-ttu-id="ffdc1-181">如果成功，此方法在响应`201 Created`正文中返回响应代码和[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-181">If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffdc1-182">示例</span><span class="sxs-lookup"><span data-stu-id="ffdc1-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffdc1-183">请求</span><span class="sxs-lookup"><span data-stu-id="ffdc1-183">Request</span></span>
<span data-ttu-id="ffdc1-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ffdc1-185">响应</span><span class="sxs-lookup"><span data-stu-id="ffdc1-185">Response</span></span>
<span data-ttu-id="ffdc1-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ffdc1-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





