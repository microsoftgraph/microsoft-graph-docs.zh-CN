---
title: 获取 deviceAppManagement
description: 读取 deviceAppManagement 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6f4ce05f838b88bbe2f930557b4e2384347be4ac
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086261"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="c5437-103">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="c5437-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="c5437-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c5437-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c5437-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c5437-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5437-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5437-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5437-107">读取 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c5437-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5437-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c5437-108">Prerequisites</span></span>

<span data-ttu-id="c5437-109">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="c5437-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c5437-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5437-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="c5437-111">请注意，相应的权限根据工作流的不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="c5437-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="c5437-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5437-112">Permission type</span></span>|<span data-ttu-id="c5437-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c5437-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="c5437-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5437-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="c5437-115">&nbsp;&nbsp; **应用**、**图书**、**加入**、**合作伙伴集成**或**策略集**</span><span class="sxs-lookup"><span data-stu-id="c5437-115">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="c5437-116">Devicemanagementapps.readwrite.all、Devicemanagementapps.readwrite.all 和所有 ReadW</span><span class="sxs-lookup"><span data-stu-id="c5437-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="c5437-117">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="c5437-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c5437-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5437-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="c5437-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5437-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5437-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5437-120">Not supported.</span></span>|
|<span data-ttu-id="c5437-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5437-121">Application</span></span>| |
| <span data-ttu-id="c5437-122">&nbsp;&nbsp; **应用**、**图书**、**加入**、**合作伙伴集成**或**策略集**</span><span class="sxs-lookup"><span data-stu-id="c5437-122">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="c5437-123">Devicemanagementapps.readwrite.all、Devicemanagementapps.readwrite.all 和所有 ReadW</span><span class="sxs-lookup"><span data-stu-id="c5437-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="c5437-124">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="c5437-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c5437-125">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5437-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5437-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5437-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5437-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c5437-127">Optional query parameters</span></span>

<span data-ttu-id="c5437-128">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c5437-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5437-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5437-129">Request headers</span></span>

|<span data-ttu-id="c5437-130">标头</span><span class="sxs-lookup"><span data-stu-id="c5437-130">Header</span></span>|<span data-ttu-id="c5437-131">值</span><span class="sxs-lookup"><span data-stu-id="c5437-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5437-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5437-132">Authorization</span></span>|<span data-ttu-id="c5437-133">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c5437-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5437-134">接受</span><span class="sxs-lookup"><span data-stu-id="c5437-134">Accept</span></span>|<span data-ttu-id="c5437-135">application/json</span><span class="sxs-lookup"><span data-stu-id="c5437-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5437-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5437-136">Request body</span></span>

<span data-ttu-id="c5437-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5437-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5437-138">响应</span><span class="sxs-lookup"><span data-stu-id="c5437-138">Response</span></span>

<span data-ttu-id="c5437-139">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c5437-139">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5437-140">示例</span><span class="sxs-lookup"><span data-stu-id="c5437-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5437-141">请求</span><span class="sxs-lookup"><span data-stu-id="c5437-141">Request</span></span>

<span data-ttu-id="c5437-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5437-142">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="c5437-143">响应</span><span class="sxs-lookup"><span data-stu-id="c5437-143">Response</span></span>

<span data-ttu-id="c5437-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5437-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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












