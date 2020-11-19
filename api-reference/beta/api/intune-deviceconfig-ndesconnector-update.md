---
title: 更新 ndesConnector
description: 更新 ndesConnector 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ef715625dbcd8779280ac2165b25dc2b8edda34d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49270930"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="8c581-103">更新 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="8c581-103">Update ndesConnector</span></span>

<span data-ttu-id="8c581-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c581-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c581-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c581-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c581-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c581-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c581-107">更新 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8c581-107">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c581-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c581-108">Prerequisites</span></span>
<span data-ttu-id="8c581-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c581-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c581-111">Permission type</span></span>|<span data-ttu-id="8c581-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8c581-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c581-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c581-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c581-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c581-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c581-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c581-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c581-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c581-116">Not supported.</span></span>|
|<span data-ttu-id="8c581-117">Application</span><span class="sxs-lookup"><span data-stu-id="8c581-117">Application</span></span>|<span data-ttu-id="8c581-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c581-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c581-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c581-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="8c581-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c581-120">Request headers</span></span>
|<span data-ttu-id="8c581-121">标头</span><span class="sxs-lookup"><span data-stu-id="8c581-121">Header</span></span>|<span data-ttu-id="8c581-122">值</span><span class="sxs-lookup"><span data-stu-id="8c581-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c581-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c581-123">Authorization</span></span>|<span data-ttu-id="8c581-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c581-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c581-125">接受</span><span class="sxs-lookup"><span data-stu-id="8c581-125">Accept</span></span>|<span data-ttu-id="8c581-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c581-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c581-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c581-127">Request body</span></span>
<span data-ttu-id="8c581-128">在请求正文中，提供 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c581-128">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="8c581-129">下表显示创建 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8c581-129">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="8c581-130">属性</span><span class="sxs-lookup"><span data-stu-id="8c581-130">Property</span></span>|<span data-ttu-id="8c581-131">类型</span><span class="sxs-lookup"><span data-stu-id="8c581-131">Type</span></span>|<span data-ttu-id="8c581-132">说明</span><span class="sxs-lookup"><span data-stu-id="8c581-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c581-133">id</span><span class="sxs-lookup"><span data-stu-id="8c581-133">id</span></span>|<span data-ttu-id="8c581-134">字符串</span><span class="sxs-lookup"><span data-stu-id="8c581-134">String</span></span>|<span data-ttu-id="8c581-135">NDES 连接器的键。</span><span class="sxs-lookup"><span data-stu-id="8c581-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="8c581-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="8c581-136">lastConnectionDateTime</span></span>|<span data-ttu-id="8c581-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c581-137">DateTimeOffset</span></span>|<span data-ttu-id="8c581-138">Ndes 连接器的上次连接时间</span><span class="sxs-lookup"><span data-stu-id="8c581-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="8c581-139">state</span><span class="sxs-lookup"><span data-stu-id="8c581-139">state</span></span>|[<span data-ttu-id="8c581-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="8c581-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="8c581-141">Ndes 连接器状态。</span><span class="sxs-lookup"><span data-stu-id="8c581-141">Ndes Connector Status.</span></span> <span data-ttu-id="8c581-142">可取值为：`none`、`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="8c581-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="8c581-143">displayName</span><span class="sxs-lookup"><span data-stu-id="8c581-143">displayName</span></span>|<span data-ttu-id="8c581-144">字符串</span><span class="sxs-lookup"><span data-stu-id="8c581-144">String</span></span>|<span data-ttu-id="8c581-145">Ndes 连接器的友好名称。</span><span class="sxs-lookup"><span data-stu-id="8c581-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="8c581-146">响应</span><span class="sxs-lookup"><span data-stu-id="8c581-146">Response</span></span>
<span data-ttu-id="8c581-147">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8c581-147">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c581-148">示例</span><span class="sxs-lookup"><span data-stu-id="8c581-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c581-149">请求</span><span class="sxs-lookup"><span data-stu-id="8c581-149">Request</span></span>
<span data-ttu-id="8c581-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c581-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8c581-151">响应</span><span class="sxs-lookup"><span data-stu-id="8c581-151">Response</span></span>
<span data-ttu-id="8c581-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c581-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




