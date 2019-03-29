---
title: assign 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a67fecb2916b0394a9562d29692233ce9188f59e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961019"
---
# <a name="assign-action"></a><span data-ttu-id="626da-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="626da-103">assign action</span></span>

> <span data-ttu-id="626da-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="626da-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="626da-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="626da-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="626da-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="626da-106">Prerequisites</span></span>
<span data-ttu-id="626da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="626da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="626da-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="626da-109">Permission type</span></span>|<span data-ttu-id="626da-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="626da-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="626da-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="626da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="626da-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="626da-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="626da-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="626da-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="626da-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="626da-114">Not supported.</span></span>|
|<span data-ttu-id="626da-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="626da-115">Application</span></span>|<span data-ttu-id="626da-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="626da-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="626da-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="626da-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="626da-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="626da-118">Request headers</span></span>
|<span data-ttu-id="626da-119">标头</span><span class="sxs-lookup"><span data-stu-id="626da-119">Header</span></span>|<span data-ttu-id="626da-120">值</span><span class="sxs-lookup"><span data-stu-id="626da-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="626da-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="626da-121">Authorization</span></span>|<span data-ttu-id="626da-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="626da-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="626da-123">接受</span><span class="sxs-lookup"><span data-stu-id="626da-123">Accept</span></span>|<span data-ttu-id="626da-124">application/json</span><span class="sxs-lookup"><span data-stu-id="626da-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="626da-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="626da-125">Request body</span></span>
<span data-ttu-id="626da-126">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="626da-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="626da-127">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="626da-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="626da-128">属性</span><span class="sxs-lookup"><span data-stu-id="626da-128">Property</span></span>|<span data-ttu-id="626da-129">类型</span><span class="sxs-lookup"><span data-stu-id="626da-129">Type</span></span>|<span data-ttu-id="626da-130">说明</span><span class="sxs-lookup"><span data-stu-id="626da-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="626da-131">enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="626da-131">enrollmentConfigurationAssignments</span></span>|<span data-ttu-id="626da-132">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="626da-132">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="626da-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="626da-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="626da-134">响应</span><span class="sxs-lookup"><span data-stu-id="626da-134">Response</span></span>
<span data-ttu-id="626da-135">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="626da-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="626da-136">示例</span><span class="sxs-lookup"><span data-stu-id="626da-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="626da-137">请求</span><span class="sxs-lookup"><span data-stu-id="626da-137">Request</span></span>
<span data-ttu-id="626da-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="626da-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign

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

### <a name="response"></a><span data-ttu-id="626da-139">响应</span><span class="sxs-lookup"><span data-stu-id="626da-139">Response</span></span>
<span data-ttu-id="626da-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="626da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



