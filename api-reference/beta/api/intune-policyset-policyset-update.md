---
title: 更新操作
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d3714a89ac13b90d79a669ba35e7bb8b541cf13
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802109"
---
# <a name="update-action"></a><span data-ttu-id="f4aac-103">更新操作</span><span class="sxs-lookup"><span data-stu-id="f4aac-103">update action</span></span>

> <span data-ttu-id="f4aac-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4aac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4aac-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4aac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4aac-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f4aac-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4aac-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4aac-107">Prerequisites</span></span>
<span data-ttu-id="f4aac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4aac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4aac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4aac-110">Permission type</span></span>|<span data-ttu-id="f4aac-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4aac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4aac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4aac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4aac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4aac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4aac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4aac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4aac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4aac-115">Not supported.</span></span>|
|<span data-ttu-id="f4aac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4aac-116">Application</span></span>|<span data-ttu-id="f4aac-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4aac-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4aac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4aac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/update
```

## <a name="request-headers"></a><span data-ttu-id="f4aac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4aac-119">Request headers</span></span>
|<span data-ttu-id="f4aac-120">标头</span><span class="sxs-lookup"><span data-stu-id="f4aac-120">Header</span></span>|<span data-ttu-id="f4aac-121">值</span><span class="sxs-lookup"><span data-stu-id="f4aac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4aac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4aac-122">Authorization</span></span>|<span data-ttu-id="f4aac-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4aac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4aac-124">接受</span><span class="sxs-lookup"><span data-stu-id="f4aac-124">Accept</span></span>|<span data-ttu-id="f4aac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4aac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4aac-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4aac-126">Request body</span></span>
<span data-ttu-id="f4aac-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4aac-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f4aac-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="f4aac-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f4aac-129">属性</span><span class="sxs-lookup"><span data-stu-id="f4aac-129">Property</span></span>|<span data-ttu-id="f4aac-130">类型</span><span class="sxs-lookup"><span data-stu-id="f4aac-130">Type</span></span>|<span data-ttu-id="f4aac-131">说明</span><span class="sxs-lookup"><span data-stu-id="f4aac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4aac-132">addedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="f4aac-132">addedPolicySetItems</span></span>|<span data-ttu-id="f4aac-133">[policySetItem](../resources/intune-policyset-policysetitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="f4aac-133">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="f4aac-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f4aac-134">Not yet documented</span></span>|
|<span data-ttu-id="f4aac-135">updatedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="f4aac-135">updatedPolicySetItems</span></span>|<span data-ttu-id="f4aac-136">[policySetItem](../resources/intune-policyset-policysetitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="f4aac-136">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="f4aac-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f4aac-137">Not yet documented</span></span>|
|<span data-ttu-id="f4aac-138">deletedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="f4aac-138">deletedPolicySetItems</span></span>|<span data-ttu-id="f4aac-139">String collection</span><span class="sxs-lookup"><span data-stu-id="f4aac-139">String collection</span></span>|<span data-ttu-id="f4aac-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f4aac-140">Not yet documented</span></span>|
|<span data-ttu-id="f4aac-141">assignments</span><span class="sxs-lookup"><span data-stu-id="f4aac-141">assignments</span></span>|<span data-ttu-id="f4aac-142">[policySetAssignment](../resources/intune-policyset-policysetassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="f4aac-142">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="f4aac-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f4aac-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f4aac-144">响应</span><span class="sxs-lookup"><span data-stu-id="f4aac-144">Response</span></span>
<span data-ttu-id="f4aac-145">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f4aac-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f4aac-146">示例</span><span class="sxs-lookup"><span data-stu-id="f4aac-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4aac-147">请求</span><span class="sxs-lookup"><span data-stu-id="f4aac-147">Request</span></span>
<span data-ttu-id="f4aac-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4aac-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/update

Content-type: application/json
Content-length: 1529

{
  "addedPolicySetItems": [
    {
      "@odata.type": "#microsoft.graph.policySetItem",
      "id": "06ec9d5e-9d5e-06ec-5e9d-ec065e9dec06",
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
  ],
  "updatedPolicySetItems": [
    {
      "@odata.type": "#microsoft.graph.policySetItem",
      "id": "06ec9d5e-9d5e-06ec-5e9d-ec065e9dec06",
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
  ],
  "deletedPolicySetItems": [
    "Deleted Policy Set Items value"
  ],
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.policySetAssignment",
      "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f4aac-149">响应</span><span class="sxs-lookup"><span data-stu-id="f4aac-149">Response</span></span>
<span data-ttu-id="f4aac-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4aac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




