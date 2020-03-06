---
title: 删除 deviceCategory
description: 删除 deviceCategory。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1123153dc864717489e49cf0f62a315cd94a390e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512102"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="37674-103">删除 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="37674-103">Delete deviceCategory</span></span>

<span data-ttu-id="37674-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37674-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37674-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="37674-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37674-106">删除 [deviceCategory](../resources/intune-shared-devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="37674-106">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37674-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="37674-107">Prerequisites</span></span>
<span data-ttu-id="37674-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37674-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37674-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="37674-110">Permission type</span></span>|<span data-ttu-id="37674-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="37674-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37674-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37674-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="37674-113">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="37674-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="37674-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37674-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="37674-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37674-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37674-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="37674-116">Not supported.</span></span>|
|<span data-ttu-id="37674-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="37674-117">Application</span></span>|<span data-ttu-id="37674-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="37674-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37674-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37674-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="37674-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="37674-120">Request headers</span></span>
|<span data-ttu-id="37674-121">标头</span><span class="sxs-lookup"><span data-stu-id="37674-121">Header</span></span>|<span data-ttu-id="37674-122">值</span><span class="sxs-lookup"><span data-stu-id="37674-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37674-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37674-123">Authorization</span></span>|<span data-ttu-id="37674-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="37674-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37674-125">接受</span><span class="sxs-lookup"><span data-stu-id="37674-125">Accept</span></span>|<span data-ttu-id="37674-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37674-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37674-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="37674-127">Request body</span></span>
<span data-ttu-id="37674-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="37674-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37674-129">响应</span><span class="sxs-lookup"><span data-stu-id="37674-129">Response</span></span>
<span data-ttu-id="37674-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="37674-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="37674-131">示例</span><span class="sxs-lookup"><span data-stu-id="37674-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="37674-132">请求</span><span class="sxs-lookup"><span data-stu-id="37674-132">Request</span></span>
<span data-ttu-id="37674-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="37674-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="37674-134">响应</span><span class="sxs-lookup"><span data-stu-id="37674-134">Response</span></span>
<span data-ttu-id="37674-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="37674-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




