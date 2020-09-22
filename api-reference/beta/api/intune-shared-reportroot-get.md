---
title: 获取 reportRoot
description: 读取 reportRoot 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9dffd70c71578a7f0acc97f03b0e73b1a73d2ead
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053795"
---
# <a name="get-reportroot"></a><span data-ttu-id="2829a-103">获取 reportRoot</span><span class="sxs-lookup"><span data-stu-id="2829a-103">Get reportRoot</span></span>

<span data-ttu-id="2829a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2829a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2829a-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2829a-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2829a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2829a-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2829a-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2829a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2829a-108">读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2829a-108">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2829a-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="2829a-109">Prerequisites</span></span>
<span data-ttu-id="2829a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2829a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2829a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="2829a-112">Permission type</span></span>|<span data-ttu-id="2829a-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2829a-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2829a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2829a-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2829a-115">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="2829a-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2829a-116">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2829a-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="2829a-117">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="2829a-117">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="2829a-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2829a-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2829a-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2829a-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2829a-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="2829a-120">Not supported.</span></span>|
|<span data-ttu-id="2829a-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="2829a-121">Application</span></span>||
| <span data-ttu-id="2829a-122">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="2829a-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2829a-123">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2829a-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="2829a-124">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="2829a-124">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="2829a-125">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2829a-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2829a-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2829a-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2829a-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2829a-127">Optional query parameters</span></span>
<span data-ttu-id="2829a-128">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2829a-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2829a-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="2829a-129">Request headers</span></span>
|<span data-ttu-id="2829a-130">标头</span><span class="sxs-lookup"><span data-stu-id="2829a-130">Header</span></span>|<span data-ttu-id="2829a-131">值</span><span class="sxs-lookup"><span data-stu-id="2829a-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2829a-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="2829a-132">Authorization</span></span>|<span data-ttu-id="2829a-133">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2829a-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2829a-134">接受</span><span class="sxs-lookup"><span data-stu-id="2829a-134">Accept</span></span>|<span data-ttu-id="2829a-135">application/json</span><span class="sxs-lookup"><span data-stu-id="2829a-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2829a-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="2829a-136">Request body</span></span>
<span data-ttu-id="2829a-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2829a-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2829a-138">响应</span><span class="sxs-lookup"><span data-stu-id="2829a-138">Response</span></span>
<span data-ttu-id="2829a-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [reportRoot](../resources/intune-shared-reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2829a-139">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2829a-140">示例</span><span class="sxs-lookup"><span data-stu-id="2829a-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="2829a-141">请求</span><span class="sxs-lookup"><span data-stu-id="2829a-141">Request</span></span>
<span data-ttu-id="2829a-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2829a-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="2829a-143">响应</span><span class="sxs-lookup"><span data-stu-id="2829a-143">Response</span></span>
<span data-ttu-id="2829a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2829a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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












