---
title: 更新 ndesConnector
description: 更新 ndesConnector 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e1694a163742b63df535744b43b33e3fc2ca9d65
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054502"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="ca3a9-103">更新 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="ca3a9-103">Update ndesConnector</span></span>

<span data-ttu-id="ca3a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca3a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca3a9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca3a9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca3a9-107">更新 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-107">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca3a9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca3a9-108">Prerequisites</span></span>
<span data-ttu-id="ca3a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca3a9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca3a9-111">Permission type</span></span>|<span data-ttu-id="ca3a9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ca3a9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca3a9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca3a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca3a9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca3a9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca3a9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca3a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca3a9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-116">Not supported.</span></span>|
|<span data-ttu-id="ca3a9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca3a9-117">Application</span></span>|<span data-ttu-id="ca3a9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca3a9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca3a9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca3a9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="ca3a9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca3a9-120">Request headers</span></span>
|<span data-ttu-id="ca3a9-121">标头</span><span class="sxs-lookup"><span data-stu-id="ca3a9-121">Header</span></span>|<span data-ttu-id="ca3a9-122">值</span><span class="sxs-lookup"><span data-stu-id="ca3a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca3a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca3a9-123">Authorization</span></span>|<span data-ttu-id="ca3a9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca3a9-125">接受</span><span class="sxs-lookup"><span data-stu-id="ca3a9-125">Accept</span></span>|<span data-ttu-id="ca3a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca3a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca3a9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca3a9-127">Request body</span></span>
<span data-ttu-id="ca3a9-128">在请求正文中，提供 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-128">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="ca3a9-129">下表显示创建 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-129">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="ca3a9-130">属性</span><span class="sxs-lookup"><span data-stu-id="ca3a9-130">Property</span></span>|<span data-ttu-id="ca3a9-131">类型</span><span class="sxs-lookup"><span data-stu-id="ca3a9-131">Type</span></span>|<span data-ttu-id="ca3a9-132">说明</span><span class="sxs-lookup"><span data-stu-id="ca3a9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca3a9-133">id</span><span class="sxs-lookup"><span data-stu-id="ca3a9-133">id</span></span>|<span data-ttu-id="ca3a9-134">String</span><span class="sxs-lookup"><span data-stu-id="ca3a9-134">String</span></span>|<span data-ttu-id="ca3a9-135">NDES 连接器的键。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="ca3a9-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="ca3a9-136">lastConnectionDateTime</span></span>|<span data-ttu-id="ca3a9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca3a9-137">DateTimeOffset</span></span>|<span data-ttu-id="ca3a9-138">Ndes 连接器的上次连接时间</span><span class="sxs-lookup"><span data-stu-id="ca3a9-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="ca3a9-139">state</span><span class="sxs-lookup"><span data-stu-id="ca3a9-139">state</span></span>|[<span data-ttu-id="ca3a9-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="ca3a9-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="ca3a9-141">Ndes 连接器状态。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-141">Ndes Connector Status.</span></span> <span data-ttu-id="ca3a9-142">可取值为：`none`、`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="ca3a9-143">displayName</span><span class="sxs-lookup"><span data-stu-id="ca3a9-143">displayName</span></span>|<span data-ttu-id="ca3a9-144">String</span><span class="sxs-lookup"><span data-stu-id="ca3a9-144">String</span></span>|<span data-ttu-id="ca3a9-145">Ndes 连接器的友好名称。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="ca3a9-146">响应</span><span class="sxs-lookup"><span data-stu-id="ca3a9-146">Response</span></span>
<span data-ttu-id="ca3a9-147">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-147">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca3a9-148">示例</span><span class="sxs-lookup"><span data-stu-id="ca3a9-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca3a9-149">请求</span><span class="sxs-lookup"><span data-stu-id="ca3a9-149">Request</span></span>
<span data-ttu-id="ca3a9-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="ca3a9-151">响应</span><span class="sxs-lookup"><span data-stu-id="ca3a9-151">Response</span></span>
<span data-ttu-id="ca3a9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca3a9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```






