---
title: 删除 termsAndConditionsAssignment
description: 删除 termsAndConditionsAssignment。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 84020415cd08794b64735adaa5b768acd548ab63
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852078"
---
# <a name="delete-termsandconditionsassignment"></a><span data-ttu-id="4c583-103">删除 termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="4c583-103">Delete termsAndConditionsAssignment</span></span>

> <span data-ttu-id="4c583-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4c583-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c583-105">删除 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="4c583-105">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c583-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="4c583-106">Prerequisites</span></span>
<span data-ttu-id="4c583-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="4c583-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c583-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c583-109">Permission type</span></span>|<span data-ttu-id="4c583-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4c583-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c583-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c583-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c583-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c583-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4c583-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c583-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c583-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c583-114">Not supported.</span></span>|
|<span data-ttu-id="4c583-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c583-115">Application</span></span>|<span data-ttu-id="4c583-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c583-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c583-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c583-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4c583-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c583-118">Request headers</span></span>
|<span data-ttu-id="4c583-119">标头</span><span class="sxs-lookup"><span data-stu-id="4c583-119">Header</span></span>|<span data-ttu-id="4c583-120">值</span><span class="sxs-lookup"><span data-stu-id="4c583-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c583-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c583-121">Authorization</span></span>|<span data-ttu-id="4c583-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4c583-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c583-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4c583-123">Accept</span></span>|<span data-ttu-id="4c583-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4c583-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c583-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c583-125">Request body</span></span>
<span data-ttu-id="4c583-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4c583-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c583-127">响应</span><span class="sxs-lookup"><span data-stu-id="4c583-127">Response</span></span>
<span data-ttu-id="4c583-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4c583-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4c583-129">示例</span><span class="sxs-lookup"><span data-stu-id="4c583-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c583-130">请求</span><span class="sxs-lookup"><span data-stu-id="4c583-130">Request</span></span>
<span data-ttu-id="4c583-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4c583-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="4c583-132">响应</span><span class="sxs-lookup"><span data-stu-id="4c583-132">Response</span></span>
<span data-ttu-id="4c583-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4c583-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



