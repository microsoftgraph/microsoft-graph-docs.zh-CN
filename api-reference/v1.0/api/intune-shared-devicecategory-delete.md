---
title: 删除 deviceCategory
description: 删除 deviceCategory。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 43ceef30f28438c293ed8983ffc4748a4b54a2b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811149"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="a25bd-103">删除 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="a25bd-103">Delete deviceCategory</span></span>

> <span data-ttu-id="a25bd-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a25bd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a25bd-105">删除 [deviceCategory](../resources/intune-shared-devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="a25bd-105">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a25bd-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a25bd-106">Prerequisites</span></span>
<span data-ttu-id="a25bd-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a25bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a25bd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a25bd-109">Permission type</span></span>|<span data-ttu-id="a25bd-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a25bd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a25bd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a25bd-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a25bd-112">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="a25bd-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="a25bd-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a25bd-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a25bd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a25bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a25bd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a25bd-115">Not supported.</span></span>|
|<span data-ttu-id="a25bd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a25bd-116">Application</span></span>|<span data-ttu-id="a25bd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a25bd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a25bd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a25bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="a25bd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a25bd-119">Request headers</span></span>
|<span data-ttu-id="a25bd-120">标头</span><span class="sxs-lookup"><span data-stu-id="a25bd-120">Header</span></span>|<span data-ttu-id="a25bd-121">值</span><span class="sxs-lookup"><span data-stu-id="a25bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a25bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a25bd-122">Authorization</span></span>|<span data-ttu-id="a25bd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a25bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a25bd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a25bd-124">Accept</span></span>|<span data-ttu-id="a25bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a25bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a25bd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a25bd-126">Request body</span></span>
<span data-ttu-id="a25bd-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a25bd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a25bd-128">响应</span><span class="sxs-lookup"><span data-stu-id="a25bd-128">Response</span></span>
<span data-ttu-id="a25bd-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a25bd-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a25bd-130">示例</span><span class="sxs-lookup"><span data-stu-id="a25bd-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="a25bd-131">请求</span><span class="sxs-lookup"><span data-stu-id="a25bd-131">Request</span></span>
<span data-ttu-id="a25bd-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a25bd-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="a25bd-133">响应</span><span class="sxs-lookup"><span data-stu-id="a25bd-133">Response</span></span>
<span data-ttu-id="a25bd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a25bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



