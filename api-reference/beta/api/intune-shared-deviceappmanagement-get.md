---
title: 获取 deviceAppManagement
description: 读取 deviceAppManagement 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 290a88af983f5c4b4bc6d032b8960c810960d969
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342712"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="6af98-103">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="6af98-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="6af98-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6af98-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6af98-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6af98-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6af98-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6af98-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6af98-107">读取 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6af98-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6af98-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6af98-108">Prerequisites</span></span>

<span data-ttu-id="6af98-109">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6af98-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6af98-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6af98-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="6af98-111">请注意，在相应权限根据工作流而有所不同。</span><span class="sxs-lookup"><span data-stu-id="6af98-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="6af98-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6af98-112">Permission type</span></span>|<span data-ttu-id="6af98-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6af98-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="6af98-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6af98-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="6af98-115">&nbsp;&nbsp; **应用程序**、**书籍**或**入职培训**</span><span class="sxs-lookup"><span data-stu-id="6af98-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="6af98-116">DeviceManagementApps.ReadWrite.All DeviceManagementApps.ReadW.All</span><span class="sxs-lookup"><span data-stu-id="6af98-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="6af98-117">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="6af98-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6af98-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6af98-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="6af98-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6af98-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6af98-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="6af98-120">Not supported.</span></span>|
|<span data-ttu-id="6af98-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="6af98-121">Application</span></span>|<span data-ttu-id="6af98-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="6af98-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6af98-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6af98-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6af98-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6af98-124">Optional query parameters</span></span>

<span data-ttu-id="6af98-125">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6af98-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6af98-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="6af98-126">Request headers</span></span>

|<span data-ttu-id="6af98-127">标头</span><span class="sxs-lookup"><span data-stu-id="6af98-127">Header</span></span>|<span data-ttu-id="6af98-128">值</span><span class="sxs-lookup"><span data-stu-id="6af98-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6af98-129">授权</span><span class="sxs-lookup"><span data-stu-id="6af98-129">Authorization</span></span>|<span data-ttu-id="6af98-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6af98-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6af98-131">Accept</span><span class="sxs-lookup"><span data-stu-id="6af98-131">Accept</span></span>|<span data-ttu-id="6af98-132">application/json</span><span class="sxs-lookup"><span data-stu-id="6af98-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6af98-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="6af98-133">Request body</span></span>

<span data-ttu-id="6af98-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6af98-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6af98-135">响应</span><span class="sxs-lookup"><span data-stu-id="6af98-135">Response</span></span>

<span data-ttu-id="6af98-136">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6af98-136">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6af98-137">示例</span><span class="sxs-lookup"><span data-stu-id="6af98-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6af98-138">请求</span><span class="sxs-lookup"><span data-stu-id="6af98-138">Request</span></span>

<span data-ttu-id="6af98-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6af98-139">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="6af98-140">响应</span><span class="sxs-lookup"><span data-stu-id="6af98-140">Response</span></span>

<span data-ttu-id="6af98-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6af98-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



