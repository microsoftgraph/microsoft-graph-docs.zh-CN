---
title: 更新 deviceManagementDomainJoinConnector
description: 更新 deviceManagementDomainJoinConnector 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 12bc8b52a857e70b3bda358365399f398d19c10d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462542"
---
# <a name="update-devicemanagementdomainjoinconnector"></a><span data-ttu-id="1860c-103">更新 deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="1860c-103">Update deviceManagementDomainJoinConnector</span></span>

<span data-ttu-id="1860c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1860c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1860c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1860c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1860c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1860c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1860c-107">更新[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1860c-107">Update the properties of a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1860c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1860c-108">Prerequisites</span></span>
<span data-ttu-id="1860c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1860c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1860c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1860c-111">Permission type</span></span>|<span data-ttu-id="1860c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1860c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1860c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1860c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1860c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1860c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1860c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1860c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1860c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1860c-116">Not supported.</span></span>|
|<span data-ttu-id="1860c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1860c-117">Application</span></span>|<span data-ttu-id="1860c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1860c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1860c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1860c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="1860c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1860c-120">Request headers</span></span>
|<span data-ttu-id="1860c-121">标头</span><span class="sxs-lookup"><span data-stu-id="1860c-121">Header</span></span>|<span data-ttu-id="1860c-122">值</span><span class="sxs-lookup"><span data-stu-id="1860c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1860c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1860c-123">Authorization</span></span>|<span data-ttu-id="1860c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1860c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1860c-125">接受</span><span class="sxs-lookup"><span data-stu-id="1860c-125">Accept</span></span>|<span data-ttu-id="1860c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1860c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1860c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1860c-127">Request body</span></span>
<span data-ttu-id="1860c-128">在请求正文中，提供[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1860c-128">In the request body, supply a JSON representation for the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

<span data-ttu-id="1860c-129">下表显示创建[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1860c-129">The following table shows the properties that are required when you create the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md).</span></span>

|<span data-ttu-id="1860c-130">属性</span><span class="sxs-lookup"><span data-stu-id="1860c-130">Property</span></span>|<span data-ttu-id="1860c-131">类型</span><span class="sxs-lookup"><span data-stu-id="1860c-131">Type</span></span>|<span data-ttu-id="1860c-132">说明</span><span class="sxs-lookup"><span data-stu-id="1860c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1860c-133">id</span><span class="sxs-lookup"><span data-stu-id="1860c-133">id</span></span>|<span data-ttu-id="1860c-134">String</span><span class="sxs-lookup"><span data-stu-id="1860c-134">String</span></span>|<span data-ttu-id="1860c-135">代表连接器的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1860c-135">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="1860c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1860c-136">displayName</span></span>|<span data-ttu-id="1860c-137">字符串</span><span class="sxs-lookup"><span data-stu-id="1860c-137">String</span></span>|<span data-ttu-id="1860c-138">连接器显示名称。</span><span class="sxs-lookup"><span data-stu-id="1860c-138">The connector display name.</span></span>|
|<span data-ttu-id="1860c-139">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="1860c-139">lastConnectionDateTime</span></span>|<span data-ttu-id="1860c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1860c-140">DateTimeOffset</span></span>|<span data-ttu-id="1860c-141">上次联系 Intune 的时间连接器。</span><span class="sxs-lookup"><span data-stu-id="1860c-141">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="1860c-142">state</span><span class="sxs-lookup"><span data-stu-id="1860c-142">state</span></span>|[<span data-ttu-id="1860c-143">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="1860c-143">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="1860c-144">连接器状态。</span><span class="sxs-lookup"><span data-stu-id="1860c-144">The connector state.</span></span> <span data-ttu-id="1860c-145">可取值为：`active`、`error`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="1860c-145">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="1860c-146">version</span><span class="sxs-lookup"><span data-stu-id="1860c-146">version</span></span>|<span data-ttu-id="1860c-147">String</span><span class="sxs-lookup"><span data-stu-id="1860c-147">String</span></span>|<span data-ttu-id="1860c-148">连接器的版本。</span><span class="sxs-lookup"><span data-stu-id="1860c-148">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="1860c-149">响应</span><span class="sxs-lookup"><span data-stu-id="1860c-149">Response</span></span>
<span data-ttu-id="1860c-150">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1860c-150">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1860c-151">示例</span><span class="sxs-lookup"><span data-stu-id="1860c-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="1860c-152">请求</span><span class="sxs-lookup"><span data-stu-id="1860c-152">Request</span></span>
<span data-ttu-id="1860c-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1860c-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
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

### <a name="response"></a><span data-ttu-id="1860c-154">响应</span><span class="sxs-lookup"><span data-stu-id="1860c-154">Response</span></span>
<span data-ttu-id="1860c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1860c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





