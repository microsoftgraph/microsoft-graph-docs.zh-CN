---
title: assign 操作
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 6812f3c1879c331cc27aeb25ea4516af080252b7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315300"
---
# <a name="assign-action"></a><span data-ttu-id="f5bbb-103">assign 操作</span><span class="sxs-lookup"><span data-stu-id="f5bbb-103">assign action</span></span>

> <span data-ttu-id="f5bbb-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f5bbb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5bbb-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f5bbb-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5bbb-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f5bbb-106">Prerequisites</span></span>
<span data-ttu-id="f5bbb-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f5bbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5bbb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5bbb-109">Permission type</span></span>|<span data-ttu-id="f5bbb-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f5bbb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5bbb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5bbb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f5bbb-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5bbb-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f5bbb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5bbb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5bbb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5bbb-114">Not supported.</span></span>|
|<span data-ttu-id="f5bbb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5bbb-115">Application</span></span>|<span data-ttu-id="f5bbb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5bbb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5bbb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5bbb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="f5bbb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5bbb-118">Request headers</span></span>
|<span data-ttu-id="f5bbb-119">标头</span><span class="sxs-lookup"><span data-stu-id="f5bbb-119">Header</span></span>|<span data-ttu-id="f5bbb-120">值</span><span class="sxs-lookup"><span data-stu-id="f5bbb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5bbb-121">授权</span><span class="sxs-lookup"><span data-stu-id="f5bbb-121">Authorization</span></span>|<span data-ttu-id="f5bbb-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f5bbb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5bbb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f5bbb-123">Accept</span></span>|<span data-ttu-id="f5bbb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f5bbb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5bbb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5bbb-125">Request body</span></span>
<span data-ttu-id="f5bbb-126">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5bbb-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f5bbb-127">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="f5bbb-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f5bbb-128">属性</span><span class="sxs-lookup"><span data-stu-id="f5bbb-128">Property</span></span>|<span data-ttu-id="f5bbb-129">类型</span><span class="sxs-lookup"><span data-stu-id="f5bbb-129">Type</span></span>|<span data-ttu-id="f5bbb-130">说明</span><span class="sxs-lookup"><span data-stu-id="f5bbb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5bbb-131">enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="f5bbb-131">enrollmentConfigurationAssignments</span></span>|<span data-ttu-id="f5bbb-132">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5bbb-132">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f5bbb-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f5bbb-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f5bbb-134">响应</span><span class="sxs-lookup"><span data-stu-id="f5bbb-134">Response</span></span>
<span data-ttu-id="f5bbb-135">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f5bbb-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f5bbb-136">示例</span><span class="sxs-lookup"><span data-stu-id="f5bbb-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="f5bbb-137">请求</span><span class="sxs-lookup"><span data-stu-id="f5bbb-137">Request</span></span>
<span data-ttu-id="f5bbb-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5bbb-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f5bbb-139">响应</span><span class="sxs-lookup"><span data-stu-id="f5bbb-139">Response</span></span>
<span data-ttu-id="f5bbb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f5bbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



