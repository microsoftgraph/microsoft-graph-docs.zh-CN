---
title: 获取 deviceAppManagement
description: 读取 deviceAppManagement 对象的属性和关系。
ms.openlocfilehash: b73e616735ca3f096c01a9f7eba8a7d751bb7160
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042669"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="8864c-103">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="8864c-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="8864c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8864c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8864c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8864c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8864c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8864c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8864c-107">读取 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8864c-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8864c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8864c-108">Prerequisites</span></span>

<span data-ttu-id="8864c-109">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8864c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8864c-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8864c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="8864c-111">请注意，在相应权限根据工作流而有所不同。</span><span class="sxs-lookup"><span data-stu-id="8864c-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="8864c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8864c-112">Permission type</span></span>|<span data-ttu-id="8864c-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8864c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="8864c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8864c-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="8864c-115">&nbsp;&nbsp; **应用程序**、**书籍**或**入职培训**</span><span class="sxs-lookup"><span data-stu-id="8864c-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="8864c-116">DeviceManagementApps.ReadWrite.All DeviceManagementApps.ReadW.All</span><span class="sxs-lookup"><span data-stu-id="8864c-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="8864c-117">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="8864c-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8864c-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8864c-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="8864c-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8864c-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8864c-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="8864c-120">Not supported.</span></span>|
|<span data-ttu-id="8864c-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="8864c-121">Application</span></span>|<span data-ttu-id="8864c-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="8864c-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8864c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8864c-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8864c-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8864c-124">Optional query parameters</span></span>

<span data-ttu-id="8864c-125">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8864c-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8864c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="8864c-126">Request headers</span></span>

|<span data-ttu-id="8864c-127">标头</span><span class="sxs-lookup"><span data-stu-id="8864c-127">Header</span></span>|<span data-ttu-id="8864c-128">值</span><span class="sxs-lookup"><span data-stu-id="8864c-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8864c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8864c-129">Authorization</span></span>|<span data-ttu-id="8864c-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8864c-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8864c-131">Accept</span><span class="sxs-lookup"><span data-stu-id="8864c-131">Accept</span></span>|<span data-ttu-id="8864c-132">application/json</span><span class="sxs-lookup"><span data-stu-id="8864c-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8864c-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="8864c-133">Request body</span></span>

<span data-ttu-id="8864c-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8864c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8864c-135">响应</span><span class="sxs-lookup"><span data-stu-id="8864c-135">Response</span></span>

<span data-ttu-id="8864c-136">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8864c-136">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8864c-137">示例</span><span class="sxs-lookup"><span data-stu-id="8864c-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="8864c-138">请求</span><span class="sxs-lookup"><span data-stu-id="8864c-138">Request</span></span>

<span data-ttu-id="8864c-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8864c-139">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="8864c-140">响应</span><span class="sxs-lookup"><span data-stu-id="8864c-140">Response</span></span>

<span data-ttu-id="8864c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8864c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



