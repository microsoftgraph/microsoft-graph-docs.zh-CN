---
title: 更新 mobileAppPolicySetItem
description: 更新 mobileAppPolicySetItem 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cfd672f816699d7f608828418878470112916cc9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159295"
---
# <a name="update-mobileapppolicysetitem"></a><span data-ttu-id="1a6a6-103">更新 mobileAppPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="1a6a6-103">Update mobileAppPolicySetItem</span></span>

<span data-ttu-id="1a6a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a6a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a6a6-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a6a6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a6a6-107">更新 [mobileAppPolicySetItem 对象](../resources/intune-policyset-mobileapppolicysetitem.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-107">Update the properties of a [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a6a6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a6a6-108">Prerequisites</span></span>
<span data-ttu-id="1a6a6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a6a6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a6a6-111">Permission type</span></span>|<span data-ttu-id="1a6a6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1a6a6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a6a6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a6a6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a6a6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a6a6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a6a6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a6a6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a6a6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-116">Not supported.</span></span>|
|<span data-ttu-id="1a6a6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a6a6-117">Application</span></span>|<span data-ttu-id="1a6a6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a6a6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a6a6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a6a6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="1a6a6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a6a6-120">Request headers</span></span>
|<span data-ttu-id="1a6a6-121">标头</span><span class="sxs-lookup"><span data-stu-id="1a6a6-121">Header</span></span>|<span data-ttu-id="1a6a6-122">值</span><span class="sxs-lookup"><span data-stu-id="1a6a6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a6a6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a6a6-123">Authorization</span></span>|<span data-ttu-id="1a6a6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a6a6-125">接受</span><span class="sxs-lookup"><span data-stu-id="1a6a6-125">Accept</span></span>|<span data-ttu-id="1a6a6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a6a6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a6a6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a6a6-127">Request body</span></span>
<span data-ttu-id="1a6a6-128">在请求正文中，提供 [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-128">In the request body, supply a JSON representation for the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

<span data-ttu-id="1a6a6-129">下表显示创建 [mobileAppPolicySetItem 时所需的属性](../resources/intune-policyset-mobileapppolicysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-129">The following table shows the properties that are required when you create the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md).</span></span>

|<span data-ttu-id="1a6a6-130">属性</span><span class="sxs-lookup"><span data-stu-id="1a6a6-130">Property</span></span>|<span data-ttu-id="1a6a6-131">类型</span><span class="sxs-lookup"><span data-stu-id="1a6a6-131">Type</span></span>|<span data-ttu-id="1a6a6-132">说明</span><span class="sxs-lookup"><span data-stu-id="1a6a6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a6a6-133">id</span><span class="sxs-lookup"><span data-stu-id="1a6a6-133">id</span></span>|<span data-ttu-id="1a6a6-134">String</span><span class="sxs-lookup"><span data-stu-id="1a6a6-134">String</span></span>|<span data-ttu-id="1a6a6-135">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="1a6a6-136">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1a6a6-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1a6a6-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a6a6-137">createdDateTime</span></span>|<span data-ttu-id="1a6a6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a6a6-138">DateTimeOffset</span></span>|<span data-ttu-id="1a6a6-139">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="1a6a6-140">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1a6a6-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1a6a6-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a6a6-141">lastModifiedDateTime</span></span>|<span data-ttu-id="1a6a6-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a6a6-142">DateTimeOffset</span></span>|<span data-ttu-id="1a6a6-143">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="1a6a6-144">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1a6a6-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1a6a6-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="1a6a6-145">payloadId</span></span>|<span data-ttu-id="1a6a6-146">String</span><span class="sxs-lookup"><span data-stu-id="1a6a6-146">String</span></span>|<span data-ttu-id="1a6a6-147">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="1a6a6-148">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1a6a6-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1a6a6-149">itemType</span><span class="sxs-lookup"><span data-stu-id="1a6a6-149">itemType</span></span>|<span data-ttu-id="1a6a6-150">String</span><span class="sxs-lookup"><span data-stu-id="1a6a6-150">String</span></span>|<span data-ttu-id="1a6a6-151">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="1a6a6-152">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1a6a6-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1a6a6-153">displayName</span><span class="sxs-lookup"><span data-stu-id="1a6a6-153">displayName</span></span>|<span data-ttu-id="1a6a6-154">String</span><span class="sxs-lookup"><span data-stu-id="1a6a6-154">String</span></span>|<span data-ttu-id="1a6a6-155">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="1a6a6-156">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1a6a6-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1a6a6-157">status</span><span class="sxs-lookup"><span data-stu-id="1a6a6-157">status</span></span>|[<span data-ttu-id="1a6a6-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="1a6a6-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="1a6a6-159">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="1a6a6-160">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="1a6a6-161">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="1a6a6-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="1a6a6-162">errorCode</span></span>|[<span data-ttu-id="1a6a6-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="1a6a6-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="1a6a6-164">错误代码（如果有）。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-164">Error code if any occured.</span></span> <span data-ttu-id="1a6a6-165">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="1a6a6-166">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="1a6a6-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="1a6a6-167">guidedDeploymentTags</span></span>|<span data-ttu-id="1a6a6-168">字符串集合</span><span class="sxs-lookup"><span data-stu-id="1a6a6-168">String collection</span></span>|<span data-ttu-id="1a6a6-169">引导式部署的标记 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1a6a6-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1a6a6-170">intent</span><span class="sxs-lookup"><span data-stu-id="1a6a6-170">intent</span></span>|[<span data-ttu-id="1a6a6-171">installIntent</span><span class="sxs-lookup"><span data-stu-id="1a6a6-171">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="1a6a6-172">MobileAppPolicySetItem 的安装意图。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-172">Install intent of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="1a6a6-173">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-173">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="1a6a6-174">settings</span><span class="sxs-lookup"><span data-stu-id="1a6a6-174">settings</span></span>|[<span data-ttu-id="1a6a6-175">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1a6a6-175">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="1a6a6-176">MobileAppPolicySetItem 的设置。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-176">Settings of the MobileAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="1a6a6-177">响应</span><span class="sxs-lookup"><span data-stu-id="1a6a6-177">Response</span></span>
<span data-ttu-id="1a6a6-178">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-178">If successful, this method returns a `200 OK` response code and an updated [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a6a6-179">示例</span><span class="sxs-lookup"><span data-stu-id="1a6a6-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a6a6-180">请求</span><span class="sxs-lookup"><span data-stu-id="1a6a6-180">Request</span></span>
<span data-ttu-id="1a6a6-181">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 540

{
  "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "intent": "required",
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value",
    "uninstallOnDeviceRemoval": true,
    "isRemovable": true
  }
}
```

### <a name="response"></a><span data-ttu-id="1a6a6-182">响应</span><span class="sxs-lookup"><span data-stu-id="1a6a6-182">Response</span></span>
<span data-ttu-id="1a6a6-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a6a6-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
  "id": "b6ffe6cf-e6cf-b6ff-cfe6-ffb6cfe6ffb6",
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
  "intent": "required",
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value",
    "uninstallOnDeviceRemoval": true,
    "isRemovable": true
  }
}
```




