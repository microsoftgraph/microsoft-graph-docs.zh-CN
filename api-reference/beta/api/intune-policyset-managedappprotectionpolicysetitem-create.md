---
title: 创建 managedAppProtectionPolicySetItem
description: 创建新的 managedAppProtectionPolicySetItem 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c509323ecc26ea1cd08d358ac64c7d6c0ad4b176
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093446"
---
# <a name="create-managedappprotectionpolicysetitem"></a><span data-ttu-id="b191f-103">创建 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="b191f-103">Create managedAppProtectionPolicySetItem</span></span>

<span data-ttu-id="b191f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b191f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b191f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b191f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b191f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b191f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b191f-107">创建新的 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b191f-107">Create a new [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b191f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b191f-108">Prerequisites</span></span>
<span data-ttu-id="b191f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b191f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b191f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b191f-111">Permission type</span></span>|<span data-ttu-id="b191f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b191f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b191f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b191f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b191f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b191f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b191f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b191f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b191f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b191f-116">Not supported.</span></span>|
|<span data-ttu-id="b191f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b191f-117">Application</span></span>|<span data-ttu-id="b191f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b191f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b191f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b191f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="b191f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b191f-120">Request headers</span></span>
|<span data-ttu-id="b191f-121">标头</span><span class="sxs-lookup"><span data-stu-id="b191f-121">Header</span></span>|<span data-ttu-id="b191f-122">值</span><span class="sxs-lookup"><span data-stu-id="b191f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b191f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b191f-123">Authorization</span></span>|<span data-ttu-id="b191f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b191f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b191f-125">接受</span><span class="sxs-lookup"><span data-stu-id="b191f-125">Accept</span></span>|<span data-ttu-id="b191f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b191f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b191f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b191f-127">Request body</span></span>
<span data-ttu-id="b191f-128">在请求正文中，提供 managedAppProtectionPolicySetItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b191f-128">In the request body, supply a JSON representation for the managedAppProtectionPolicySetItem object.</span></span>

<span data-ttu-id="b191f-129">下表显示创建 managedAppProtectionPolicySetItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b191f-129">The following table shows the properties that are required when you create the managedAppProtectionPolicySetItem.</span></span>

|<span data-ttu-id="b191f-130">属性</span><span class="sxs-lookup"><span data-stu-id="b191f-130">Property</span></span>|<span data-ttu-id="b191f-131">类型</span><span class="sxs-lookup"><span data-stu-id="b191f-131">Type</span></span>|<span data-ttu-id="b191f-132">说明</span><span class="sxs-lookup"><span data-stu-id="b191f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b191f-133">id</span><span class="sxs-lookup"><span data-stu-id="b191f-133">id</span></span>|<span data-ttu-id="b191f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b191f-134">String</span></span>|<span data-ttu-id="b191f-135">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="b191f-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="b191f-136">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b191f-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b191f-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b191f-137">createdDateTime</span></span>|<span data-ttu-id="b191f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b191f-138">DateTimeOffset</span></span>|<span data-ttu-id="b191f-139">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="b191f-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="b191f-140">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b191f-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b191f-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b191f-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b191f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b191f-142">DateTimeOffset</span></span>|<span data-ttu-id="b191f-143">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="b191f-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="b191f-144">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b191f-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b191f-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="b191f-145">payloadId</span></span>|<span data-ttu-id="b191f-146">字符串</span><span class="sxs-lookup"><span data-stu-id="b191f-146">String</span></span>|<span data-ttu-id="b191f-147">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="b191f-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="b191f-148">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b191f-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b191f-149">itemType</span><span class="sxs-lookup"><span data-stu-id="b191f-149">itemType</span></span>|<span data-ttu-id="b191f-150">字符串</span><span class="sxs-lookup"><span data-stu-id="b191f-150">String</span></span>|<span data-ttu-id="b191f-151">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="b191f-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="b191f-152">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b191f-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b191f-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b191f-153">displayName</span></span>|<span data-ttu-id="b191f-154">字符串</span><span class="sxs-lookup"><span data-stu-id="b191f-154">String</span></span>|<span data-ttu-id="b191f-155">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="b191f-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="b191f-156">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b191f-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b191f-157">状态</span><span class="sxs-lookup"><span data-stu-id="b191f-157">status</span></span>|[<span data-ttu-id="b191f-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="b191f-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="b191f-159">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="b191f-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="b191f-160">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b191f-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="b191f-161">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="b191f-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="b191f-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="b191f-162">errorCode</span></span>|[<span data-ttu-id="b191f-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="b191f-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="b191f-164">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="b191f-164">Error code if any occured.</span></span> <span data-ttu-id="b191f-165">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b191f-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="b191f-166">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="b191f-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="b191f-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="b191f-167">guidedDeploymentTags</span></span>|<span data-ttu-id="b191f-168">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b191f-168">String collection</span></span>|<span data-ttu-id="b191f-169">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="b191f-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b191f-170">targetedAppManagementLevels</span><span class="sxs-lookup"><span data-stu-id="b191f-170">targetedAppManagementLevels</span></span>|<span data-ttu-id="b191f-171">字符串</span><span class="sxs-lookup"><span data-stu-id="b191f-171">String</span></span>|<span data-ttu-id="b191f-172">ManagedAppPolicySetItem 的 TargetedAppManagementLevels。</span><span class="sxs-lookup"><span data-stu-id="b191f-172">TargetedAppManagementLevels of the ManagedAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="b191f-173">响应</span><span class="sxs-lookup"><span data-stu-id="b191f-173">Response</span></span>
<span data-ttu-id="b191f-174">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b191f-174">If successful, this method returns a `201 Created` response code and a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b191f-175">示例</span><span class="sxs-lookup"><span data-stu-id="b191f-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="b191f-176">请求</span><span class="sxs-lookup"><span data-stu-id="b191f-176">Request</span></span>
<span data-ttu-id="b191f-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b191f-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
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

### <a name="response"></a><span data-ttu-id="b191f-178">响应</span><span class="sxs-lookup"><span data-stu-id="b191f-178">Response</span></span>
<span data-ttu-id="b191f-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b191f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






