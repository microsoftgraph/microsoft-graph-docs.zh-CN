---
title: 创建 deviceManagementDomainJoinConnector
description: 创建新的 deviceManagementDomainJoinConnector 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 294a3538fe31f0da056975d6cfd17ec17efd1a47
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002096"
---
# <a name="create-devicemanagementdomainjoinconnector"></a><span data-ttu-id="4fe60-103">创建 deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="4fe60-103">Create deviceManagementDomainJoinConnector</span></span>

> <span data-ttu-id="4fe60-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4fe60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fe60-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4fe60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fe60-106">创建新的[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4fe60-106">Create a new [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fe60-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4fe60-107">Prerequisites</span></span>
<span data-ttu-id="4fe60-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fe60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fe60-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fe60-110">Permission type</span></span>|<span data-ttu-id="4fe60-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4fe60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fe60-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fe60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4fe60-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fe60-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4fe60-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fe60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fe60-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fe60-115">Not supported.</span></span>|
|<span data-ttu-id="4fe60-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4fe60-116">Application</span></span>|<span data-ttu-id="4fe60-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fe60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fe60-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fe60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/domainJoinConnectors
```

## <a name="request-headers"></a><span data-ttu-id="4fe60-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fe60-119">Request headers</span></span>
|<span data-ttu-id="4fe60-120">标头</span><span class="sxs-lookup"><span data-stu-id="4fe60-120">Header</span></span>|<span data-ttu-id="4fe60-121">值</span><span class="sxs-lookup"><span data-stu-id="4fe60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fe60-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fe60-122">Authorization</span></span>|<span data-ttu-id="4fe60-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4fe60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fe60-124">接受</span><span class="sxs-lookup"><span data-stu-id="4fe60-124">Accept</span></span>|<span data-ttu-id="4fe60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4fe60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fe60-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fe60-126">Request body</span></span>
<span data-ttu-id="4fe60-127">在请求正文中, 提供 deviceManagementDomainJoinConnector 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4fe60-127">In the request body, supply a JSON representation for the deviceManagementDomainJoinConnector object.</span></span>

<span data-ttu-id="4fe60-128">下表显示创建 deviceManagementDomainJoinConnector 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4fe60-128">The following table shows the properties that are required when you create the deviceManagementDomainJoinConnector.</span></span>

|<span data-ttu-id="4fe60-129">属性</span><span class="sxs-lookup"><span data-stu-id="4fe60-129">Property</span></span>|<span data-ttu-id="4fe60-130">类型</span><span class="sxs-lookup"><span data-stu-id="4fe60-130">Type</span></span>|<span data-ttu-id="4fe60-131">说明</span><span class="sxs-lookup"><span data-stu-id="4fe60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fe60-132">id</span><span class="sxs-lookup"><span data-stu-id="4fe60-132">id</span></span>|<span data-ttu-id="4fe60-133">String</span><span class="sxs-lookup"><span data-stu-id="4fe60-133">String</span></span>|<span data-ttu-id="4fe60-134">代表连接器的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4fe60-134">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="4fe60-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4fe60-135">displayName</span></span>|<span data-ttu-id="4fe60-136">字符串</span><span class="sxs-lookup"><span data-stu-id="4fe60-136">String</span></span>|<span data-ttu-id="4fe60-137">连接器显示名称。</span><span class="sxs-lookup"><span data-stu-id="4fe60-137">The connector display name.</span></span>|
|<span data-ttu-id="4fe60-138">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="4fe60-138">lastConnectionDateTime</span></span>|<span data-ttu-id="4fe60-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fe60-139">DateTimeOffset</span></span>|<span data-ttu-id="4fe60-140">上次联系 Intune 的时间连接器。</span><span class="sxs-lookup"><span data-stu-id="4fe60-140">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="4fe60-141">state</span><span class="sxs-lookup"><span data-stu-id="4fe60-141">state</span></span>|[<span data-ttu-id="4fe60-142">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="4fe60-142">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="4fe60-143">连接器状态。</span><span class="sxs-lookup"><span data-stu-id="4fe60-143">The connector state.</span></span> <span data-ttu-id="4fe60-144">可取值为：`active`、`error`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="4fe60-144">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="4fe60-145">version</span><span class="sxs-lookup"><span data-stu-id="4fe60-145">version</span></span>|<span data-ttu-id="4fe60-146">String</span><span class="sxs-lookup"><span data-stu-id="4fe60-146">String</span></span>|<span data-ttu-id="4fe60-147">连接器的版本。</span><span class="sxs-lookup"><span data-stu-id="4fe60-147">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="4fe60-148">响应</span><span class="sxs-lookup"><span data-stu-id="4fe60-148">Response</span></span>
<span data-ttu-id="4fe60-149">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4fe60-149">If successful, this method returns a `201 Created` response code and a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fe60-150">示例</span><span class="sxs-lookup"><span data-stu-id="4fe60-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fe60-151">请求</span><span class="sxs-lookup"><span data-stu-id="4fe60-151">Request</span></span>
<span data-ttu-id="4fe60-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4fe60-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "error",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="4fe60-153">响应</span><span class="sxs-lookup"><span data-stu-id="4fe60-153">Response</span></span>
<span data-ttu-id="4fe60-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4fe60-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "77296cf7-6cf7-7729-f76c-2977f76c2977",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "error",
  "version": "Version value"
}
```





