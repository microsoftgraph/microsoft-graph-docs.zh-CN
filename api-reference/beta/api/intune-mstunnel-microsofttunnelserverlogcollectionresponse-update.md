---
title: 更新 microsoftTunnelServerLogCollectionResponse
description: 更新 microsoftTunnelServerLogCollectionResponse 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 257bfd68d719dbf22f04f946a3720304142ca112
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162216"
---
# <a name="update-microsofttunnelserverlogcollectionresponse"></a><span data-ttu-id="b316b-103">更新 microsoftTunnelServerLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="b316b-103">Update microsoftTunnelServerLogCollectionResponse</span></span>

<span data-ttu-id="b316b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b316b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b316b-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b316b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b316b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b316b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b316b-107">更新 [microsoftTunnelServerLogCollectionResponse 对象](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="b316b-107">Update the properties of a [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b316b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b316b-108">Prerequisites</span></span>
<span data-ttu-id="b316b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b316b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b316b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b316b-111">Permission type</span></span>|<span data-ttu-id="b316b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b316b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b316b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b316b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b316b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b316b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b316b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b316b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b316b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b316b-116">Not supported.</span></span>|
|<span data-ttu-id="b316b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b316b-117">Application</span></span>|<span data-ttu-id="b316b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b316b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b316b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b316b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelServerLogCollectionResponses/{microsoftTunnelServerLogCollectionResponseId}
```

## <a name="request-headers"></a><span data-ttu-id="b316b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b316b-120">Request headers</span></span>
|<span data-ttu-id="b316b-121">标头</span><span class="sxs-lookup"><span data-stu-id="b316b-121">Header</span></span>|<span data-ttu-id="b316b-122">值</span><span class="sxs-lookup"><span data-stu-id="b316b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b316b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b316b-123">Authorization</span></span>|<span data-ttu-id="b316b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b316b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b316b-125">接受</span><span class="sxs-lookup"><span data-stu-id="b316b-125">Accept</span></span>|<span data-ttu-id="b316b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b316b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b316b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b316b-127">Request body</span></span>
<span data-ttu-id="b316b-128">在请求正文中，提供 [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b316b-128">In the request body, supply a JSON representation for the [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object.</span></span>

<span data-ttu-id="b316b-129">下表显示创建 [microsoftTunnelServerLogCollectionResponse 时所需的属性](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)。</span><span class="sxs-lookup"><span data-stu-id="b316b-129">The following table shows the properties that are required when you create the [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md).</span></span>

|<span data-ttu-id="b316b-130">属性</span><span class="sxs-lookup"><span data-stu-id="b316b-130">Property</span></span>|<span data-ttu-id="b316b-131">类型</span><span class="sxs-lookup"><span data-stu-id="b316b-131">Type</span></span>|<span data-ttu-id="b316b-132">说明</span><span class="sxs-lookup"><span data-stu-id="b316b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b316b-133">id</span><span class="sxs-lookup"><span data-stu-id="b316b-133">id</span></span>|<span data-ttu-id="b316b-134">String</span><span class="sxs-lookup"><span data-stu-id="b316b-134">String</span></span>|<span data-ttu-id="b316b-135">实体的唯一 ID</span><span class="sxs-lookup"><span data-stu-id="b316b-135">The unique ID of the entity</span></span>|
|<span data-ttu-id="b316b-136">status</span><span class="sxs-lookup"><span data-stu-id="b316b-136">status</span></span>|[<span data-ttu-id="b316b-137">microsoftTunnelLogCollectionStatus</span><span class="sxs-lookup"><span data-stu-id="b316b-137">microsoftTunnelLogCollectionStatus</span></span>](../resources/intune-mstunnel-microsofttunnellogcollectionstatus.md)|<span data-ttu-id="b316b-138">日志集合的状态。</span><span class="sxs-lookup"><span data-stu-id="b316b-138">The status of log collection.</span></span> <span data-ttu-id="b316b-139">可取值为：`pending`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b316b-139">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="b316b-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b316b-140">startDateTime</span></span>|<span data-ttu-id="b316b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b316b-141">DateTimeOffset</span></span>|<span data-ttu-id="b316b-142">收集的日志的开始时间</span><span class="sxs-lookup"><span data-stu-id="b316b-142">The start time of the logs collected</span></span> |
|<span data-ttu-id="b316b-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b316b-143">endDateTime</span></span>|<span data-ttu-id="b316b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b316b-144">DateTimeOffset</span></span>|<span data-ttu-id="b316b-145">收集的日志的结束时间</span><span class="sxs-lookup"><span data-stu-id="b316b-145">The end time of the logs collected</span></span>|
|<span data-ttu-id="b316b-146">sizeInBytes</span><span class="sxs-lookup"><span data-stu-id="b316b-146">sizeInBytes</span></span>|<span data-ttu-id="b316b-147">Int64</span><span class="sxs-lookup"><span data-stu-id="b316b-147">Int64</span></span>|<span data-ttu-id="b316b-148">日志的大小（以字节为单位）</span><span class="sxs-lookup"><span data-stu-id="b316b-148">The size of the logs in bytes</span></span>|



## <a name="response"></a><span data-ttu-id="b316b-149">响应</span><span class="sxs-lookup"><span data-stu-id="b316b-149">Response</span></span>
<span data-ttu-id="b316b-150">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b316b-150">If successful, this method returns a `200 OK` response code and an updated [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b316b-151">示例</span><span class="sxs-lookup"><span data-stu-id="b316b-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="b316b-152">请求</span><span class="sxs-lookup"><span data-stu-id="b316b-152">Request</span></span>
<span data-ttu-id="b316b-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b316b-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelServerLogCollectionResponses/{microsoftTunnelServerLogCollectionResponseId}
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
  "status": "completed",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "sizeInBytes": 11
}
```

### <a name="response"></a><span data-ttu-id="b316b-154">响应</span><span class="sxs-lookup"><span data-stu-id="b316b-154">Response</span></span>
<span data-ttu-id="b316b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b316b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 293

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
  "id": "05dcc2e9-c2e9-05dc-e9c2-dc05e9c2dc05",
  "status": "completed",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "sizeInBytes": 11
}
```




