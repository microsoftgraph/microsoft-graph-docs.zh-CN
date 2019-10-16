---
title: 更新 managedDeviceMobileAppConfigurationPolicySetItem
description: 更新 managedDeviceMobileAppConfigurationPolicySetItem 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d6cb52ca7471867e3f6f528dce02c12239f5c7b2
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536376"
---
# <a name="update-manageddevicemobileappconfigurationpolicysetitem"></a><span data-ttu-id="f4682-103">更新 managedDeviceMobileAppConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="f4682-103">Update managedDeviceMobileAppConfigurationPolicySetItem</span></span>

> <span data-ttu-id="f4682-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4682-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4682-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4682-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4682-106">更新[managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f4682-106">Update the properties of a [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4682-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4682-107">Prerequisites</span></span>
<span data-ttu-id="f4682-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4682-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4682-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4682-110">Permission type</span></span>|<span data-ttu-id="f4682-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4682-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4682-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4682-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4682-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4682-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4682-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4682-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4682-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4682-115">Not supported.</span></span>|
|<span data-ttu-id="f4682-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4682-116">Application</span></span>|<span data-ttu-id="f4682-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4682-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4682-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4682-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="f4682-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4682-119">Request headers</span></span>
|<span data-ttu-id="f4682-120">标头</span><span class="sxs-lookup"><span data-stu-id="f4682-120">Header</span></span>|<span data-ttu-id="f4682-121">值</span><span class="sxs-lookup"><span data-stu-id="f4682-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4682-122">授权</span><span class="sxs-lookup"><span data-stu-id="f4682-122">Authorization</span></span>|<span data-ttu-id="f4682-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4682-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4682-124">接受</span><span class="sxs-lookup"><span data-stu-id="f4682-124">Accept</span></span>|<span data-ttu-id="f4682-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4682-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4682-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4682-126">Request body</span></span>
<span data-ttu-id="f4682-127">在请求正文中，提供[managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4682-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object.</span></span>

<span data-ttu-id="f4682-128">下表显示创建[managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f4682-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md).</span></span>

|<span data-ttu-id="f4682-129">属性</span><span class="sxs-lookup"><span data-stu-id="f4682-129">Property</span></span>|<span data-ttu-id="f4682-130">类型</span><span class="sxs-lookup"><span data-stu-id="f4682-130">Type</span></span>|<span data-ttu-id="f4682-131">说明</span><span class="sxs-lookup"><span data-stu-id="f4682-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4682-132">id</span><span class="sxs-lookup"><span data-stu-id="f4682-132">id</span></span>|<span data-ttu-id="f4682-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f4682-133">String</span></span>|<span data-ttu-id="f4682-134">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="f4682-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="f4682-135">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f4682-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f4682-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4682-136">createdDateTime</span></span>|<span data-ttu-id="f4682-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4682-137">DateTimeOffset</span></span>|<span data-ttu-id="f4682-138">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="f4682-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="f4682-139">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f4682-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f4682-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4682-140">lastModifiedDateTime</span></span>|<span data-ttu-id="f4682-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4682-141">DateTimeOffset</span></span>|<span data-ttu-id="f4682-142">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="f4682-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="f4682-143">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f4682-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f4682-144">payloadId</span><span class="sxs-lookup"><span data-stu-id="f4682-144">payloadId</span></span>|<span data-ttu-id="f4682-145">字符串</span><span class="sxs-lookup"><span data-stu-id="f4682-145">String</span></span>|<span data-ttu-id="f4682-146">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="f4682-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="f4682-147">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f4682-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f4682-148">itemType</span><span class="sxs-lookup"><span data-stu-id="f4682-148">itemType</span></span>|<span data-ttu-id="f4682-149">字符串</span><span class="sxs-lookup"><span data-stu-id="f4682-149">String</span></span>|<span data-ttu-id="f4682-150">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="f4682-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="f4682-151">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f4682-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f4682-152">displayName</span><span class="sxs-lookup"><span data-stu-id="f4682-152">displayName</span></span>|<span data-ttu-id="f4682-153">String</span><span class="sxs-lookup"><span data-stu-id="f4682-153">String</span></span>|<span data-ttu-id="f4682-154">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="f4682-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="f4682-155">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f4682-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f4682-156">status</span><span class="sxs-lookup"><span data-stu-id="f4682-156">status</span></span>|[<span data-ttu-id="f4682-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="f4682-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="f4682-158">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="f4682-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="f4682-159">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="f4682-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="f4682-160">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="f4682-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="f4682-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="f4682-161">errorCode</span></span>|[<span data-ttu-id="f4682-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="f4682-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="f4682-163">错误代码（如果发生）。</span><span class="sxs-lookup"><span data-stu-id="f4682-163">Error code if any occured.</span></span> <span data-ttu-id="f4682-164">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="f4682-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="f4682-165">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="f4682-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="f4682-166">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="f4682-166">guidedDeploymentTags</span></span>|<span data-ttu-id="f4682-167">String 集合</span><span class="sxs-lookup"><span data-stu-id="f4682-167">String collection</span></span>|<span data-ttu-id="f4682-168">继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记</span><span class="sxs-lookup"><span data-stu-id="f4682-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f4682-169">响应</span><span class="sxs-lookup"><span data-stu-id="f4682-169">Response</span></span>
<span data-ttu-id="f4682-170">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f4682-170">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4682-171">示例</span><span class="sxs-lookup"><span data-stu-id="f4682-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4682-172">请求</span><span class="sxs-lookup"><span data-stu-id="f4682-172">Request</span></span>
<span data-ttu-id="f4682-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4682-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 330

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="f4682-174">响应</span><span class="sxs-lookup"><span data-stu-id="f4682-174">Response</span></span>
<span data-ttu-id="f4682-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4682-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationPolicySetItem",
  "id": "bb065442-5442-bb06-4254-06bb425406bb",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ]
}
```






