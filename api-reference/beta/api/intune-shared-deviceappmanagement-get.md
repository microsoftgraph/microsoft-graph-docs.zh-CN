---
title: 获取 deviceAppManagement
description: 读取 deviceAppManagement 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 787003853684855bef7b42bb8940ed248cb322c1
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537125"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="5fe96-103">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="5fe96-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="5fe96-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5fe96-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5fe96-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5fe96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5fe96-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5fe96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fe96-107">读取 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5fe96-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fe96-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5fe96-108">Prerequisites</span></span>

<span data-ttu-id="5fe96-109">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="5fe96-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5fe96-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5fe96-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="5fe96-111">请注意，相应的权限根据工作流的不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="5fe96-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="5fe96-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5fe96-112">Permission type</span></span>|<span data-ttu-id="5fe96-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5fe96-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="5fe96-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5fe96-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="5fe96-115">&nbsp;&nbsp; **应用**、**图书**、**加入**、**合作伙伴集成**或**策略集**</span><span class="sxs-lookup"><span data-stu-id="5fe96-115">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="5fe96-116">Devicemanagementapps.readwrite.all、Devicemanagementapps.readwrite.all 和所有 ReadW</span><span class="sxs-lookup"><span data-stu-id="5fe96-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="5fe96-117">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="5fe96-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5fe96-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5fe96-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="5fe96-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5fe96-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fe96-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fe96-120">Not supported.</span></span>|
|<span data-ttu-id="5fe96-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="5fe96-121">Application</span></span>| |
| <span data-ttu-id="5fe96-122">&nbsp;&nbsp; **应用**、**图书**、**加入**、**合作伙伴集成**或**策略集**</span><span class="sxs-lookup"><span data-stu-id="5fe96-122">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="5fe96-123">Devicemanagementapps.readwrite.all、Devicemanagementapps.readwrite.all 和所有 ReadW</span><span class="sxs-lookup"><span data-stu-id="5fe96-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="5fe96-124">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="5fe96-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5fe96-125">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5fe96-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fe96-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5fe96-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5fe96-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5fe96-127">Optional query parameters</span></span>

<span data-ttu-id="5fe96-128">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5fe96-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5fe96-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="5fe96-129">Request headers</span></span>

|<span data-ttu-id="5fe96-130">标头</span><span class="sxs-lookup"><span data-stu-id="5fe96-130">Header</span></span>|<span data-ttu-id="5fe96-131">值</span><span class="sxs-lookup"><span data-stu-id="5fe96-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fe96-132">授权</span><span class="sxs-lookup"><span data-stu-id="5fe96-132">Authorization</span></span>|<span data-ttu-id="5fe96-133">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5fe96-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fe96-134">接受</span><span class="sxs-lookup"><span data-stu-id="5fe96-134">Accept</span></span>|<span data-ttu-id="5fe96-135">application/json</span><span class="sxs-lookup"><span data-stu-id="5fe96-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fe96-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="5fe96-136">Request body</span></span>

<span data-ttu-id="5fe96-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5fe96-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fe96-138">响应</span><span class="sxs-lookup"><span data-stu-id="5fe96-138">Response</span></span>

<span data-ttu-id="5fe96-139">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5fe96-139">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fe96-140">示例</span><span class="sxs-lookup"><span data-stu-id="5fe96-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fe96-141">请求</span><span class="sxs-lookup"><span data-stu-id="5fe96-141">Request</span></span>

<span data-ttu-id="5fe96-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5fe96-142">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="5fe96-143">响应</span><span class="sxs-lookup"><span data-stu-id="5fe96-143">Response</span></span>

<span data-ttu-id="5fe96-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5fe96-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









