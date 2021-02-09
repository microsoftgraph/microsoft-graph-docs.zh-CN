---
title: 创建 mobileAppPolicySetItem
description: 创建新的 mobileAppPolicySetItem 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2db884dfec7bf2460b80c30f3fc96155f22e1111
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159316"
---
# <a name="create-mobileapppolicysetitem"></a><span data-ttu-id="3d8cd-103">创建 mobileAppPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="3d8cd-103">Create mobileAppPolicySetItem</span></span>

<span data-ttu-id="3d8cd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d8cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d8cd-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d8cd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d8cd-107">创建新的 [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-107">Create a new [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d8cd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d8cd-108">Prerequisites</span></span>
<span data-ttu-id="3d8cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d8cd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d8cd-111">Permission type</span></span>|<span data-ttu-id="3d8cd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3d8cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d8cd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d8cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d8cd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d8cd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3d8cd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d8cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d8cd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-116">Not supported.</span></span>|
|<span data-ttu-id="3d8cd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d8cd-117">Application</span></span>|<span data-ttu-id="3d8cd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d8cd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d8cd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d8cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="3d8cd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d8cd-120">Request headers</span></span>
|<span data-ttu-id="3d8cd-121">标头</span><span class="sxs-lookup"><span data-stu-id="3d8cd-121">Header</span></span>|<span data-ttu-id="3d8cd-122">值</span><span class="sxs-lookup"><span data-stu-id="3d8cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d8cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d8cd-123">Authorization</span></span>|<span data-ttu-id="3d8cd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d8cd-125">接受</span><span class="sxs-lookup"><span data-stu-id="3d8cd-125">Accept</span></span>|<span data-ttu-id="3d8cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d8cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d8cd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d8cd-127">Request body</span></span>
<span data-ttu-id="3d8cd-128">在请求正文中，提供 mobileAppPolicySetItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-128">In the request body, supply a JSON representation for the mobileAppPolicySetItem object.</span></span>

<span data-ttu-id="3d8cd-129">下表显示创建 mobileAppPolicySetItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-129">The following table shows the properties that are required when you create the mobileAppPolicySetItem.</span></span>

|<span data-ttu-id="3d8cd-130">属性</span><span class="sxs-lookup"><span data-stu-id="3d8cd-130">Property</span></span>|<span data-ttu-id="3d8cd-131">类型</span><span class="sxs-lookup"><span data-stu-id="3d8cd-131">Type</span></span>|<span data-ttu-id="3d8cd-132">说明</span><span class="sxs-lookup"><span data-stu-id="3d8cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d8cd-133">id</span><span class="sxs-lookup"><span data-stu-id="3d8cd-133">id</span></span>|<span data-ttu-id="3d8cd-134">String</span><span class="sxs-lookup"><span data-stu-id="3d8cd-134">String</span></span>|<span data-ttu-id="3d8cd-135">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="3d8cd-136">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3d8cd-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3d8cd-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d8cd-137">createdDateTime</span></span>|<span data-ttu-id="3d8cd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d8cd-138">DateTimeOffset</span></span>|<span data-ttu-id="3d8cd-139">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="3d8cd-140">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3d8cd-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3d8cd-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d8cd-141">lastModifiedDateTime</span></span>|<span data-ttu-id="3d8cd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d8cd-142">DateTimeOffset</span></span>|<span data-ttu-id="3d8cd-143">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="3d8cd-144">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3d8cd-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3d8cd-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="3d8cd-145">payloadId</span></span>|<span data-ttu-id="3d8cd-146">String</span><span class="sxs-lookup"><span data-stu-id="3d8cd-146">String</span></span>|<span data-ttu-id="3d8cd-147">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="3d8cd-148">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3d8cd-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3d8cd-149">itemType</span><span class="sxs-lookup"><span data-stu-id="3d8cd-149">itemType</span></span>|<span data-ttu-id="3d8cd-150">String</span><span class="sxs-lookup"><span data-stu-id="3d8cd-150">String</span></span>|<span data-ttu-id="3d8cd-151">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="3d8cd-152">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3d8cd-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3d8cd-153">displayName</span><span class="sxs-lookup"><span data-stu-id="3d8cd-153">displayName</span></span>|<span data-ttu-id="3d8cd-154">String</span><span class="sxs-lookup"><span data-stu-id="3d8cd-154">String</span></span>|<span data-ttu-id="3d8cd-155">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="3d8cd-156">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3d8cd-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3d8cd-157">status</span><span class="sxs-lookup"><span data-stu-id="3d8cd-157">status</span></span>|[<span data-ttu-id="3d8cd-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="3d8cd-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="3d8cd-159">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="3d8cd-160">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="3d8cd-161">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="3d8cd-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="3d8cd-162">errorCode</span></span>|[<span data-ttu-id="3d8cd-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="3d8cd-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="3d8cd-164">错误代码（如果有）。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-164">Error code if any occured.</span></span> <span data-ttu-id="3d8cd-165">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="3d8cd-166">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="3d8cd-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="3d8cd-167">guidedDeploymentTags</span></span>|<span data-ttu-id="3d8cd-168">字符串集合</span><span class="sxs-lookup"><span data-stu-id="3d8cd-168">String collection</span></span>|<span data-ttu-id="3d8cd-169">引导式部署的标记 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="3d8cd-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="3d8cd-170">intent</span><span class="sxs-lookup"><span data-stu-id="3d8cd-170">intent</span></span>|[<span data-ttu-id="3d8cd-171">installIntent</span><span class="sxs-lookup"><span data-stu-id="3d8cd-171">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="3d8cd-172">MobileAppPolicySetItem 的安装意图。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-172">Install intent of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="3d8cd-173">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-173">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="3d8cd-174">settings</span><span class="sxs-lookup"><span data-stu-id="3d8cd-174">settings</span></span>|[<span data-ttu-id="3d8cd-175">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="3d8cd-175">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="3d8cd-176">MobileAppPolicySetItem 的设置。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-176">Settings of the MobileAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="3d8cd-177">响应</span><span class="sxs-lookup"><span data-stu-id="3d8cd-177">Response</span></span>
<span data-ttu-id="3d8cd-178">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-178">If successful, this method returns a `201 Created` response code and a [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d8cd-179">示例</span><span class="sxs-lookup"><span data-stu-id="3d8cd-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d8cd-180">请求</span><span class="sxs-lookup"><span data-stu-id="3d8cd-180">Request</span></span>
<span data-ttu-id="3d8cd-181">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
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

### <a name="response"></a><span data-ttu-id="3d8cd-182">响应</span><span class="sxs-lookup"><span data-stu-id="3d8cd-182">Response</span></span>
<span data-ttu-id="3d8cd-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d8cd-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




