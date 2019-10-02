---
title: 创建 deviceManagementExchangeConnector
description: 创建新的 deviceManagementExchangeConnector 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ea05e8f7d787065b72ad05f53c7411180293ee2
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362496"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="92292-103">创建 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="92292-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="92292-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92292-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92292-105">创建新的 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92292-105">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92292-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="92292-106">Prerequisites</span></span>
<span data-ttu-id="92292-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92292-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="92292-109">Permission type</span></span>|<span data-ttu-id="92292-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="92292-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92292-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92292-111">Delegated (work or school account)</span></span>|<span data-ttu-id="92292-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92292-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="92292-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92292-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92292-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="92292-114">Not supported.</span></span>|
|<span data-ttu-id="92292-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="92292-115">Application</span></span>|<span data-ttu-id="92292-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="92292-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92292-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92292-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="92292-118">请求头</span><span class="sxs-lookup"><span data-stu-id="92292-118">Request headers</span></span>
|<span data-ttu-id="92292-119">标头</span><span class="sxs-lookup"><span data-stu-id="92292-119">Header</span></span>|<span data-ttu-id="92292-120">值</span><span class="sxs-lookup"><span data-stu-id="92292-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92292-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="92292-121">Authorization</span></span>|<span data-ttu-id="92292-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="92292-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92292-123">接受</span><span class="sxs-lookup"><span data-stu-id="92292-123">Accept</span></span>|<span data-ttu-id="92292-124">application/json</span><span class="sxs-lookup"><span data-stu-id="92292-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92292-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="92292-125">Request body</span></span>
<span data-ttu-id="92292-126">在请求正文中，提供 deviceManagementExchangeConnector 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92292-126">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="92292-127">下表显示创建 deviceManagementExchangeConnector 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="92292-127">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="92292-128">属性</span><span class="sxs-lookup"><span data-stu-id="92292-128">Property</span></span>|<span data-ttu-id="92292-129">类型</span><span class="sxs-lookup"><span data-stu-id="92292-129">Type</span></span>|<span data-ttu-id="92292-130">说明</span><span class="sxs-lookup"><span data-stu-id="92292-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92292-131">id</span><span class="sxs-lookup"><span data-stu-id="92292-131">id</span></span>|<span data-ttu-id="92292-132">String</span><span class="sxs-lookup"><span data-stu-id="92292-132">String</span></span>|<span data-ttu-id="92292-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="92292-133">Not yet documented</span></span>|
|<span data-ttu-id="92292-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="92292-134">lastSyncDateTime</span></span>|<span data-ttu-id="92292-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92292-135">DateTimeOffset</span></span>|<span data-ttu-id="92292-136">Exchange Connector 的上一次同步时间</span><span class="sxs-lookup"><span data-stu-id="92292-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="92292-137">status</span><span class="sxs-lookup"><span data-stu-id="92292-137">status</span></span>|[<span data-ttu-id="92292-138">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="92292-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="92292-139">Exchange Connector 状态。</span><span class="sxs-lookup"><span data-stu-id="92292-139">Exchange Connector Status.</span></span> <span data-ttu-id="92292-140">可取值为：`none`、`connectionPending`、`connected`、`disconnected`。</span><span class="sxs-lookup"><span data-stu-id="92292-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="92292-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="92292-141">primarySmtpAddress</span></span>|<span data-ttu-id="92292-142">String</span><span class="sxs-lookup"><span data-stu-id="92292-142">String</span></span>|<span data-ttu-id="92292-143">用于配置服务到服务 Exchange Connector 的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="92292-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="92292-144">serverName</span><span class="sxs-lookup"><span data-stu-id="92292-144">serverName</span></span>|<span data-ttu-id="92292-145">String</span><span class="sxs-lookup"><span data-stu-id="92292-145">String</span></span>|<span data-ttu-id="92292-146">Exchange 服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="92292-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="92292-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="92292-147">connectorServerName</span></span>|<span data-ttu-id="92292-148">String</span><span class="sxs-lookup"><span data-stu-id="92292-148">String</span></span>|<span data-ttu-id="92292-149">托管 Exchange Connector 的服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="92292-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="92292-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="92292-150">exchangeConnectorType</span></span>|[<span data-ttu-id="92292-151">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="92292-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="92292-152">配置的 Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="92292-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="92292-153">可取值为：`onPremises`、`hosted`、`serviceToService`、`dedicated`。</span><span class="sxs-lookup"><span data-stu-id="92292-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="92292-154">version</span><span class="sxs-lookup"><span data-stu-id="92292-154">version</span></span>|<span data-ttu-id="92292-155">String</span><span class="sxs-lookup"><span data-stu-id="92292-155">String</span></span>|<span data-ttu-id="92292-156">ExchangeConnectorAgent 版本</span><span class="sxs-lookup"><span data-stu-id="92292-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="92292-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="92292-157">exchangeAlias</span></span>|<span data-ttu-id="92292-158">String</span><span class="sxs-lookup"><span data-stu-id="92292-158">String</span></span>|<span data-ttu-id="92292-159">分配到 Exchange 服务器的别名</span><span class="sxs-lookup"><span data-stu-id="92292-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="92292-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="92292-160">exchangeOrganization</span></span>|<span data-ttu-id="92292-161">String</span><span class="sxs-lookup"><span data-stu-id="92292-161">String</span></span>|<span data-ttu-id="92292-162">Exchange 服务器的 Exchange 组织</span><span class="sxs-lookup"><span data-stu-id="92292-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="92292-163">响应</span><span class="sxs-lookup"><span data-stu-id="92292-163">Response</span></span>
<span data-ttu-id="92292-164">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92292-164">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92292-165">示例</span><span class="sxs-lookup"><span data-stu-id="92292-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="92292-166">请求</span><span class="sxs-lookup"><span data-stu-id="92292-166">Request</span></span>
<span data-ttu-id="92292-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92292-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="92292-168">响应</span><span class="sxs-lookup"><span data-stu-id="92292-168">Response</span></span>
<span data-ttu-id="92292-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92292-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```




