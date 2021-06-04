---
title: 删除 deviceCategory
description: 删除 deviceCategory。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bd38e1eb6f732db629a6c88a9a4a36e0357431df
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732389"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="3ed8c-103">删除 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="3ed8c-103">Delete deviceCategory</span></span>

<span data-ttu-id="3ed8c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ed8c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ed8c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ed8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ed8c-106">删除 [deviceCategory](../resources/intune-shared-devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="3ed8c-106">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ed8c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3ed8c-107">Prerequisites</span></span>
<span data-ttu-id="3ed8c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ed8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ed8c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ed8c-110">Permission type</span></span>|<span data-ttu-id="3ed8c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3ed8c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ed8c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ed8c-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3ed8c-113">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="3ed8c-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="3ed8c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ed8c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3ed8c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ed8c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ed8c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ed8c-116">Not supported.</span></span>|
|<span data-ttu-id="3ed8c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ed8c-117">Application</span></span>|<span data-ttu-id="3ed8c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ed8c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ed8c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ed8c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="3ed8c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ed8c-120">Request headers</span></span>
|<span data-ttu-id="3ed8c-121">标头</span><span class="sxs-lookup"><span data-stu-id="3ed8c-121">Header</span></span>|<span data-ttu-id="3ed8c-122">值</span><span class="sxs-lookup"><span data-stu-id="3ed8c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ed8c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ed8c-123">Authorization</span></span>|<span data-ttu-id="3ed8c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3ed8c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ed8c-125">接受</span><span class="sxs-lookup"><span data-stu-id="3ed8c-125">Accept</span></span>|<span data-ttu-id="3ed8c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ed8c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ed8c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ed8c-127">Request body</span></span>
<span data-ttu-id="3ed8c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ed8c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ed8c-129">响应</span><span class="sxs-lookup"><span data-stu-id="3ed8c-129">Response</span></span>
<span data-ttu-id="3ed8c-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3ed8c-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3ed8c-131">示例</span><span class="sxs-lookup"><span data-stu-id="3ed8c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3ed8c-132">请求</span><span class="sxs-lookup"><span data-stu-id="3ed8c-132">Request</span></span>
<span data-ttu-id="3ed8c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ed8c-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="3ed8c-134">响应</span><span class="sxs-lookup"><span data-stu-id="3ed8c-134">Response</span></span>
<span data-ttu-id="3ed8c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3ed8c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









