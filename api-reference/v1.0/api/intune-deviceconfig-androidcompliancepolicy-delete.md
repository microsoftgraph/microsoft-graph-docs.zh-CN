---
title: 删除 androidCompliancePolicy
description: 删除 androidCompliancePolicy。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7e68781d3d2403ad7b56de4419ef7fc8e042b93a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43316738"
---
# <a name="delete-androidcompliancepolicy"></a><span data-ttu-id="2f6ea-103">删除 androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2f6ea-103">Delete androidCompliancePolicy</span></span>

<span data-ttu-id="2f6ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f6ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f6ea-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f6ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f6ea-106">删除 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="2f6ea-106">Deletes a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f6ea-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f6ea-107">Prerequisites</span></span>
<span data-ttu-id="2f6ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f6ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f6ea-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f6ea-110">Permission type</span></span>|<span data-ttu-id="2f6ea-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2f6ea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f6ea-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f6ea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f6ea-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f6ea-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f6ea-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f6ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f6ea-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f6ea-115">Not supported.</span></span>|
|<span data-ttu-id="2f6ea-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f6ea-116">Application</span></span>|<span data-ttu-id="2f6ea-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f6ea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f6ea-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f6ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="2f6ea-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f6ea-119">Request headers</span></span>
|<span data-ttu-id="2f6ea-120">标头</span><span class="sxs-lookup"><span data-stu-id="2f6ea-120">Header</span></span>|<span data-ttu-id="2f6ea-121">值</span><span class="sxs-lookup"><span data-stu-id="2f6ea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f6ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f6ea-122">Authorization</span></span>|<span data-ttu-id="2f6ea-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f6ea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f6ea-124">接受</span><span class="sxs-lookup"><span data-stu-id="2f6ea-124">Accept</span></span>|<span data-ttu-id="2f6ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f6ea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f6ea-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f6ea-126">Request body</span></span>
<span data-ttu-id="2f6ea-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2f6ea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f6ea-128">响应</span><span class="sxs-lookup"><span data-stu-id="2f6ea-128">Response</span></span>
<span data-ttu-id="2f6ea-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2f6ea-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2f6ea-130">示例</span><span class="sxs-lookup"><span data-stu-id="2f6ea-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f6ea-131">请求</span><span class="sxs-lookup"><span data-stu-id="2f6ea-131">Request</span></span>
<span data-ttu-id="2f6ea-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f6ea-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="2f6ea-133">响应</span><span class="sxs-lookup"><span data-stu-id="2f6ea-133">Response</span></span>
<span data-ttu-id="2f6ea-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f6ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






