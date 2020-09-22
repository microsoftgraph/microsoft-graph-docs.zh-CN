---
title: 列出 deviceCategories
description: 列出 deviceCategory 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c2eb8250715686fc427bfe82510eb984aa683235
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980377"
---
# <a name="list-devicecategories"></a><span data-ttu-id="e039c-103">列出 deviceCategories</span><span class="sxs-lookup"><span data-stu-id="e039c-103">List deviceCategories</span></span>

<span data-ttu-id="e039c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e039c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e039c-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e039c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e039c-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e039c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e039c-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e039c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e039c-108">列出 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e039c-108">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e039c-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="e039c-109">Prerequisites</span></span>
<span data-ttu-id="e039c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e039c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e039c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e039c-112">Permission type</span></span>|<span data-ttu-id="e039c-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e039c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e039c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e039c-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e039c-115">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="e039c-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e039c-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e039c-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e039c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e039c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e039c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e039c-118">Not supported.</span></span>|
|<span data-ttu-id="e039c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e039c-119">Application</span></span>||
| <span data-ttu-id="e039c-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="e039c-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e039c-121">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e039c-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e039c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e039c-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="e039c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e039c-123">Request headers</span></span>

|<span data-ttu-id="e039c-124">标头</span><span class="sxs-lookup"><span data-stu-id="e039c-124">Header</span></span>|<span data-ttu-id="e039c-125">值</span><span class="sxs-lookup"><span data-stu-id="e039c-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e039c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e039c-126">Authorization</span></span>|<span data-ttu-id="e039c-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e039c-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e039c-128">接受</span><span class="sxs-lookup"><span data-stu-id="e039c-128">Accept</span></span>|<span data-ttu-id="e039c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e039c-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e039c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e039c-130">Request body</span></span>

<span data-ttu-id="e039c-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e039c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e039c-132">响应</span><span class="sxs-lookup"><span data-stu-id="e039c-132">Response</span></span>

<span data-ttu-id="e039c-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e039c-133">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e039c-134">示例</span><span class="sxs-lookup"><span data-stu-id="e039c-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="e039c-135">请求</span><span class="sxs-lookup"><span data-stu-id="e039c-135">Request</span></span>

<span data-ttu-id="e039c-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e039c-136">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="e039c-137">响应</span><span class="sxs-lookup"><span data-stu-id="e039c-137">Response</span></span>

<span data-ttu-id="e039c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e039c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCategory",
      "id": "f881b841-b841-f881-41b8-81f841b881f8",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```












