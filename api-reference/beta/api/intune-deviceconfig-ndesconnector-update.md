---
title: 更新 ndesConnector
description: 更新 ndesConnector 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c7bb14b89b4474b5196ee563e03d7e7419b0c40
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155069"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="25795-103">更新 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="25795-103">Update ndesConnector</span></span>

<span data-ttu-id="25795-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25795-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25795-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="25795-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25795-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25795-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25795-107">更新 [ndesConnector 对象](../resources/intune-deviceconfig-ndesconnector.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="25795-107">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25795-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="25795-108">Prerequisites</span></span>
<span data-ttu-id="25795-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25795-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25795-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="25795-111">Permission type</span></span>|<span data-ttu-id="25795-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25795-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25795-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25795-113">Delegated (work or school account)</span></span>|<span data-ttu-id="25795-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25795-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25795-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25795-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25795-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="25795-116">Not supported.</span></span>|
|<span data-ttu-id="25795-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="25795-117">Application</span></span>|<span data-ttu-id="25795-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25795-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25795-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25795-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="25795-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="25795-120">Request headers</span></span>
|<span data-ttu-id="25795-121">标头</span><span class="sxs-lookup"><span data-stu-id="25795-121">Header</span></span>|<span data-ttu-id="25795-122">值</span><span class="sxs-lookup"><span data-stu-id="25795-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25795-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="25795-123">Authorization</span></span>|<span data-ttu-id="25795-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="25795-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25795-125">接受</span><span class="sxs-lookup"><span data-stu-id="25795-125">Accept</span></span>|<span data-ttu-id="25795-126">application/json</span><span class="sxs-lookup"><span data-stu-id="25795-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25795-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="25795-127">Request body</span></span>
<span data-ttu-id="25795-128">在请求正文中，提供 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25795-128">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="25795-129">下表显示创建 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="25795-129">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="25795-130">属性</span><span class="sxs-lookup"><span data-stu-id="25795-130">Property</span></span>|<span data-ttu-id="25795-131">类型</span><span class="sxs-lookup"><span data-stu-id="25795-131">Type</span></span>|<span data-ttu-id="25795-132">说明</span><span class="sxs-lookup"><span data-stu-id="25795-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25795-133">id</span><span class="sxs-lookup"><span data-stu-id="25795-133">id</span></span>|<span data-ttu-id="25795-134">String</span><span class="sxs-lookup"><span data-stu-id="25795-134">String</span></span>|<span data-ttu-id="25795-135">NDES 连接器的键。</span><span class="sxs-lookup"><span data-stu-id="25795-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="25795-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="25795-136">lastConnectionDateTime</span></span>|<span data-ttu-id="25795-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25795-137">DateTimeOffset</span></span>|<span data-ttu-id="25795-138">Ndes 连接器的上次连接时间</span><span class="sxs-lookup"><span data-stu-id="25795-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="25795-139">state</span><span class="sxs-lookup"><span data-stu-id="25795-139">state</span></span>|[<span data-ttu-id="25795-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="25795-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="25795-141">Ndes 连接器状态。</span><span class="sxs-lookup"><span data-stu-id="25795-141">Ndes Connector Status.</span></span> <span data-ttu-id="25795-142">可取值为：`none`、`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="25795-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="25795-143">displayName</span><span class="sxs-lookup"><span data-stu-id="25795-143">displayName</span></span>|<span data-ttu-id="25795-144">String</span><span class="sxs-lookup"><span data-stu-id="25795-144">String</span></span>|<span data-ttu-id="25795-145">Ndes 连接器的友好名称。</span><span class="sxs-lookup"><span data-stu-id="25795-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="25795-146">响应</span><span class="sxs-lookup"><span data-stu-id="25795-146">Response</span></span>
<span data-ttu-id="25795-147">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="25795-147">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25795-148">示例</span><span class="sxs-lookup"><span data-stu-id="25795-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="25795-149">请求</span><span class="sxs-lookup"><span data-stu-id="25795-149">Request</span></span>
<span data-ttu-id="25795-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="25795-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="25795-151">响应</span><span class="sxs-lookup"><span data-stu-id="25795-151">Response</span></span>
<span data-ttu-id="25795-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="25795-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




