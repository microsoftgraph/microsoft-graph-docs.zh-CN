---
title: 创建 ndesConnector
description: 创建新的 ndesConnector 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c9e5700c4637d9581bcf71ee18e9e8c82772ceee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000852"
---
# <a name="create-ndesconnector"></a><span data-ttu-id="f020c-103">创建 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="f020c-103">Create ndesConnector</span></span>

<span data-ttu-id="f020c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f020c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f020c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f020c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f020c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f020c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f020c-107">创建新的 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f020c-107">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f020c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f020c-108">Prerequisites</span></span>
<span data-ttu-id="f020c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f020c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f020c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f020c-111">Permission type</span></span>|<span data-ttu-id="f020c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f020c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f020c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f020c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f020c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f020c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f020c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f020c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f020c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f020c-116">Not supported.</span></span>|
|<span data-ttu-id="f020c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f020c-117">Application</span></span>|<span data-ttu-id="f020c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f020c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f020c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f020c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="f020c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f020c-120">Request headers</span></span>
|<span data-ttu-id="f020c-121">标头</span><span class="sxs-lookup"><span data-stu-id="f020c-121">Header</span></span>|<span data-ttu-id="f020c-122">值</span><span class="sxs-lookup"><span data-stu-id="f020c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f020c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f020c-123">Authorization</span></span>|<span data-ttu-id="f020c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f020c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f020c-125">接受</span><span class="sxs-lookup"><span data-stu-id="f020c-125">Accept</span></span>|<span data-ttu-id="f020c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f020c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f020c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f020c-127">Request body</span></span>
<span data-ttu-id="f020c-128">在请求正文中，提供 ndesConnector 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f020c-128">In the request body, supply a JSON representation for the ndesConnector object.</span></span>

<span data-ttu-id="f020c-129">下表显示创建 ndesConnector 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f020c-129">The following table shows the properties that are required when you create the ndesConnector.</span></span>

|<span data-ttu-id="f020c-130">属性</span><span class="sxs-lookup"><span data-stu-id="f020c-130">Property</span></span>|<span data-ttu-id="f020c-131">类型</span><span class="sxs-lookup"><span data-stu-id="f020c-131">Type</span></span>|<span data-ttu-id="f020c-132">说明</span><span class="sxs-lookup"><span data-stu-id="f020c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f020c-133">id</span><span class="sxs-lookup"><span data-stu-id="f020c-133">id</span></span>|<span data-ttu-id="f020c-134">String</span><span class="sxs-lookup"><span data-stu-id="f020c-134">String</span></span>|<span data-ttu-id="f020c-135">NDES 连接器的键。</span><span class="sxs-lookup"><span data-stu-id="f020c-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="f020c-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="f020c-136">lastConnectionDateTime</span></span>|<span data-ttu-id="f020c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f020c-137">DateTimeOffset</span></span>|<span data-ttu-id="f020c-138">Ndes 连接器的上次连接时间</span><span class="sxs-lookup"><span data-stu-id="f020c-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="f020c-139">state</span><span class="sxs-lookup"><span data-stu-id="f020c-139">state</span></span>|[<span data-ttu-id="f020c-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="f020c-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="f020c-141">Ndes 连接器状态。</span><span class="sxs-lookup"><span data-stu-id="f020c-141">Ndes Connector Status.</span></span> <span data-ttu-id="f020c-142">可取值为：`none`、`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="f020c-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="f020c-143">displayName</span><span class="sxs-lookup"><span data-stu-id="f020c-143">displayName</span></span>|<span data-ttu-id="f020c-144">String</span><span class="sxs-lookup"><span data-stu-id="f020c-144">String</span></span>|<span data-ttu-id="f020c-145">Ndes 连接器的友好名称。</span><span class="sxs-lookup"><span data-stu-id="f020c-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="f020c-146">响应</span><span class="sxs-lookup"><span data-stu-id="f020c-146">Response</span></span>
<span data-ttu-id="f020c-147">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f020c-147">If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f020c-148">示例</span><span class="sxs-lookup"><span data-stu-id="f020c-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="f020c-149">请求</span><span class="sxs-lookup"><span data-stu-id="f020c-149">Request</span></span>
<span data-ttu-id="f020c-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f020c-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/ndesConnectors
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="f020c-151">响应</span><span class="sxs-lookup"><span data-stu-id="f020c-151">Response</span></span>
<span data-ttu-id="f020c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f020c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






