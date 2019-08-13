---
title: 更新 ndesConnector
description: 更新 ndesConnector 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a28f58cf611e45534e65e58e63556921ba87e926
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345538"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="71ab9-103">更新 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="71ab9-103">Update ndesConnector</span></span>

> <span data-ttu-id="71ab9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="71ab9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71ab9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71ab9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71ab9-106">更新[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="71ab9-106">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71ab9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="71ab9-107">Prerequisites</span></span>
<span data-ttu-id="71ab9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71ab9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71ab9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="71ab9-110">Permission type</span></span>|<span data-ttu-id="71ab9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="71ab9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71ab9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71ab9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71ab9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71ab9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71ab9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71ab9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71ab9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="71ab9-115">Not supported.</span></span>|
|<span data-ttu-id="71ab9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="71ab9-116">Application</span></span>|<span data-ttu-id="71ab9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71ab9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71ab9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71ab9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="71ab9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="71ab9-119">Request headers</span></span>
|<span data-ttu-id="71ab9-120">标头</span><span class="sxs-lookup"><span data-stu-id="71ab9-120">Header</span></span>|<span data-ttu-id="71ab9-121">值</span><span class="sxs-lookup"><span data-stu-id="71ab9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71ab9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71ab9-122">Authorization</span></span>|<span data-ttu-id="71ab9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="71ab9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71ab9-124">接受</span><span class="sxs-lookup"><span data-stu-id="71ab9-124">Accept</span></span>|<span data-ttu-id="71ab9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71ab9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71ab9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="71ab9-126">Request body</span></span>
<span data-ttu-id="71ab9-127">在请求正文中, 提供[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71ab9-127">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="71ab9-128">下表显示创建[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="71ab9-128">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="71ab9-129">属性</span><span class="sxs-lookup"><span data-stu-id="71ab9-129">Property</span></span>|<span data-ttu-id="71ab9-130">类型</span><span class="sxs-lookup"><span data-stu-id="71ab9-130">Type</span></span>|<span data-ttu-id="71ab9-131">说明</span><span class="sxs-lookup"><span data-stu-id="71ab9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71ab9-132">id</span><span class="sxs-lookup"><span data-stu-id="71ab9-132">id</span></span>|<span data-ttu-id="71ab9-133">String</span><span class="sxs-lookup"><span data-stu-id="71ab9-133">String</span></span>|<span data-ttu-id="71ab9-134">NDES 连接器的键。</span><span class="sxs-lookup"><span data-stu-id="71ab9-134">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="71ab9-135">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="71ab9-135">lastConnectionDateTime</span></span>|<span data-ttu-id="71ab9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71ab9-136">DateTimeOffset</span></span>|<span data-ttu-id="71ab9-137">Ndes 连接器的上次连接时间</span><span class="sxs-lookup"><span data-stu-id="71ab9-137">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="71ab9-138">state</span><span class="sxs-lookup"><span data-stu-id="71ab9-138">state</span></span>|[<span data-ttu-id="71ab9-139">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="71ab9-139">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="71ab9-140">Ndes 连接器状态。</span><span class="sxs-lookup"><span data-stu-id="71ab9-140">Ndes Connector Status.</span></span> <span data-ttu-id="71ab9-141">可取值为：`none`、`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="71ab9-141">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="71ab9-142">displayName</span><span class="sxs-lookup"><span data-stu-id="71ab9-142">displayName</span></span>|<span data-ttu-id="71ab9-143">String</span><span class="sxs-lookup"><span data-stu-id="71ab9-143">String</span></span>|<span data-ttu-id="71ab9-144">Ndes 连接器的友好名称。</span><span class="sxs-lookup"><span data-stu-id="71ab9-144">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="71ab9-145">响应</span><span class="sxs-lookup"><span data-stu-id="71ab9-145">Response</span></span>
<span data-ttu-id="71ab9-146">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="71ab9-146">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71ab9-147">示例</span><span class="sxs-lookup"><span data-stu-id="71ab9-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="71ab9-148">请求</span><span class="sxs-lookup"><span data-stu-id="71ab9-148">Request</span></span>
<span data-ttu-id="71ab9-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71ab9-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="71ab9-150">响应</span><span class="sxs-lookup"><span data-stu-id="71ab9-150">Response</span></span>
<span data-ttu-id="71ab9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71ab9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






