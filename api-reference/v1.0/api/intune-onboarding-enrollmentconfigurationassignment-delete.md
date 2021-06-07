---
title: 删除 enrollmentConfigurationAssignment
description: 删除 enrollmentConfigurationAssignment。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3f68215015717fb81e8edad2845ac8465f72ca9e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758001"
---
# <a name="delete-enrollmentconfigurationassignment"></a><span data-ttu-id="8e888-103">删除 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8e888-103">Delete enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="8e888-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e888-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e888-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e888-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e888-106">删除 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="8e888-106">Deletes a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e888-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8e888-107">Prerequisites</span></span>
<span data-ttu-id="8e888-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e888-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e888-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e888-110">Permission type</span></span>|<span data-ttu-id="8e888-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e888-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e888-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e888-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e888-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e888-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8e888-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e888-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e888-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e888-115">Not supported.</span></span>|
|<span data-ttu-id="8e888-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e888-116">Application</span></span>|<span data-ttu-id="8e888-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e888-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e888-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e888-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8e888-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e888-119">Request headers</span></span>
|<span data-ttu-id="8e888-120">标头</span><span class="sxs-lookup"><span data-stu-id="8e888-120">Header</span></span>|<span data-ttu-id="8e888-121">值</span><span class="sxs-lookup"><span data-stu-id="8e888-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e888-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e888-122">Authorization</span></span>|<span data-ttu-id="8e888-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8e888-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e888-124">接受</span><span class="sxs-lookup"><span data-stu-id="8e888-124">Accept</span></span>|<span data-ttu-id="8e888-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8e888-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e888-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e888-126">Request body</span></span>
<span data-ttu-id="8e888-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8e888-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e888-128">响应</span><span class="sxs-lookup"><span data-stu-id="8e888-128">Response</span></span>
<span data-ttu-id="8e888-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8e888-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8e888-130">示例</span><span class="sxs-lookup"><span data-stu-id="8e888-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e888-131">请求</span><span class="sxs-lookup"><span data-stu-id="8e888-131">Request</span></span>
<span data-ttu-id="8e888-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e888-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="8e888-133">响应</span><span class="sxs-lookup"><span data-stu-id="8e888-133">Response</span></span>
<span data-ttu-id="8e888-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8e888-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




