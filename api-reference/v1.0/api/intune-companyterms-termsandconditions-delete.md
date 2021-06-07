---
title: 删除 termsAndConditions
description: 删除 termsAndConditions。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 53828552ac563c672c663b80aaf6e63d67c76ef8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757232"
---
# <a name="delete-termsandconditions"></a><span data-ttu-id="d0ede-103">删除 termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="d0ede-103">Delete termsAndConditions</span></span>

<span data-ttu-id="d0ede-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0ede-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0ede-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0ede-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0ede-106">删除 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)。</span><span class="sxs-lookup"><span data-stu-id="d0ede-106">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0ede-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d0ede-107">Prerequisites</span></span>
<span data-ttu-id="d0ede-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0ede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0ede-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0ede-110">Permission type</span></span>|<span data-ttu-id="d0ede-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0ede-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0ede-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0ede-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0ede-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0ede-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d0ede-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0ede-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0ede-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0ede-115">Not supported.</span></span>|
|<span data-ttu-id="d0ede-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0ede-116">Application</span></span>|<span data-ttu-id="d0ede-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0ede-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0ede-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0ede-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="d0ede-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0ede-119">Request headers</span></span>
|<span data-ttu-id="d0ede-120">标头</span><span class="sxs-lookup"><span data-stu-id="d0ede-120">Header</span></span>|<span data-ttu-id="d0ede-121">值</span><span class="sxs-lookup"><span data-stu-id="d0ede-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0ede-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0ede-122">Authorization</span></span>|<span data-ttu-id="d0ede-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d0ede-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0ede-124">接受</span><span class="sxs-lookup"><span data-stu-id="d0ede-124">Accept</span></span>|<span data-ttu-id="d0ede-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0ede-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0ede-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0ede-126">Request body</span></span>
<span data-ttu-id="d0ede-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d0ede-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0ede-128">响应</span><span class="sxs-lookup"><span data-stu-id="d0ede-128">Response</span></span>
<span data-ttu-id="d0ede-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d0ede-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d0ede-130">示例</span><span class="sxs-lookup"><span data-stu-id="d0ede-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0ede-131">请求</span><span class="sxs-lookup"><span data-stu-id="d0ede-131">Request</span></span>
<span data-ttu-id="d0ede-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0ede-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="d0ede-133">响应</span><span class="sxs-lookup"><span data-stu-id="d0ede-133">Response</span></span>
<span data-ttu-id="d0ede-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0ede-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




