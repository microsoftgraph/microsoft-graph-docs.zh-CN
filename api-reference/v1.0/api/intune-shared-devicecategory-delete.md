---
title: 删除 deviceCategory
description: 删除 deviceCategory。
ms.openlocfilehash: a85190a47bca7ec58d899be3618ae59229ecef06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011673"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="ecb8f-103">删除 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="ecb8f-103">Delete deviceCategory</span></span>

> <span data-ttu-id="ecb8f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ecb8f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecb8f-105">删除 [deviceCategory](../resources/intune-shared-devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="ecb8f-105">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ecb8f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ecb8f-106">Prerequisites</span></span>
<span data-ttu-id="ecb8f-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ecb8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecb8f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ecb8f-109">Permission type</span></span>|<span data-ttu-id="ecb8f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ecb8f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecb8f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ecb8f-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ecb8f-112">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="ecb8f-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ecb8f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecb8f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ecb8f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ecb8f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecb8f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecb8f-115">Not supported.</span></span>|
|<span data-ttu-id="ecb8f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ecb8f-116">Application</span></span>|<span data-ttu-id="ecb8f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecb8f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecb8f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ecb8f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="ecb8f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ecb8f-119">Request headers</span></span>
|<span data-ttu-id="ecb8f-120">标头</span><span class="sxs-lookup"><span data-stu-id="ecb8f-120">Header</span></span>|<span data-ttu-id="ecb8f-121">值</span><span class="sxs-lookup"><span data-stu-id="ecb8f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecb8f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecb8f-122">Authorization</span></span>|<span data-ttu-id="ecb8f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ecb8f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecb8f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ecb8f-124">Accept</span></span>|<span data-ttu-id="ecb8f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ecb8f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecb8f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ecb8f-126">Request body</span></span>
<span data-ttu-id="ecb8f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ecb8f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecb8f-128">响应</span><span class="sxs-lookup"><span data-stu-id="ecb8f-128">Response</span></span>
<span data-ttu-id="ecb8f-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ecb8f-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ecb8f-130">示例</span><span class="sxs-lookup"><span data-stu-id="ecb8f-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="ecb8f-131">请求</span><span class="sxs-lookup"><span data-stu-id="ecb8f-131">Request</span></span>
<span data-ttu-id="ecb8f-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ecb8f-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="ecb8f-133">响应</span><span class="sxs-lookup"><span data-stu-id="ecb8f-133">Response</span></span>
<span data-ttu-id="ecb8f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ecb8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



