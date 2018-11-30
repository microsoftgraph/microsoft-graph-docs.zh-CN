---
title: 删除 mdmWindowsInformationProtectionPolicy
description: 删除 mdmWindowsInformationProtectionPolicy。
ms.openlocfilehash: 6b88f673b556c0dd126981fce8c5b274939b9682
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007994"
---
# <a name="delete-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="364fc-103">删除 mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="364fc-103">Delete mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="364fc-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="364fc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="364fc-105">删除 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="364fc-105">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="364fc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="364fc-106">Prerequisites</span></span>
<span data-ttu-id="364fc-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="364fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="364fc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="364fc-109">Permission type</span></span>|<span data-ttu-id="364fc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="364fc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="364fc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="364fc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="364fc-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="364fc-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="364fc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="364fc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="364fc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="364fc-114">Not supported.</span></span>|
|<span data-ttu-id="364fc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="364fc-115">Application</span></span>|<span data-ttu-id="364fc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="364fc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="364fc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="364fc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="364fc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="364fc-118">Request headers</span></span>
|<span data-ttu-id="364fc-119">标头</span><span class="sxs-lookup"><span data-stu-id="364fc-119">Header</span></span>|<span data-ttu-id="364fc-120">值</span><span class="sxs-lookup"><span data-stu-id="364fc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="364fc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="364fc-121">Authorization</span></span>|<span data-ttu-id="364fc-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="364fc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="364fc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="364fc-123">Accept</span></span>|<span data-ttu-id="364fc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="364fc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="364fc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="364fc-125">Request body</span></span>
<span data-ttu-id="364fc-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="364fc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="364fc-127">响应</span><span class="sxs-lookup"><span data-stu-id="364fc-127">Response</span></span>
<span data-ttu-id="364fc-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="364fc-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="364fc-129">示例</span><span class="sxs-lookup"><span data-stu-id="364fc-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="364fc-130">请求</span><span class="sxs-lookup"><span data-stu-id="364fc-130">Request</span></span>
<span data-ttu-id="364fc-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="364fc-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="364fc-132">响应</span><span class="sxs-lookup"><span data-stu-id="364fc-132">Response</span></span>
<span data-ttu-id="364fc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="364fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



