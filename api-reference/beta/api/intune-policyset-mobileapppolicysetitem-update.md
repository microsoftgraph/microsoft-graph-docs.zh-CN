---
title: 更新 mobileAppPolicySetItem
description: 更新 mobileAppPolicySetItem 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fd98514fcc16dbc413725cb8d597c7d8cc50ae1d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134646"
---
# <a name="update-mobileapppolicysetitem"></a><span data-ttu-id="b1aac-103">更新 mobileAppPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="b1aac-103">Update mobileAppPolicySetItem</span></span>

<span data-ttu-id="b1aac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1aac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1aac-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1aac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1aac-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1aac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1aac-107">更新 [mobileAppPolicySetItem 对象](../resources/intune-policyset-mobileapppolicysetitem.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="b1aac-107">Update the properties of a [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1aac-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b1aac-108">Prerequisites</span></span>
<span data-ttu-id="b1aac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1aac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1aac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1aac-111">Permission type</span></span>|<span data-ttu-id="b1aac-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b1aac-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1aac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1aac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1aac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1aac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1aac-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1aac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1aac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1aac-116">Not supported.</span></span>|
|<span data-ttu-id="b1aac-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1aac-117">Application</span></span>|<span data-ttu-id="b1aac-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1aac-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1aac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1aac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="b1aac-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1aac-120">Request headers</span></span>
|<span data-ttu-id="b1aac-121">标头</span><span class="sxs-lookup"><span data-stu-id="b1aac-121">Header</span></span>|<span data-ttu-id="b1aac-122">值</span><span class="sxs-lookup"><span data-stu-id="b1aac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1aac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1aac-123">Authorization</span></span>|<span data-ttu-id="b1aac-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b1aac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1aac-125">接受</span><span class="sxs-lookup"><span data-stu-id="b1aac-125">Accept</span></span>|<span data-ttu-id="b1aac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1aac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1aac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1aac-127">Request body</span></span>
<span data-ttu-id="b1aac-128">在请求正文中，提供 [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1aac-128">In the request body, supply a JSON representation for the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

<span data-ttu-id="b1aac-129">下表显示创建 [mobileAppPolicySetItem 时所需的属性](../resources/intune-policyset-mobileapppolicysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b1aac-129">The following table shows the properties that are required when you create the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md).</span></span>

|<span data-ttu-id="b1aac-130">属性</span><span class="sxs-lookup"><span data-stu-id="b1aac-130">Property</span></span>|<span data-ttu-id="b1aac-131">类型</span><span class="sxs-lookup"><span data-stu-id="b1aac-131">Type</span></span>|<span data-ttu-id="b1aac-132">说明</span><span class="sxs-lookup"><span data-stu-id="b1aac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1aac-133">id</span><span class="sxs-lookup"><span data-stu-id="b1aac-133">id</span></span>|<span data-ttu-id="b1aac-134">String</span><span class="sxs-lookup"><span data-stu-id="b1aac-134">String</span></span>|<span data-ttu-id="b1aac-135">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="b1aac-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="b1aac-136">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b1aac-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b1aac-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1aac-137">createdDateTime</span></span>|<span data-ttu-id="b1aac-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1aac-138">DateTimeOffset</span></span>|<span data-ttu-id="b1aac-139">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="b1aac-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="b1aac-140">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b1aac-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b1aac-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1aac-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b1aac-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1aac-142">DateTimeOffset</span></span>|<span data-ttu-id="b1aac-143">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="b1aac-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="b1aac-144">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b1aac-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b1aac-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="b1aac-145">payloadId</span></span>|<span data-ttu-id="b1aac-146">String</span><span class="sxs-lookup"><span data-stu-id="b1aac-146">String</span></span>|<span data-ttu-id="b1aac-147">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="b1aac-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="b1aac-148">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b1aac-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b1aac-149">itemType</span><span class="sxs-lookup"><span data-stu-id="b1aac-149">itemType</span></span>|<span data-ttu-id="b1aac-150">String</span><span class="sxs-lookup"><span data-stu-id="b1aac-150">String</span></span>|<span data-ttu-id="b1aac-151">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="b1aac-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="b1aac-152">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b1aac-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b1aac-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b1aac-153">displayName</span></span>|<span data-ttu-id="b1aac-154">String</span><span class="sxs-lookup"><span data-stu-id="b1aac-154">String</span></span>|<span data-ttu-id="b1aac-155">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="b1aac-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="b1aac-156">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b1aac-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b1aac-157">状态</span><span class="sxs-lookup"><span data-stu-id="b1aac-157">status</span></span>|[<span data-ttu-id="b1aac-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="b1aac-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="b1aac-159">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="b1aac-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="b1aac-160">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b1aac-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="b1aac-161">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="b1aac-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="b1aac-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="b1aac-162">errorCode</span></span>|[<span data-ttu-id="b1aac-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="b1aac-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="b1aac-164">错误代码（如果发生了任何错误）。</span><span class="sxs-lookup"><span data-stu-id="b1aac-164">Error code if any occured.</span></span> <span data-ttu-id="b1aac-165">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b1aac-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="b1aac-166">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="b1aac-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="b1aac-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="b1aac-167">guidedDeploymentTags</span></span>|<span data-ttu-id="b1aac-168">String collection</span><span class="sxs-lookup"><span data-stu-id="b1aac-168">String collection</span></span>|<span data-ttu-id="b1aac-169">引导式部署的标记 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b1aac-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b1aac-170">intent</span><span class="sxs-lookup"><span data-stu-id="b1aac-170">intent</span></span>|[<span data-ttu-id="b1aac-171">installIntent</span><span class="sxs-lookup"><span data-stu-id="b1aac-171">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="b1aac-172">MobileAppPolicySetItem 的安装意图。</span><span class="sxs-lookup"><span data-stu-id="b1aac-172">Install intent of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="b1aac-173">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="b1aac-173">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="b1aac-174">settings</span><span class="sxs-lookup"><span data-stu-id="b1aac-174">settings</span></span>|[<span data-ttu-id="b1aac-175">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="b1aac-175">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="b1aac-176">MobileAppPolicySetItem 的设置。</span><span class="sxs-lookup"><span data-stu-id="b1aac-176">Settings of the MobileAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="b1aac-177">响应</span><span class="sxs-lookup"><span data-stu-id="b1aac-177">Response</span></span>
<span data-ttu-id="b1aac-178">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1aac-178">If successful, this method returns a `200 OK` response code and an updated [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1aac-179">示例</span><span class="sxs-lookup"><span data-stu-id="b1aac-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1aac-180">请求</span><span class="sxs-lookup"><span data-stu-id="b1aac-180">Request</span></span>
<span data-ttu-id="b1aac-181">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1aac-181">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b1aac-182">响应</span><span class="sxs-lookup"><span data-stu-id="b1aac-182">Response</span></span>
<span data-ttu-id="b1aac-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1aac-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




