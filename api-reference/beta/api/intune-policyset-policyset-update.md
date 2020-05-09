---
title: 更新操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01e437970f9213e80b29ed6b20f93ab87bdcd30b
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179269"
---
# <a name="update-action"></a><span data-ttu-id="d0946-103">更新操作</span><span class="sxs-lookup"><span data-stu-id="d0946-103">update action</span></span>

<span data-ttu-id="d0946-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0946-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0946-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d0946-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0946-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0946-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0946-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d0946-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0946-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d0946-108">Prerequisites</span></span>
<span data-ttu-id="d0946-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0946-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0946-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0946-111">Permission type</span></span>|<span data-ttu-id="d0946-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d0946-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0946-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0946-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0946-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0946-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0946-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0946-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0946-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0946-116">Not supported.</span></span>|
|<span data-ttu-id="d0946-117">Application</span><span class="sxs-lookup"><span data-stu-id="d0946-117">Application</span></span>|<span data-ttu-id="d0946-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0946-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0946-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0946-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/update
```

## <a name="request-headers"></a><span data-ttu-id="d0946-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0946-120">Request headers</span></span>
|<span data-ttu-id="d0946-121">标头</span><span class="sxs-lookup"><span data-stu-id="d0946-121">Header</span></span>|<span data-ttu-id="d0946-122">值</span><span class="sxs-lookup"><span data-stu-id="d0946-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0946-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0946-123">Authorization</span></span>|<span data-ttu-id="d0946-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d0946-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0946-125">接受</span><span class="sxs-lookup"><span data-stu-id="d0946-125">Accept</span></span>|<span data-ttu-id="d0946-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0946-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0946-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0946-127">Request body</span></span>
<span data-ttu-id="d0946-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0946-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d0946-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="d0946-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d0946-130">属性</span><span class="sxs-lookup"><span data-stu-id="d0946-130">Property</span></span>|<span data-ttu-id="d0946-131">类型</span><span class="sxs-lookup"><span data-stu-id="d0946-131">Type</span></span>|<span data-ttu-id="d0946-132">说明</span><span class="sxs-lookup"><span data-stu-id="d0946-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0946-133">addedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="d0946-133">addedPolicySetItems</span></span>|<span data-ttu-id="d0946-134">[policySetItem](../resources/intune-policyset-policysetitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="d0946-134">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="d0946-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d0946-135">Not yet documented</span></span>|
|<span data-ttu-id="d0946-136">updatedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="d0946-136">updatedPolicySetItems</span></span>|<span data-ttu-id="d0946-137">[policySetItem](../resources/intune-policyset-policysetitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="d0946-137">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="d0946-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d0946-138">Not yet documented</span></span>|
|<span data-ttu-id="d0946-139">deletedPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="d0946-139">deletedPolicySetItems</span></span>|<span data-ttu-id="d0946-140">String collection</span><span class="sxs-lookup"><span data-stu-id="d0946-140">String collection</span></span>|<span data-ttu-id="d0946-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d0946-141">Not yet documented</span></span>|
|<span data-ttu-id="d0946-142">assignments</span><span class="sxs-lookup"><span data-stu-id="d0946-142">assignments</span></span>|<span data-ttu-id="d0946-143">[policySetAssignment](../resources/intune-policyset-policysetassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="d0946-143">[policySetAssignment](../resources/intune-policyset-policysetassignment.md) collection</span></span>|<span data-ttu-id="d0946-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d0946-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d0946-145">响应</span><span class="sxs-lookup"><span data-stu-id="d0946-145">Response</span></span>
<span data-ttu-id="d0946-146">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d0946-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d0946-147">示例</span><span class="sxs-lookup"><span data-stu-id="d0946-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0946-148">请求</span><span class="sxs-lookup"><span data-stu-id="d0946-148">Request</span></span>
<span data-ttu-id="d0946-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0946-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/update

Content-type: application/json
Content-length: 1517

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d0946-150">响应</span><span class="sxs-lookup"><span data-stu-id="d0946-150">Response</span></span>
<span data-ttu-id="d0946-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0946-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



