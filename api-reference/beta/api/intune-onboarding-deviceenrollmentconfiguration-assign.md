---
title: assign 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32c6cbc15185281813bc3721bc61d4906776bdda
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900585"
---
# <a name="assign-action"></a><span data-ttu-id="c4601-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="c4601-103">assign action</span></span>

> <span data-ttu-id="c4601-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c4601-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4601-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c4601-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4601-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c4601-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4601-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c4601-107">Prerequisites</span></span>
<span data-ttu-id="c4601-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4601-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4601-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4601-110">Permission type</span></span>|<span data-ttu-id="c4601-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c4601-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4601-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4601-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4601-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4601-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c4601-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4601-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4601-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4601-115">Not supported.</span></span>|
|<span data-ttu-id="c4601-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4601-116">Application</span></span>|<span data-ttu-id="c4601-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4601-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4601-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4601-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="c4601-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4601-119">Request headers</span></span>
|<span data-ttu-id="c4601-120">标头</span><span class="sxs-lookup"><span data-stu-id="c4601-120">Header</span></span>|<span data-ttu-id="c4601-121">值</span><span class="sxs-lookup"><span data-stu-id="c4601-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4601-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4601-122">Authorization</span></span>|<span data-ttu-id="c4601-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c4601-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4601-124">接受</span><span class="sxs-lookup"><span data-stu-id="c4601-124">Accept</span></span>|<span data-ttu-id="c4601-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4601-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4601-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4601-126">Request body</span></span>
<span data-ttu-id="c4601-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4601-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c4601-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c4601-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c4601-129">属性</span><span class="sxs-lookup"><span data-stu-id="c4601-129">Property</span></span>|<span data-ttu-id="c4601-130">类型</span><span class="sxs-lookup"><span data-stu-id="c4601-130">Type</span></span>|<span data-ttu-id="c4601-131">说明</span><span class="sxs-lookup"><span data-stu-id="c4601-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4601-132">enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="c4601-132">enrollmentConfigurationAssignments</span></span>|<span data-ttu-id="c4601-133">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c4601-133">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c4601-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c4601-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c4601-135">响应</span><span class="sxs-lookup"><span data-stu-id="c4601-135">Response</span></span>
<span data-ttu-id="c4601-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c4601-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c4601-137">示例</span><span class="sxs-lookup"><span data-stu-id="c4601-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4601-138">请求</span><span class="sxs-lookup"><span data-stu-id="c4601-138">Request</span></span>
<span data-ttu-id="c4601-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4601-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign

Content-type: application/json
Content-length: 304

{
  "enrollmentConfigurationAssignments": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c4601-140">响应</span><span class="sxs-lookup"><span data-stu-id="c4601-140">Response</span></span>
<span data-ttu-id="c4601-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c4601-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




