---
title: 获取 deviceAppManagement
description: 读取 deviceAppManagement 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c27099cdc0e2ffbbc3e0e02cde07b9b4e34ea33c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408311"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="6ac7e-103">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="6ac7e-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="6ac7e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6ac7e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ac7e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ac7e-107">读取 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ac7e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6ac7e-108">Prerequisites</span></span>

<span data-ttu-id="6ac7e-109">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6ac7e-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="6ac7e-111">请注意，在相应权限根据工作流而有所不同。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="6ac7e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ac7e-112">Permission type</span></span>|<span data-ttu-id="6ac7e-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6ac7e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="6ac7e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ac7e-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="6ac7e-115">&nbsp;&nbsp; **应用程序**、**书籍**或**入职培训**</span><span class="sxs-lookup"><span data-stu-id="6ac7e-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="6ac7e-116">DeviceManagementApps.ReadWrite.All DeviceManagementApps.ReadW.All</span><span class="sxs-lookup"><span data-stu-id="6ac7e-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="6ac7e-117">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="6ac7e-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6ac7e-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ac7e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="6ac7e-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ac7e-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ac7e-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-120">Not supported.</span></span>|
|<span data-ttu-id="6ac7e-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ac7e-121">Application</span></span>|<span data-ttu-id="6ac7e-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ac7e-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ac7e-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ac7e-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6ac7e-124">Optional query parameters</span></span>

<span data-ttu-id="6ac7e-125">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ac7e-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ac7e-126">Request headers</span></span>

|<span data-ttu-id="6ac7e-127">标头</span><span class="sxs-lookup"><span data-stu-id="6ac7e-127">Header</span></span>|<span data-ttu-id="6ac7e-128">值</span><span class="sxs-lookup"><span data-stu-id="6ac7e-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ac7e-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ac7e-129">Authorization</span></span>|<span data-ttu-id="6ac7e-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ac7e-131">Accept</span><span class="sxs-lookup"><span data-stu-id="6ac7e-131">Accept</span></span>|<span data-ttu-id="6ac7e-132">application/json</span><span class="sxs-lookup"><span data-stu-id="6ac7e-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ac7e-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ac7e-133">Request body</span></span>

<span data-ttu-id="6ac7e-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ac7e-135">响应</span><span class="sxs-lookup"><span data-stu-id="6ac7e-135">Response</span></span>

<span data-ttu-id="6ac7e-136">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-136">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ac7e-137">示例</span><span class="sxs-lookup"><span data-stu-id="6ac7e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ac7e-138">请求</span><span class="sxs-lookup"><span data-stu-id="6ac7e-138">Request</span></span>

<span data-ttu-id="6ac7e-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-139">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="6ac7e-140">响应</span><span class="sxs-lookup"><span data-stu-id="6ac7e-140">Response</span></span>

<span data-ttu-id="6ac7e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6ac7e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



