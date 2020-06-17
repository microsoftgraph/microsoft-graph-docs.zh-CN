---
title: 删除 complianceManagementPartner
description: 删除 complianceManagementPartner。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d2c9cdc6571339ca38bf4f575d658de1c9cf83c
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744123"
---
# <a name="delete-compliancemanagementpartner"></a><span data-ttu-id="4e7e1-103">删除 complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="4e7e1-103">Delete complianceManagementPartner</span></span>

<span data-ttu-id="4e7e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e7e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e7e1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e7e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e7e1-106">删除[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="4e7e1-106">Deletes a [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e7e1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4e7e1-107">Prerequisites</span></span>
<span data-ttu-id="4e7e1-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4e7e1-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4e7e1-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e7e1-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e7e1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e7e1-110">Permission type</span></span>|<span data-ttu-id="4e7e1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4e7e1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e7e1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e7e1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e7e1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e7e1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4e7e1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e7e1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e7e1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e7e1-115">Not supported.</span></span>|
|<span data-ttu-id="4e7e1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e7e1-116">Application</span></span>|<span data-ttu-id="4e7e1-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e7e1-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e7e1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e7e1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="4e7e1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e7e1-119">Request headers</span></span>
|<span data-ttu-id="4e7e1-120">标头</span><span class="sxs-lookup"><span data-stu-id="4e7e1-120">Header</span></span>|<span data-ttu-id="4e7e1-121">值</span><span class="sxs-lookup"><span data-stu-id="4e7e1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e7e1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e7e1-122">Authorization</span></span>|<span data-ttu-id="4e7e1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4e7e1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e7e1-124">接受</span><span class="sxs-lookup"><span data-stu-id="4e7e1-124">Accept</span></span>|<span data-ttu-id="4e7e1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e7e1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e7e1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e7e1-126">Request body</span></span>
<span data-ttu-id="4e7e1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e7e1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e7e1-128">响应</span><span class="sxs-lookup"><span data-stu-id="4e7e1-128">Response</span></span>
<span data-ttu-id="4e7e1-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4e7e1-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4e7e1-130">示例</span><span class="sxs-lookup"><span data-stu-id="4e7e1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e7e1-131">请求</span><span class="sxs-lookup"><span data-stu-id="4e7e1-131">Request</span></span>
<span data-ttu-id="4e7e1-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4e7e1-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="4e7e1-133">响应</span><span class="sxs-lookup"><span data-stu-id="4e7e1-133">Response</span></span>
<span data-ttu-id="4e7e1-134">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="4e7e1-134">Here is an example of the response.</span></span> <span data-ttu-id="4e7e1-135">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="4e7e1-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4e7e1-136">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="4e7e1-136">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



