---
title: 创建 deviceManagementExchangeConnector
description: 创建新的 deviceManagementExchangeConnector 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57e770f1c6929016e1ef15e806aec5924316d5b6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512683"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="d4ece-103">创建 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="d4ece-103">Create deviceManagementExchangeConnector</span></span>

<span data-ttu-id="d4ece-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4ece-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4ece-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4ece-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4ece-106">创建新的 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d4ece-106">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4ece-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d4ece-107">Prerequisites</span></span>
<span data-ttu-id="d4ece-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4ece-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4ece-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4ece-110">Permission type</span></span>|<span data-ttu-id="d4ece-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d4ece-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4ece-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4ece-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4ece-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4ece-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d4ece-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4ece-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4ece-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4ece-115">Not supported.</span></span>|
|<span data-ttu-id="d4ece-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4ece-116">Application</span></span>|<span data-ttu-id="d4ece-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4ece-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4ece-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4ece-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="d4ece-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4ece-119">Request headers</span></span>
|<span data-ttu-id="d4ece-120">标头</span><span class="sxs-lookup"><span data-stu-id="d4ece-120">Header</span></span>|<span data-ttu-id="d4ece-121">值</span><span class="sxs-lookup"><span data-stu-id="d4ece-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4ece-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4ece-122">Authorization</span></span>|<span data-ttu-id="d4ece-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d4ece-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4ece-124">接受</span><span class="sxs-lookup"><span data-stu-id="d4ece-124">Accept</span></span>|<span data-ttu-id="d4ece-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4ece-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4ece-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4ece-126">Request body</span></span>
<span data-ttu-id="d4ece-127">在请求正文中，提供 deviceManagementExchangeConnector 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4ece-127">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="d4ece-128">下表显示创建 deviceManagementExchangeConnector 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d4ece-128">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="d4ece-129">属性</span><span class="sxs-lookup"><span data-stu-id="d4ece-129">Property</span></span>|<span data-ttu-id="d4ece-130">类型</span><span class="sxs-lookup"><span data-stu-id="d4ece-130">Type</span></span>|<span data-ttu-id="d4ece-131">说明</span><span class="sxs-lookup"><span data-stu-id="d4ece-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4ece-132">id</span><span class="sxs-lookup"><span data-stu-id="d4ece-132">id</span></span>|<span data-ttu-id="d4ece-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d4ece-133">String</span></span>|<span data-ttu-id="d4ece-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d4ece-134">Not yet documented</span></span>|
|<span data-ttu-id="d4ece-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d4ece-135">lastSyncDateTime</span></span>|<span data-ttu-id="d4ece-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4ece-136">DateTimeOffset</span></span>|<span data-ttu-id="d4ece-137">Exchange Connector 的上一次同步时间</span><span class="sxs-lookup"><span data-stu-id="d4ece-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="d4ece-138">status</span><span class="sxs-lookup"><span data-stu-id="d4ece-138">status</span></span>|[<span data-ttu-id="d4ece-139">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="d4ece-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="d4ece-140">Exchange Connector 状态。</span><span class="sxs-lookup"><span data-stu-id="d4ece-140">Exchange Connector Status.</span></span> <span data-ttu-id="d4ece-141">可取值为：`none`、`connectionPending`、`connected`、`disconnected`。</span><span class="sxs-lookup"><span data-stu-id="d4ece-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="d4ece-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="d4ece-142">primarySmtpAddress</span></span>|<span data-ttu-id="d4ece-143">字符串</span><span class="sxs-lookup"><span data-stu-id="d4ece-143">String</span></span>|<span data-ttu-id="d4ece-144">用于配置服务到服务 Exchange Connector 的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d4ece-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="d4ece-145">serverName</span><span class="sxs-lookup"><span data-stu-id="d4ece-145">serverName</span></span>|<span data-ttu-id="d4ece-146">字符串</span><span class="sxs-lookup"><span data-stu-id="d4ece-146">String</span></span>|<span data-ttu-id="d4ece-147">Exchange 服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="d4ece-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="d4ece-148">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="d4ece-148">connectorServerName</span></span>|<span data-ttu-id="d4ece-149">字符串</span><span class="sxs-lookup"><span data-stu-id="d4ece-149">String</span></span>|<span data-ttu-id="d4ece-150">托管 Exchange Connector 的服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="d4ece-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="d4ece-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="d4ece-151">exchangeConnectorType</span></span>|[<span data-ttu-id="d4ece-152">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="d4ece-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="d4ece-153">配置的 Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="d4ece-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="d4ece-154">可取值为：`onPremises`、`hosted`、`serviceToService`、`dedicated`。</span><span class="sxs-lookup"><span data-stu-id="d4ece-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="d4ece-155">version</span><span class="sxs-lookup"><span data-stu-id="d4ece-155">version</span></span>|<span data-ttu-id="d4ece-156">字符串</span><span class="sxs-lookup"><span data-stu-id="d4ece-156">String</span></span>|<span data-ttu-id="d4ece-157">ExchangeConnectorAgent 版本</span><span class="sxs-lookup"><span data-stu-id="d4ece-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="d4ece-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="d4ece-158">exchangeAlias</span></span>|<span data-ttu-id="d4ece-159">字符串</span><span class="sxs-lookup"><span data-stu-id="d4ece-159">String</span></span>|<span data-ttu-id="d4ece-160">分配到 Exchange 服务器的别名</span><span class="sxs-lookup"><span data-stu-id="d4ece-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="d4ece-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="d4ece-161">exchangeOrganization</span></span>|<span data-ttu-id="d4ece-162">String</span><span class="sxs-lookup"><span data-stu-id="d4ece-162">String</span></span>|<span data-ttu-id="d4ece-163">Exchange 服务器的 Exchange 组织</span><span class="sxs-lookup"><span data-stu-id="d4ece-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="d4ece-164">响应</span><span class="sxs-lookup"><span data-stu-id="d4ece-164">Response</span></span>
<span data-ttu-id="d4ece-165">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d4ece-165">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4ece-166">示例</span><span class="sxs-lookup"><span data-stu-id="d4ece-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4ece-167">请求</span><span class="sxs-lookup"><span data-stu-id="d4ece-167">Request</span></span>
<span data-ttu-id="d4ece-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4ece-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4ece-169">响应</span><span class="sxs-lookup"><span data-stu-id="d4ece-169">Response</span></span>
<span data-ttu-id="d4ece-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d4ece-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




