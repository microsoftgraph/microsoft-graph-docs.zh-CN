---
title: 创建 deviceManagementDomainJoinConnector
description: 创建新的 deviceManagementDomainJoinConnector 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 178d43f041058f4380c7b179d56d7f91d1923a6a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191097"
---
# <a name="create-devicemanagementdomainjoinconnector"></a><span data-ttu-id="d4abd-103">创建 deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="d4abd-103">Create deviceManagementDomainJoinConnector</span></span>

> <span data-ttu-id="d4abd-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d4abd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4abd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4abd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4abd-106">创建新的[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d4abd-106">Create a new [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4abd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d4abd-107">Prerequisites</span></span>
<span data-ttu-id="d4abd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4abd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4abd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4abd-110">Permission type</span></span>|<span data-ttu-id="d4abd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d4abd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4abd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4abd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4abd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4abd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4abd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4abd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4abd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4abd-115">Not supported.</span></span>|
|<span data-ttu-id="d4abd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4abd-116">Application</span></span>|<span data-ttu-id="d4abd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4abd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4abd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4abd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/domainJoinConnectors
```

## <a name="request-headers"></a><span data-ttu-id="d4abd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4abd-119">Request headers</span></span>
|<span data-ttu-id="d4abd-120">标头</span><span class="sxs-lookup"><span data-stu-id="d4abd-120">Header</span></span>|<span data-ttu-id="d4abd-121">值</span><span class="sxs-lookup"><span data-stu-id="d4abd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4abd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4abd-122">Authorization</span></span>|<span data-ttu-id="d4abd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d4abd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4abd-124">接受</span><span class="sxs-lookup"><span data-stu-id="d4abd-124">Accept</span></span>|<span data-ttu-id="d4abd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4abd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4abd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4abd-126">Request body</span></span>
<span data-ttu-id="d4abd-127">在请求正文中，提供 deviceManagementDomainJoinConnector 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4abd-127">In the request body, supply a JSON representation for the deviceManagementDomainJoinConnector object.</span></span>

<span data-ttu-id="d4abd-128">下表显示创建 deviceManagementDomainJoinConnector 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d4abd-128">The following table shows the properties that are required when you create the deviceManagementDomainJoinConnector.</span></span>

|<span data-ttu-id="d4abd-129">属性</span><span class="sxs-lookup"><span data-stu-id="d4abd-129">Property</span></span>|<span data-ttu-id="d4abd-130">类型</span><span class="sxs-lookup"><span data-stu-id="d4abd-130">Type</span></span>|<span data-ttu-id="d4abd-131">说明</span><span class="sxs-lookup"><span data-stu-id="d4abd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4abd-132">id</span><span class="sxs-lookup"><span data-stu-id="d4abd-132">id</span></span>|<span data-ttu-id="d4abd-133">String</span><span class="sxs-lookup"><span data-stu-id="d4abd-133">String</span></span>|<span data-ttu-id="d4abd-134">代表连接器的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d4abd-134">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="d4abd-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d4abd-135">displayName</span></span>|<span data-ttu-id="d4abd-136">字符串</span><span class="sxs-lookup"><span data-stu-id="d4abd-136">String</span></span>|<span data-ttu-id="d4abd-137">连接器显示名称。</span><span class="sxs-lookup"><span data-stu-id="d4abd-137">The connector display name.</span></span>|
|<span data-ttu-id="d4abd-138">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="d4abd-138">lastConnectionDateTime</span></span>|<span data-ttu-id="d4abd-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4abd-139">DateTimeOffset</span></span>|<span data-ttu-id="d4abd-140">上次联系 Intune 的时间连接器。</span><span class="sxs-lookup"><span data-stu-id="d4abd-140">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="d4abd-141">state</span><span class="sxs-lookup"><span data-stu-id="d4abd-141">state</span></span>|[<span data-ttu-id="d4abd-142">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="d4abd-142">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="d4abd-143">连接器状态。</span><span class="sxs-lookup"><span data-stu-id="d4abd-143">The connector state.</span></span> <span data-ttu-id="d4abd-144">可取值为：`active`、`error`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="d4abd-144">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="d4abd-145">version</span><span class="sxs-lookup"><span data-stu-id="d4abd-145">version</span></span>|<span data-ttu-id="d4abd-146">String</span><span class="sxs-lookup"><span data-stu-id="d4abd-146">String</span></span>|<span data-ttu-id="d4abd-147">连接器的版本。</span><span class="sxs-lookup"><span data-stu-id="d4abd-147">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="d4abd-148">响应</span><span class="sxs-lookup"><span data-stu-id="d4abd-148">Response</span></span>
<span data-ttu-id="d4abd-149">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d4abd-149">If successful, this method returns a `201 Created` response code and a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4abd-150">示例</span><span class="sxs-lookup"><span data-stu-id="d4abd-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4abd-151">请求</span><span class="sxs-lookup"><span data-stu-id="d4abd-151">Request</span></span>
<span data-ttu-id="d4abd-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4abd-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4abd-153">响应</span><span class="sxs-lookup"><span data-stu-id="d4abd-153">Response</span></span>
<span data-ttu-id="d4abd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d4abd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




