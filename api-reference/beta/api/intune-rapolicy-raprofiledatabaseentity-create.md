---
title: 创建 raProfileDatabaseEntity
description: 创建新的 raProfileDatabaseEntity 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb892f1a64dd1223956f3fda73a6aeb8512edf00
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124249"
---
# <a name="create-raprofiledatabaseentity"></a><span data-ttu-id="365d4-103">创建 raProfileDatabaseEntity</span><span class="sxs-lookup"><span data-stu-id="365d4-103">Create raProfileDatabaseEntity</span></span>

<span data-ttu-id="365d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="365d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="365d4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="365d4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="365d4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="365d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="365d4-107">创建新的[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="365d4-107">Create a new [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="365d4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="365d4-108">Prerequisites</span></span>
<span data-ttu-id="365d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="365d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="365d4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="365d4-111">Permission type</span></span>|<span data-ttu-id="365d4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="365d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="365d4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="365d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="365d4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="365d4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="365d4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="365d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="365d4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="365d4-116">Not supported.</span></span>|
|<span data-ttu-id="365d4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="365d4-117">Application</span></span>|<span data-ttu-id="365d4-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="365d4-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="365d4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="365d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /resourceAccessProfileEntities
```

## <a name="request-headers"></a><span data-ttu-id="365d4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="365d4-120">Request headers</span></span>
|<span data-ttu-id="365d4-121">标头</span><span class="sxs-lookup"><span data-stu-id="365d4-121">Header</span></span>|<span data-ttu-id="365d4-122">值</span><span class="sxs-lookup"><span data-stu-id="365d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="365d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="365d4-123">Authorization</span></span>|<span data-ttu-id="365d4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="365d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="365d4-125">接受</span><span class="sxs-lookup"><span data-stu-id="365d4-125">Accept</span></span>|<span data-ttu-id="365d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="365d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="365d4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="365d4-127">Request body</span></span>
<span data-ttu-id="365d4-128">在请求正文中，提供 raProfileDatabaseEntity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="365d4-128">In the request body, supply a JSON representation for the raProfileDatabaseEntity object.</span></span>

<span data-ttu-id="365d4-129">下表显示创建 raProfileDatabaseEntity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="365d4-129">The following table shows the properties that are required when you create the raProfileDatabaseEntity.</span></span>

|<span data-ttu-id="365d4-130">属性</span><span class="sxs-lookup"><span data-stu-id="365d4-130">Property</span></span>|<span data-ttu-id="365d4-131">类型</span><span class="sxs-lookup"><span data-stu-id="365d4-131">Type</span></span>|<span data-ttu-id="365d4-132">说明</span><span class="sxs-lookup"><span data-stu-id="365d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="365d4-133">version</span><span class="sxs-lookup"><span data-stu-id="365d4-133">version</span></span>|<span data-ttu-id="365d4-134">Int32</span><span class="sxs-lookup"><span data-stu-id="365d4-134">Int32</span></span>|<span data-ttu-id="365d4-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-135">Not yet documented</span></span>|
|<span data-ttu-id="365d4-136">isDeleted</span><span class="sxs-lookup"><span data-stu-id="365d4-136">isDeleted</span></span>|<span data-ttu-id="365d4-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="365d4-137">Boolean</span></span>|<span data-ttu-id="365d4-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-138">Not yet documented</span></span>|
|<span data-ttu-id="365d4-139">softDeletedTime</span><span class="sxs-lookup"><span data-stu-id="365d4-139">softDeletedTime</span></span>|<span data-ttu-id="365d4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="365d4-140">DateTimeOffset</span></span>|<span data-ttu-id="365d4-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-141">Not yet documented</span></span>|
|<span data-ttu-id="365d4-142">displayName</span><span class="sxs-lookup"><span data-stu-id="365d4-142">displayName</span></span>|<span data-ttu-id="365d4-143">String</span><span class="sxs-lookup"><span data-stu-id="365d4-143">String</span></span>|<span data-ttu-id="365d4-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-144">Not yet documented</span></span>|
|<span data-ttu-id="365d4-145">linkedProfileIds</span><span class="sxs-lookup"><span data-stu-id="365d4-145">linkedProfileIds</span></span>|<span data-ttu-id="365d4-146">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="365d4-146">Guid collection</span></span>|<span data-ttu-id="365d4-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-147">Not yet documented</span></span>|
|<span data-ttu-id="365d4-148">profileTypeName</span><span class="sxs-lookup"><span data-stu-id="365d4-148">profileTypeName</span></span>|<span data-ttu-id="365d4-149">String</span><span class="sxs-lookup"><span data-stu-id="365d4-149">String</span></span>|<span data-ttu-id="365d4-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-150">Not yet documented</span></span>|
|<span data-ttu-id="365d4-151">profileBody</span><span class="sxs-lookup"><span data-stu-id="365d4-151">profileBody</span></span>|<span data-ttu-id="365d4-152">String</span><span class="sxs-lookup"><span data-stu-id="365d4-152">String</span></span>|<span data-ttu-id="365d4-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-153">Not yet documented</span></span>|
|<span data-ttu-id="365d4-154">profileBodyHash</span><span class="sxs-lookup"><span data-stu-id="365d4-154">profileBodyHash</span></span>|<span data-ttu-id="365d4-155">String</span><span class="sxs-lookup"><span data-stu-id="365d4-155">String</span></span>|<span data-ttu-id="365d4-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-156">Not yet documented</span></span>|
|<span data-ttu-id="365d4-157">platformType</span><span class="sxs-lookup"><span data-stu-id="365d4-157">platformType</span></span>|<span data-ttu-id="365d4-158">Int32</span><span class="sxs-lookup"><span data-stu-id="365d4-158">Int32</span></span>|<span data-ttu-id="365d4-159">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-159">Not yet documented</span></span>|
|<span data-ttu-id="365d4-160">transformedProfileBody</span><span class="sxs-lookup"><span data-stu-id="365d4-160">transformedProfileBody</span></span>|<span data-ttu-id="365d4-161">String</span><span class="sxs-lookup"><span data-stu-id="365d4-161">String</span></span>|<span data-ttu-id="365d4-162">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-162">Not yet documented</span></span>|
|<span data-ttu-id="365d4-163">transformedProfileBodyHash</span><span class="sxs-lookup"><span data-stu-id="365d4-163">transformedProfileBodyHash</span></span>|<span data-ttu-id="365d4-164">String</span><span class="sxs-lookup"><span data-stu-id="365d4-164">String</span></span>|<span data-ttu-id="365d4-165">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-165">Not yet documented</span></span>|
|<span data-ttu-id="365d4-166">tenantId</span><span class="sxs-lookup"><span data-stu-id="365d4-166">tenantId</span></span>|<span data-ttu-id="365d4-167">Guid</span><span class="sxs-lookup"><span data-stu-id="365d4-167">Guid</span></span>|<span data-ttu-id="365d4-168">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-168">Not yet documented</span></span>|
|<span data-ttu-id="365d4-169">profileId</span><span class="sxs-lookup"><span data-stu-id="365d4-169">profileId</span></span>|<span data-ttu-id="365d4-170">Guid</span><span class="sxs-lookup"><span data-stu-id="365d4-170">Guid</span></span>|<span data-ttu-id="365d4-171">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-171">Not yet documented</span></span>|
|<span data-ttu-id="365d4-172">eTag</span><span class="sxs-lookup"><span data-stu-id="365d4-172">eTag</span></span>|<span data-ttu-id="365d4-173">String</span><span class="sxs-lookup"><span data-stu-id="365d4-173">String</span></span>|<span data-ttu-id="365d4-174">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-174">Not yet documented</span></span>|
|<span data-ttu-id="365d4-175">schemaVersion</span><span class="sxs-lookup"><span data-stu-id="365d4-175">schemaVersion</span></span>|[<span data-ttu-id="365d4-176">raPolicyServiceVersions</span><span class="sxs-lookup"><span data-stu-id="365d4-176">raPolicyServiceVersions</span></span>](../resources/intune-rapolicy-rapolicyserviceversions.md)|<span data-ttu-id="365d4-177">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="365d4-177">Not yet documented.</span></span> <span data-ttu-id="365d4-178">可取值为：`initial`、`betaStart`、`experimentStart`、`mmpcStart`、`iosStart`。</span><span class="sxs-lookup"><span data-stu-id="365d4-178">Possible values are: `initial`, `betaStart`, `experimentStart`, `mmpcStart`, `iosStart`.</span></span>|
|<span data-ttu-id="365d4-179">lastModified</span><span class="sxs-lookup"><span data-stu-id="365d4-179">lastModified</span></span>|<span data-ttu-id="365d4-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="365d4-180">DateTimeOffset</span></span>|<span data-ttu-id="365d4-181">尚未记录</span><span class="sxs-lookup"><span data-stu-id="365d4-181">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="365d4-182">响应</span><span class="sxs-lookup"><span data-stu-id="365d4-182">Response</span></span>
<span data-ttu-id="365d4-183">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="365d4-183">If successful, this method returns a `201 Created` response code and a [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="365d4-184">示例</span><span class="sxs-lookup"><span data-stu-id="365d4-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="365d4-185">请求</span><span class="sxs-lookup"><span data-stu-id="365d4-185">Request</span></span>
<span data-ttu-id="365d4-186">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="365d4-186">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/resourceAccessProfileEntities
Content-type: application/json
Content-length: 799

{
  "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
  "version": 7,
  "isDeleted": true,
  "softDeletedTime": "2016-12-31T23:59:22.6041454-08:00",
  "displayName": "Display Name value",
  "linkedProfileIds": [
    "5b59ac1a-ac1a-5b59-1aac-595b1aac595b"
  ],
  "profileTypeName": "Profile Type Name value",
  "profileBody": "Profile Body value",
  "profileBodyHash": "Profile Body Hash value",
  "platformType": 12,
  "transformedProfileBody": "Transformed Profile Body value",
  "transformedProfileBodyHash": "Transformed Profile Body Hash value",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "profileId": "6389d896-d896-6389-96d8-896396d88963",
  "eTag": "ETag value",
  "schemaVersion": "betaStart",
  "lastModified": "2017-01-01T00:03:14.6651031-08:00"
}
```

### <a name="response"></a><span data-ttu-id="365d4-187">响应</span><span class="sxs-lookup"><span data-stu-id="365d4-187">Response</span></span>
<span data-ttu-id="365d4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="365d4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 799

{
  "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
  "version": 7,
  "isDeleted": true,
  "softDeletedTime": "2016-12-31T23:59:22.6041454-08:00",
  "displayName": "Display Name value",
  "linkedProfileIds": [
    "5b59ac1a-ac1a-5b59-1aac-595b1aac595b"
  ],
  "profileTypeName": "Profile Type Name value",
  "profileBody": "Profile Body value",
  "profileBodyHash": "Profile Body Hash value",
  "platformType": 12,
  "transformedProfileBody": "Transformed Profile Body value",
  "transformedProfileBodyHash": "Transformed Profile Body Hash value",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "profileId": "6389d896-d896-6389-96d8-896396d88963",
  "eTag": "ETag value",
  "schemaVersion": "betaStart",
  "lastModified": "2017-01-01T00:03:14.6651031-08:00"
}
```



