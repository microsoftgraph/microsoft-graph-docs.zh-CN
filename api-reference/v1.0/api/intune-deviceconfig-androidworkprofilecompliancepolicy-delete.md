---
title: 删除 androidWorkProfileCompliancePolicy
description: 删除 androidWorkProfileCompliancePolicy。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 397f1cc2e0caa315dec08fceb81a795ffd907835
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757204"
---
# <a name="delete-androidworkprofilecompliancepolicy"></a><span data-ttu-id="31e2d-103">删除 androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="31e2d-103">Delete androidWorkProfileCompliancePolicy</span></span>

<span data-ttu-id="31e2d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31e2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31e2d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="31e2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31e2d-106">删除 [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="31e2d-106">Deletes a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31e2d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="31e2d-107">Prerequisites</span></span>
<span data-ttu-id="31e2d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31e2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31e2d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="31e2d-110">Permission type</span></span>|<span data-ttu-id="31e2d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31e2d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31e2d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31e2d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31e2d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31e2d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31e2d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31e2d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31e2d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="31e2d-115">Not supported.</span></span>|
|<span data-ttu-id="31e2d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="31e2d-116">Application</span></span>|<span data-ttu-id="31e2d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31e2d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31e2d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31e2d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="31e2d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="31e2d-119">Request headers</span></span>
|<span data-ttu-id="31e2d-120">标头</span><span class="sxs-lookup"><span data-stu-id="31e2d-120">Header</span></span>|<span data-ttu-id="31e2d-121">值</span><span class="sxs-lookup"><span data-stu-id="31e2d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31e2d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31e2d-122">Authorization</span></span>|<span data-ttu-id="31e2d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="31e2d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31e2d-124">接受</span><span class="sxs-lookup"><span data-stu-id="31e2d-124">Accept</span></span>|<span data-ttu-id="31e2d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31e2d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31e2d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="31e2d-126">Request body</span></span>
<span data-ttu-id="31e2d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="31e2d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31e2d-128">响应</span><span class="sxs-lookup"><span data-stu-id="31e2d-128">Response</span></span>
<span data-ttu-id="31e2d-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="31e2d-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="31e2d-130">示例</span><span class="sxs-lookup"><span data-stu-id="31e2d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="31e2d-131">请求</span><span class="sxs-lookup"><span data-stu-id="31e2d-131">Request</span></span>
<span data-ttu-id="31e2d-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31e2d-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="31e2d-133">响应</span><span class="sxs-lookup"><span data-stu-id="31e2d-133">Response</span></span>
<span data-ttu-id="31e2d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="31e2d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




