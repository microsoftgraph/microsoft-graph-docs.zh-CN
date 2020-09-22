---
title: 更新操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a9a9dcf2fafa7caa4e16d4729b4ba80e3b624c96
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48068110"
---
# <a name="update-action"></a><span data-ttu-id="3dc3f-103">更新操作</span><span class="sxs-lookup"><span data-stu-id="3dc3f-103">update action</span></span>

<span data-ttu-id="3dc3f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dc3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3dc3f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3dc3f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3dc3f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3dc3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3dc3f-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dc3f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3dc3f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3dc3f-108">Prerequisites</span></span>
<span data-ttu-id="3dc3f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3dc3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dc3f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3dc3f-111">Permission type</span></span>|<span data-ttu-id="3dc3f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3dc3f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3dc3f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3dc3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3dc3f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dc3f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3dc3f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3dc3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3dc3f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dc3f-116">Not supported.</span></span>|
|<span data-ttu-id="3dc3f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3dc3f-117">Application</span></span>|<span data-ttu-id="3dc3f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dc3f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3dc3f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3dc3f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/update
```

## <a name="request-headers"></a><span data-ttu-id="3dc3f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3dc3f-120">Request headers</span></span>
|<span data-ttu-id="3dc3f-121">标头</span><span class="sxs-lookup"><span data-stu-id="3dc3f-121">Header</span></span>|<span data-ttu-id="3dc3f-122">值</span><span class="sxs-lookup"><span data-stu-id="3dc3f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3dc3f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dc3f-123">Authorization</span></span>|<span data-ttu-id="3dc3f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3dc3f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3dc3f-125">接受</span><span class="sxs-lookup"><span data-stu-id="3dc3f-125">Accept</span></span>|<span data-ttu-id="3dc3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3dc3f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dc3f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3dc3f-127">Request body</span></span>
<span data-ttu-id="3dc3f-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3dc3f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3dc3f-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="3dc3f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3dc3f-130">属性</span><span class="sxs-lookup"><span data-stu-id="3dc3f-130">Property</span></span>|<span data-ttu-id="3dc3f-131">类型</span><span class="sxs-lookup"><span data-stu-id="3dc3f-131">Type</span></span>|<span data-ttu-id="3dc3f-132">说明</span><span class="sxs-lookup"><span data-stu-id="3dc3f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dc3f-133">addedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="3dc3f-133">addedPolicySetItems</span></span>|<span data-ttu-id="3dc3f-134">[policySetItem](../resources/intune-policyset-policysetitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3dc3f-134">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="3dc3f-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dc3f-135">Not yet documented</span></span>|
|<span data-ttu-id="3dc3f-136">updatedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="3dc3f-136">updatedPolicySetItems</span></span>|<span data-ttu-id="3dc3f-137">[policySetItem](../resources/intune-policyset-policysetitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3dc3f-137">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="3dc3f-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dc3f-138">Not yet documented</span></span>|
|<span data-ttu-id="3dc3f-139">deletedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="3dc3f-139">deletedPolicySetItems</span></span>|<span data-ttu-id="3dc3f-140">String collection</span><span class="sxs-lookup"><span data-stu-id="3dc3f-140">String collection</span></span>|<span data-ttu-id="3dc3f-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dc3f-141">Not yet documented</span></span>|
|<span data-ttu-id="3dc3f-142">assignments</span><span class="sxs-lookup"><span data-stu-id="3dc3f-142">assignments</span></span>|<span data-ttu-id="3dc3f-143">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3dc3f-143">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="3dc3f-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3dc3f-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3dc3f-145">响应</span><span class="sxs-lookup"><span data-stu-id="3dc3f-145">Response</span></span>
<span data-ttu-id="3dc3f-146">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3dc3f-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3dc3f-147">示例</span><span class="sxs-lookup"><span data-stu-id="3dc3f-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="3dc3f-148">请求</span><span class="sxs-lookup"><span data-stu-id="3dc3f-148">Request</span></span>
<span data-ttu-id="3dc3f-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3dc3f-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/update

Content-type: application/json
Content-length: 1692

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="3dc3f-150">响应</span><span class="sxs-lookup"><span data-stu-id="3dc3f-150">Response</span></span>
<span data-ttu-id="3dc3f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3dc3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






