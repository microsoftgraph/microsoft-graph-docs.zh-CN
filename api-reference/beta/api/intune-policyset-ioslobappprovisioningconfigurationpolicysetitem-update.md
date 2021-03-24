---
title: 更新 iosLobAppProvisioningConfigurationPolicySetItem
description: 更新 iosLobAppProvisioningConfigurationPolicySetItem 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da31a610291d64666fa41c2265bc60952e4c6003
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141734"
---
# <a name="update-ioslobappprovisioningconfigurationpolicysetitem"></a><span data-ttu-id="ccc6d-103">更新 iosLobAppProvisioningConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="ccc6d-103">Update iosLobAppProvisioningConfigurationPolicySetItem</span></span>

<span data-ttu-id="ccc6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccc6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ccc6d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccc6d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccc6d-107">更新 [iosLobAppProvisioningConfigurationPolicySetItem 对象](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-107">Update the properties of a [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccc6d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ccc6d-108">Prerequisites</span></span>
<span data-ttu-id="ccc6d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccc6d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ccc6d-111">Permission type</span></span>|<span data-ttu-id="ccc6d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ccc6d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccc6d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ccc6d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ccc6d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccc6d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ccc6d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ccc6d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccc6d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-116">Not supported.</span></span>|
|<span data-ttu-id="ccc6d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ccc6d-117">Application</span></span>|<span data-ttu-id="ccc6d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccc6d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccc6d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ccc6d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="ccc6d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ccc6d-120">Request headers</span></span>
|<span data-ttu-id="ccc6d-121">标头</span><span class="sxs-lookup"><span data-stu-id="ccc6d-121">Header</span></span>|<span data-ttu-id="ccc6d-122">值</span><span class="sxs-lookup"><span data-stu-id="ccc6d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccc6d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccc6d-123">Authorization</span></span>|<span data-ttu-id="ccc6d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccc6d-125">接受</span><span class="sxs-lookup"><span data-stu-id="ccc6d-125">Accept</span></span>|<span data-ttu-id="ccc6d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ccc6d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccc6d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ccc6d-127">Request body</span></span>
<span data-ttu-id="ccc6d-128">在请求正文中，提供 [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object.</span></span>

<span data-ttu-id="ccc6d-129">下表显示创建 [iosLobAppProvisioningConfigurationPolicySetItem 时所需的属性](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md).</span></span>

|<span data-ttu-id="ccc6d-130">属性</span><span class="sxs-lookup"><span data-stu-id="ccc6d-130">Property</span></span>|<span data-ttu-id="ccc6d-131">类型</span><span class="sxs-lookup"><span data-stu-id="ccc6d-131">Type</span></span>|<span data-ttu-id="ccc6d-132">说明</span><span class="sxs-lookup"><span data-stu-id="ccc6d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccc6d-133">id</span><span class="sxs-lookup"><span data-stu-id="ccc6d-133">id</span></span>|<span data-ttu-id="ccc6d-134">String</span><span class="sxs-lookup"><span data-stu-id="ccc6d-134">String</span></span>|<span data-ttu-id="ccc6d-135">MobileAppPolicySetItem 的键。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="ccc6d-136">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ccc6d-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ccc6d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ccc6d-137">createdDateTime</span></span>|<span data-ttu-id="ccc6d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccc6d-138">DateTimeOffset</span></span>|<span data-ttu-id="ccc6d-139">PolicySetItem 的创建时间。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="ccc6d-140">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ccc6d-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ccc6d-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ccc6d-141">lastModifiedDateTime</span></span>|<span data-ttu-id="ccc6d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccc6d-142">DateTimeOffset</span></span>|<span data-ttu-id="ccc6d-143">PolicySetItem 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="ccc6d-144">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ccc6d-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ccc6d-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="ccc6d-145">payloadId</span></span>|<span data-ttu-id="ccc6d-146">String</span><span class="sxs-lookup"><span data-stu-id="ccc6d-146">String</span></span>|<span data-ttu-id="ccc6d-147">PolicySetItem 的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="ccc6d-148">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ccc6d-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ccc6d-149">itemType</span><span class="sxs-lookup"><span data-stu-id="ccc6d-149">itemType</span></span>|<span data-ttu-id="ccc6d-150">String</span><span class="sxs-lookup"><span data-stu-id="ccc6d-150">String</span></span>|<span data-ttu-id="ccc6d-151">PolicySetItem 的 policySetType。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="ccc6d-152">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ccc6d-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ccc6d-153">displayName</span><span class="sxs-lookup"><span data-stu-id="ccc6d-153">displayName</span></span>|<span data-ttu-id="ccc6d-154">String</span><span class="sxs-lookup"><span data-stu-id="ccc6d-154">String</span></span>|<span data-ttu-id="ccc6d-155">PolicySetItem 的 DisplayName。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="ccc6d-156">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ccc6d-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ccc6d-157">状态</span><span class="sxs-lookup"><span data-stu-id="ccc6d-157">status</span></span>|[<span data-ttu-id="ccc6d-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="ccc6d-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="ccc6d-159">PolicySetItem 的状态。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="ccc6d-160">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="ccc6d-161">可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="ccc6d-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="ccc6d-162">errorCode</span></span>|[<span data-ttu-id="ccc6d-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="ccc6d-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="ccc6d-164">错误代码（如果发生了任何错误）。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-164">Error code if any occured.</span></span> <span data-ttu-id="ccc6d-165">继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="ccc6d-166">可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="ccc6d-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="ccc6d-167">guidedDeploymentTags</span></span>|<span data-ttu-id="ccc6d-168">String collection</span><span class="sxs-lookup"><span data-stu-id="ccc6d-168">String collection</span></span>|<span data-ttu-id="ccc6d-169">引导式部署的标记 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ccc6d-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ccc6d-170">响应</span><span class="sxs-lookup"><span data-stu-id="ccc6d-170">Response</span></span>
<span data-ttu-id="ccc6d-171">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-171">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccc6d-172">示例</span><span class="sxs-lookup"><span data-stu-id="ccc6d-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccc6d-173">请求</span><span class="sxs-lookup"><span data-stu-id="ccc6d-173">Request</span></span>
<span data-ttu-id="ccc6d-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 329

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="ccc6d-175">响应</span><span class="sxs-lookup"><span data-stu-id="ccc6d-175">Response</span></span>
<span data-ttu-id="ccc6d-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ccc6d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 501

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem",
  "id": "6a978d58-8d58-6a97-588d-976a588d976a",
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




