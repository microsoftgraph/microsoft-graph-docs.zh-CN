---
title: 删除 telecomExpenseManagementPartner
description: 删除 telecomExpenseManagementPartner。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bf6ce155d649162d8e12f07bd5be3fa1f9c018d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407310"
---
# <a name="delete-telecomexpensemanagementpartner"></a><span data-ttu-id="fcaae-103">删除 telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="fcaae-103">Delete telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="fcaae-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="fcaae-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fcaae-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fcaae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fcaae-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fcaae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcaae-107">删除 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="fcaae-107">Deletes a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcaae-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fcaae-108">Prerequisites</span></span>
<span data-ttu-id="fcaae-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fcaae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fcaae-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fcaae-111">Permission type</span></span>|<span data-ttu-id="fcaae-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fcaae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcaae-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fcaae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fcaae-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcaae-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fcaae-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fcaae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcaae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fcaae-116">Not supported.</span></span>|
|<span data-ttu-id="fcaae-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fcaae-117">Application</span></span>|<span data-ttu-id="fcaae-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fcaae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcaae-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fcaae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="fcaae-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fcaae-120">Request headers</span></span>
|<span data-ttu-id="fcaae-121">标头</span><span class="sxs-lookup"><span data-stu-id="fcaae-121">Header</span></span>|<span data-ttu-id="fcaae-122">值</span><span class="sxs-lookup"><span data-stu-id="fcaae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcaae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcaae-123">Authorization</span></span>|<span data-ttu-id="fcaae-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fcaae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcaae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fcaae-125">Accept</span></span>|<span data-ttu-id="fcaae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fcaae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcaae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fcaae-127">Request body</span></span>
<span data-ttu-id="fcaae-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fcaae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcaae-129">响应</span><span class="sxs-lookup"><span data-stu-id="fcaae-129">Response</span></span>
<span data-ttu-id="fcaae-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="fcaae-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fcaae-131">示例</span><span class="sxs-lookup"><span data-stu-id="fcaae-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcaae-132">请求</span><span class="sxs-lookup"><span data-stu-id="fcaae-132">Request</span></span>
<span data-ttu-id="fcaae-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fcaae-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="fcaae-134">响应</span><span class="sxs-lookup"><span data-stu-id="fcaae-134">Response</span></span>
<span data-ttu-id="fcaae-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fcaae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




