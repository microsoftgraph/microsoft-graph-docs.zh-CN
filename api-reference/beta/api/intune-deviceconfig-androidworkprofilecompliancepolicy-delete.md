---
title: 删除 androidWorkProfileCompliancePolicy
description: 删除 androidWorkProfileCompliancePolicy。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7aa216f89c5cc365c3b02e7e3120c4dde0ec76e5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340841"
---
# <a name="delete-androidworkprofilecompliancepolicy"></a><span data-ttu-id="29afb-103">删除 androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="29afb-103">Delete androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="29afb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="29afb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29afb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29afb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29afb-106">删除[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="29afb-106">Deletes a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29afb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="29afb-107">Prerequisites</span></span>
<span data-ttu-id="29afb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29afb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29afb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="29afb-110">Permission type</span></span>|<span data-ttu-id="29afb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="29afb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29afb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29afb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="29afb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29afb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="29afb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29afb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29afb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="29afb-115">Not supported.</span></span>|
|<span data-ttu-id="29afb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="29afb-116">Application</span></span>|<span data-ttu-id="29afb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29afb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29afb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29afb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="29afb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="29afb-119">Request headers</span></span>
|<span data-ttu-id="29afb-120">标头</span><span class="sxs-lookup"><span data-stu-id="29afb-120">Header</span></span>|<span data-ttu-id="29afb-121">值</span><span class="sxs-lookup"><span data-stu-id="29afb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29afb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="29afb-122">Authorization</span></span>|<span data-ttu-id="29afb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="29afb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29afb-124">接受</span><span class="sxs-lookup"><span data-stu-id="29afb-124">Accept</span></span>|<span data-ttu-id="29afb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="29afb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29afb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="29afb-126">Request body</span></span>
<span data-ttu-id="29afb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="29afb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29afb-128">响应</span><span class="sxs-lookup"><span data-stu-id="29afb-128">Response</span></span>
<span data-ttu-id="29afb-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="29afb-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="29afb-130">示例</span><span class="sxs-lookup"><span data-stu-id="29afb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="29afb-131">请求</span><span class="sxs-lookup"><span data-stu-id="29afb-131">Request</span></span>
<span data-ttu-id="29afb-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29afb-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="29afb-133">响应</span><span class="sxs-lookup"><span data-stu-id="29afb-133">Response</span></span>
<span data-ttu-id="29afb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29afb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






