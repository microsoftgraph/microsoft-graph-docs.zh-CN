---
title: 删除 enrollmentConfigurationAssignment
description: 删除 enrollmentConfigurationAssignment。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dcdf06654386f33135696e0ff1ead96d9be19db6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802837"
---
# <a name="delete-enrollmentconfigurationassignment"></a><span data-ttu-id="bb1d6-103">删除 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="bb1d6-103">Delete enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="bb1d6-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb1d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb1d6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb1d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb1d6-106">删除 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="bb1d6-106">Deletes a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb1d6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bb1d6-107">Prerequisites</span></span>
<span data-ttu-id="bb1d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb1d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb1d6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb1d6-110">Permission type</span></span>|<span data-ttu-id="bb1d6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bb1d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb1d6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb1d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb1d6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb1d6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bb1d6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb1d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb1d6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb1d6-115">Not supported.</span></span>|
|<span data-ttu-id="bb1d6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb1d6-116">Application</span></span>|<span data-ttu-id="bb1d6-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb1d6-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb1d6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb1d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="bb1d6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb1d6-119">Request headers</span></span>
|<span data-ttu-id="bb1d6-120">标头</span><span class="sxs-lookup"><span data-stu-id="bb1d6-120">Header</span></span>|<span data-ttu-id="bb1d6-121">值</span><span class="sxs-lookup"><span data-stu-id="bb1d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb1d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb1d6-122">Authorization</span></span>|<span data-ttu-id="bb1d6-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bb1d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb1d6-124">接受</span><span class="sxs-lookup"><span data-stu-id="bb1d6-124">Accept</span></span>|<span data-ttu-id="bb1d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb1d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb1d6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb1d6-126">Request body</span></span>
<span data-ttu-id="bb1d6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb1d6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb1d6-128">响应</span><span class="sxs-lookup"><span data-stu-id="bb1d6-128">Response</span></span>
<span data-ttu-id="bb1d6-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bb1d6-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bb1d6-130">示例</span><span class="sxs-lookup"><span data-stu-id="bb1d6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb1d6-131">请求</span><span class="sxs-lookup"><span data-stu-id="bb1d6-131">Request</span></span>
<span data-ttu-id="bb1d6-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb1d6-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="bb1d6-133">响应</span><span class="sxs-lookup"><span data-stu-id="bb1d6-133">Response</span></span>
<span data-ttu-id="bb1d6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb1d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




