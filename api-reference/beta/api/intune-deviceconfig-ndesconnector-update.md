---
title: 更新 ndesConnector
description: 更新 ndesConnector 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4d51f22c71ef43784ec45e521f0e1900abdb9c0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140276"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="5f3e2-103">更新 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="5f3e2-103">Update ndesConnector</span></span>

> <span data-ttu-id="5f3e2-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f3e2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f3e2-106">更新[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-106">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f3e2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5f3e2-107">Prerequisites</span></span>
<span data-ttu-id="5f3e2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5f3e2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f3e2-110">Permission type</span></span>|<span data-ttu-id="5f3e2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5f3e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f3e2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f3e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f3e2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f3e2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5f3e2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f3e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f3e2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-115">Not supported.</span></span>|
|<span data-ttu-id="5f3e2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f3e2-116">Application</span></span>|<span data-ttu-id="5f3e2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f3e2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f3e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="5f3e2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f3e2-119">Request headers</span></span>
|<span data-ttu-id="5f3e2-120">标头</span><span class="sxs-lookup"><span data-stu-id="5f3e2-120">Header</span></span>|<span data-ttu-id="5f3e2-121">值</span><span class="sxs-lookup"><span data-stu-id="5f3e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f3e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f3e2-122">Authorization</span></span>|<span data-ttu-id="5f3e2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f3e2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5f3e2-124">Accept</span></span>|<span data-ttu-id="5f3e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f3e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f3e2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f3e2-126">Request body</span></span>
<span data-ttu-id="5f3e2-127">在请求正文中, 提供[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-127">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="5f3e2-128">下表显示创建[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-128">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="5f3e2-129">属性</span><span class="sxs-lookup"><span data-stu-id="5f3e2-129">Property</span></span>|<span data-ttu-id="5f3e2-130">类型</span><span class="sxs-lookup"><span data-stu-id="5f3e2-130">Type</span></span>|<span data-ttu-id="5f3e2-131">说明</span><span class="sxs-lookup"><span data-stu-id="5f3e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f3e2-132">id</span><span class="sxs-lookup"><span data-stu-id="5f3e2-132">id</span></span>|<span data-ttu-id="5f3e2-133">字符串</span><span class="sxs-lookup"><span data-stu-id="5f3e2-133">String</span></span>|<span data-ttu-id="5f3e2-134">NDES 连接器的键。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-134">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="5f3e2-135">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="5f3e2-135">lastConnectionDateTime</span></span>|<span data-ttu-id="5f3e2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f3e2-136">DateTimeOffset</span></span>|<span data-ttu-id="5f3e2-137">Ndes 连接器的上次连接时间</span><span class="sxs-lookup"><span data-stu-id="5f3e2-137">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="5f3e2-138">state</span><span class="sxs-lookup"><span data-stu-id="5f3e2-138">state</span></span>|[<span data-ttu-id="5f3e2-139">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="5f3e2-139">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="5f3e2-140">Ndes 连接器状态。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-140">Ndes Connector Status.</span></span> <span data-ttu-id="5f3e2-141">可取值为：`none`、`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-141">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="5f3e2-142">displayName</span><span class="sxs-lookup"><span data-stu-id="5f3e2-142">displayName</span></span>|<span data-ttu-id="5f3e2-143">String</span><span class="sxs-lookup"><span data-stu-id="5f3e2-143">String</span></span>|<span data-ttu-id="5f3e2-144">Ndes 连接器的友好名称。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-144">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="5f3e2-145">响应</span><span class="sxs-lookup"><span data-stu-id="5f3e2-145">Response</span></span>
<span data-ttu-id="5f3e2-146">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-146">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f3e2-147">示例</span><span class="sxs-lookup"><span data-stu-id="5f3e2-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f3e2-148">请求</span><span class="sxs-lookup"><span data-stu-id="5f3e2-148">Request</span></span>
<span data-ttu-id="5f3e2-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5f3e2-150">响应</span><span class="sxs-lookup"><span data-stu-id="5f3e2-150">Response</span></span>
<span data-ttu-id="5f3e2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5f3e2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




