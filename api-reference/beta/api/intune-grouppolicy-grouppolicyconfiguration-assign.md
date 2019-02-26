---
title: assign 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4cf7440dd856731a0079ce7781b4c9c05d932d9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151651"
---
# <a name="assign-action"></a><span data-ttu-id="b7b40-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="b7b40-103">assign action</span></span>

> <span data-ttu-id="b7b40-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b7b40-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7b40-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7b40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7b40-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b7b40-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7b40-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b7b40-107">Prerequisites</span></span>
<span data-ttu-id="b7b40-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b7b40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b7b40-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7b40-110">Permission type</span></span>|<span data-ttu-id="b7b40-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b7b40-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7b40-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7b40-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7b40-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7b40-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b7b40-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7b40-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7b40-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7b40-115">Not supported.</span></span>|
|<span data-ttu-id="b7b40-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7b40-116">Application</span></span>|<span data-ttu-id="b7b40-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7b40-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7b40-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7b40-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="b7b40-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7b40-119">Request headers</span></span>
|<span data-ttu-id="b7b40-120">标头</span><span class="sxs-lookup"><span data-stu-id="b7b40-120">Header</span></span>|<span data-ttu-id="b7b40-121">值</span><span class="sxs-lookup"><span data-stu-id="b7b40-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7b40-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7b40-122">Authorization</span></span>|<span data-ttu-id="b7b40-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b7b40-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7b40-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b7b40-124">Accept</span></span>|<span data-ttu-id="b7b40-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7b40-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7b40-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7b40-126">Request body</span></span>
<span data-ttu-id="b7b40-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7b40-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b7b40-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="b7b40-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b7b40-129">属性</span><span class="sxs-lookup"><span data-stu-id="b7b40-129">Property</span></span>|<span data-ttu-id="b7b40-130">类型</span><span class="sxs-lookup"><span data-stu-id="b7b40-130">Type</span></span>|<span data-ttu-id="b7b40-131">说明</span><span class="sxs-lookup"><span data-stu-id="b7b40-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7b40-132">assignments</span><span class="sxs-lookup"><span data-stu-id="b7b40-132">assignments</span></span>|<span data-ttu-id="b7b40-133">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="b7b40-133">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b7b40-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b7b40-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b7b40-135">响应</span><span class="sxs-lookup"><span data-stu-id="b7b40-135">Response</span></span>
<span data-ttu-id="b7b40-136">如果成功, 此操作会在`200 OK`响应正文中返回响应代码和[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合。</span><span class="sxs-lookup"><span data-stu-id="b7b40-136">If successful, this action returns a `200 OK` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7b40-137">示例</span><span class="sxs-lookup"><span data-stu-id="b7b40-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7b40-138">请求</span><span class="sxs-lookup"><span data-stu-id="b7b40-138">Request</span></span>
<span data-ttu-id="b7b40-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b7b40-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign

Content-type: application/json
Content-length: 350

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b7b40-140">响应</span><span class="sxs-lookup"><span data-stu-id="b7b40-140">Response</span></span>
<span data-ttu-id="b7b40-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b7b40-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




