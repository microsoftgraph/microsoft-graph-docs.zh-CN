---
title: 更新 managedAppProtectionPolicySetItem
description: 更新 managedAppProtectionPolicySetItem 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 30e6f7be1215a3a6d06c092cf7f5c216df3ebfd8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802256"
---
# <a name="update-managedappprotectionpolicysetitem"></a><span data-ttu-id="e5cdb-103">更新 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="e5cdb-103">Update managedAppProtectionPolicySetItem</span></span>

> <span data-ttu-id="e5cdb-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5cdb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5cdb-106">更新[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-106">Update the properties of a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5cdb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e5cdb-107">Prerequisites</span></span>
<span data-ttu-id="e5cdb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5cdb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5cdb-110">Permission type</span></span>|<span data-ttu-id="e5cdb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e5cdb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5cdb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5cdb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5cdb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5cdb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5cdb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5cdb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5cdb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-115">Not supported.</span></span>|
|<span data-ttu-id="e5cdb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5cdb-116">Application</span></span>|<span data-ttu-id="e5cdb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5cdb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5cdb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5cdb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="e5cdb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5cdb-119">Request headers</span></span>
|<span data-ttu-id="e5cdb-120">标头</span><span class="sxs-lookup"><span data-stu-id="e5cdb-120">Header</span></span>|<span data-ttu-id="e5cdb-121">值</span><span class="sxs-lookup"><span data-stu-id="e5cdb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5cdb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5cdb-122">Authorization</span></span>|<span data-ttu-id="e5cdb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5cdb-124">接受</span><span class="sxs-lookup"><span data-stu-id="e5cdb-124">Accept</span></span>|<span data-ttu-id="e5cdb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5cdb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5cdb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5cdb-126">Request body</span></span>
<span data-ttu-id="e5cdb-127">在请求正文中，提供[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-127">In the request body, supply a JSON representation for the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

<span data-ttu-id="e5cdb-128">下表显示创建[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-128">The following table shows the properties that are required when you create the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md).</span></span>

|<span data-ttu-id="e5cdb-129">属性</span><span class="sxs-lookup"><span data-stu-id="e5cdb-129">Property</span></span>|<span data-ttu-id="e5cdb-130">类型</span><span class="sxs-lookup"><span data-stu-id="e5cdb-130">Type</span></span>|<span data-ttu-id="e5cdb-131">说明</span><span class="sxs-lookup"><span data-stu-id="e5cdb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5cdb-132">id</span><span class="sxs-lookup"><span data-stu-id="e5cdb-132">id</span></span>|<span data-ttu-id="e5cdb-133">String</span><span class="sxs-lookup"><span data-stu-id="e5cdb-133">String</span></span>|<span data-ttu-id="e5cdb-134">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="e5cdb-135">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="e5cdb-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="e5cdb-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5cdb-136">createdDateTime</span></span>|<span data-ttu-id="e5cdb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5cdb-137">DateTimeOffset</span></span>|<span data-ttu-id="e5cdb-138">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="e5cdb-139">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="e5cdb-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="e5cdb-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5cdb-140">lastModifiedDateTime</span></span>|<span data-ttu-id="e5cdb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5cdb-141">DateTimeOffset</span></span>|<span data-ttu-id="e5cdb-142">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="e5cdb-143">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="e5cdb-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="e5cdb-144">payloadId</span><span class="sxs-lookup"><span data-stu-id="e5cdb-144">payloadId</span></span>|<span data-ttu-id="e5cdb-145">String</span><span class="sxs-lookup"><span data-stu-id="e5cdb-145">String</span></span>|<span data-ttu-id="e5cdb-146">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="e5cdb-147">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="e5cdb-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="e5cdb-148">itemType</span><span class="sxs-lookup"><span data-stu-id="e5cdb-148">itemType</span></span>|<span data-ttu-id="e5cdb-149">String</span><span class="sxs-lookup"><span data-stu-id="e5cdb-149">String</span></span>|<span data-ttu-id="e5cdb-150">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="e5cdb-151">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="e5cdb-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="e5cdb-152">displayName</span><span class="sxs-lookup"><span data-stu-id="e5cdb-152">displayName</span></span>|<span data-ttu-id="e5cdb-153">String</span><span class="sxs-lookup"><span data-stu-id="e5cdb-153">String</span></span>|<span data-ttu-id="e5cdb-154">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="e5cdb-155">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="e5cdb-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="e5cdb-156">状态</span><span class="sxs-lookup"><span data-stu-id="e5cdb-156">status</span></span>|[<span data-ttu-id="e5cdb-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="e5cdb-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="e5cdb-158">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="e5cdb-159">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="e5cdb-160">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="e5cdb-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="e5cdb-161">errorCode</span></span>|[<span data-ttu-id="e5cdb-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="e5cdb-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="e5cdb-163">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-163">Error code if any occured.</span></span> <span data-ttu-id="e5cdb-164">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="e5cdb-165">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="e5cdb-166">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="e5cdb-166">guidedDeploymentTags</span></span>|<span data-ttu-id="e5cdb-167">String collection</span><span class="sxs-lookup"><span data-stu-id="e5cdb-167">String collection</span></span>|<span data-ttu-id="e5cdb-168">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="e5cdb-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="e5cdb-169">targetedAppManagementLevels</span><span class="sxs-lookup"><span data-stu-id="e5cdb-169">targetedAppManagementLevels</span></span>|<span data-ttu-id="e5cdb-170">String</span><span class="sxs-lookup"><span data-stu-id="e5cdb-170">String</span></span>|<span data-ttu-id="e5cdb-171">ManagedAppPolicySetItem 的 TargetedAppManagementLevels。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-171">TargetedAppManagementLevels of the ManagedAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="e5cdb-172">响应</span><span class="sxs-lookup"><span data-stu-id="e5cdb-172">Response</span></span>
<span data-ttu-id="e5cdb-173">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-173">If successful, this method returns a `200 OK` response code and an updated [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5cdb-174">示例</span><span class="sxs-lookup"><span data-stu-id="e5cdb-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5cdb-175">请求</span><span class="sxs-lookup"><span data-stu-id="e5cdb-175">Request</span></span>
<span data-ttu-id="e5cdb-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 389

{
  "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "targetedAppManagementLevels": "Targeted App Management Levels value"
}
```

### <a name="response"></a><span data-ttu-id="e5cdb-177">响应</span><span class="sxs-lookup"><span data-stu-id="e5cdb-177">Response</span></span>
<span data-ttu-id="e5cdb-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e5cdb-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 561

{
  "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
  "id": "e10d79c9-79c9-e10d-c979-0de1c9790de1",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "targetedAppManagementLevels": "Targeted App Management Levels value"
}
```




