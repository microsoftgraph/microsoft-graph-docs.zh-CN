---
title: 获取 reportRoot
description: 读取 reportRoot 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3eb399f31ab00ae0dd4fd6f229871248ec2ad1ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458201"
---
# <a name="get-reportroot"></a><span data-ttu-id="4aeec-103">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="4aeec-103">Get reportRoot</span></span>

<span data-ttu-id="4aeec-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4aeec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4aeec-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4aeec-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4aeec-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4aeec-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4aeec-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4aeec-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4aeec-108">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4aeec-108">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4aeec-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="4aeec-109">Prerequisites</span></span>
<span data-ttu-id="4aeec-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4aeec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4aeec-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4aeec-112">Permission type</span></span>|<span data-ttu-id="4aeec-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4aeec-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4aeec-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4aeec-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4aeec-115">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="4aeec-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4aeec-116">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4aeec-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="4aeec-117">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="4aeec-117">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="4aeec-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4aeec-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4aeec-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4aeec-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4aeec-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="4aeec-120">Not supported.</span></span>|
|<span data-ttu-id="4aeec-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="4aeec-121">Application</span></span>||
| <span data-ttu-id="4aeec-122">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="4aeec-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4aeec-123">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4aeec-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="4aeec-124">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="4aeec-124">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="4aeec-125">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4aeec-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4aeec-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4aeec-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4aeec-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4aeec-127">Optional query parameters</span></span>
<span data-ttu-id="4aeec-128">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4aeec-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4aeec-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="4aeec-129">Request headers</span></span>
|<span data-ttu-id="4aeec-130">标头</span><span class="sxs-lookup"><span data-stu-id="4aeec-130">Header</span></span>|<span data-ttu-id="4aeec-131">值</span><span class="sxs-lookup"><span data-stu-id="4aeec-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4aeec-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aeec-132">Authorization</span></span>|<span data-ttu-id="4aeec-133">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4aeec-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4aeec-134">接受</span><span class="sxs-lookup"><span data-stu-id="4aeec-134">Accept</span></span>|<span data-ttu-id="4aeec-135">application/json</span><span class="sxs-lookup"><span data-stu-id="4aeec-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4aeec-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="4aeec-136">Request body</span></span>
<span data-ttu-id="4aeec-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4aeec-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4aeec-138">响应</span><span class="sxs-lookup"><span data-stu-id="4aeec-138">Response</span></span>
<span data-ttu-id="4aeec-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4aeec-139">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4aeec-140">示例</span><span class="sxs-lookup"><span data-stu-id="4aeec-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="4aeec-141">请求</span><span class="sxs-lookup"><span data-stu-id="4aeec-141">Request</span></span>
<span data-ttu-id="4aeec-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4aeec-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="4aeec-143">响应</span><span class="sxs-lookup"><span data-stu-id="4aeec-143">Response</span></span>
<span data-ttu-id="4aeec-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4aeec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```











