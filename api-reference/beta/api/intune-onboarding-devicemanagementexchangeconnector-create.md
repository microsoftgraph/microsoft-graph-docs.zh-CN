---
title: 创建 deviceManagementExchangeConnector
description: 创建新的 deviceManagementExchangeConnector 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 305360769cc0a13552597644ae9568270bb85e58
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981109"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="7867c-103">创建 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="7867c-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="7867c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7867c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7867c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7867c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7867c-106">创建新的 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7867c-106">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7867c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7867c-107">Prerequisites</span></span>
<span data-ttu-id="7867c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7867c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7867c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7867c-110">Permission type</span></span>|<span data-ttu-id="7867c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7867c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7867c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7867c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7867c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7867c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7867c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7867c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7867c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7867c-115">Not supported.</span></span>|
|<span data-ttu-id="7867c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7867c-116">Application</span></span>|<span data-ttu-id="7867c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7867c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7867c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7867c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="7867c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7867c-119">Request headers</span></span>
|<span data-ttu-id="7867c-120">标头</span><span class="sxs-lookup"><span data-stu-id="7867c-120">Header</span></span>|<span data-ttu-id="7867c-121">值</span><span class="sxs-lookup"><span data-stu-id="7867c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7867c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7867c-122">Authorization</span></span>|<span data-ttu-id="7867c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7867c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7867c-124">接受</span><span class="sxs-lookup"><span data-stu-id="7867c-124">Accept</span></span>|<span data-ttu-id="7867c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7867c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7867c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7867c-126">Request body</span></span>
<span data-ttu-id="7867c-127">在请求正文中，提供 deviceManagementExchangeConnector 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7867c-127">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="7867c-128">下表显示创建 deviceManagementExchangeConnector 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7867c-128">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="7867c-129">属性</span><span class="sxs-lookup"><span data-stu-id="7867c-129">Property</span></span>|<span data-ttu-id="7867c-130">类型</span><span class="sxs-lookup"><span data-stu-id="7867c-130">Type</span></span>|<span data-ttu-id="7867c-131">说明</span><span class="sxs-lookup"><span data-stu-id="7867c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7867c-132">id</span><span class="sxs-lookup"><span data-stu-id="7867c-132">id</span></span>|<span data-ttu-id="7867c-133">String</span><span class="sxs-lookup"><span data-stu-id="7867c-133">String</span></span>|<span data-ttu-id="7867c-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7867c-134">Not yet documented</span></span>|
|<span data-ttu-id="7867c-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7867c-135">lastSyncDateTime</span></span>|<span data-ttu-id="7867c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7867c-136">DateTimeOffset</span></span>|<span data-ttu-id="7867c-137">Exchange Connector 的上一次同步时间</span><span class="sxs-lookup"><span data-stu-id="7867c-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="7867c-138">status</span><span class="sxs-lookup"><span data-stu-id="7867c-138">status</span></span>|[<span data-ttu-id="7867c-139">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="7867c-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="7867c-140">Exchange Connector 状态。</span><span class="sxs-lookup"><span data-stu-id="7867c-140">Exchange Connector Status.</span></span> <span data-ttu-id="7867c-141">可取值为：`none`、`connectionPending`、`connected`、`disconnected`。</span><span class="sxs-lookup"><span data-stu-id="7867c-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="7867c-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="7867c-142">primarySmtpAddress</span></span>|<span data-ttu-id="7867c-143">String</span><span class="sxs-lookup"><span data-stu-id="7867c-143">String</span></span>|<span data-ttu-id="7867c-144">用于配置服务到服务 Exchange Connector 的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="7867c-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="7867c-145">serverName</span><span class="sxs-lookup"><span data-stu-id="7867c-145">serverName</span></span>|<span data-ttu-id="7867c-146">String</span><span class="sxs-lookup"><span data-stu-id="7867c-146">String</span></span>|<span data-ttu-id="7867c-147">Exchange 服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="7867c-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="7867c-148">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="7867c-148">connectorServerName</span></span>|<span data-ttu-id="7867c-149">String</span><span class="sxs-lookup"><span data-stu-id="7867c-149">String</span></span>|<span data-ttu-id="7867c-150">托管 Exchange Connector 的服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="7867c-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="7867c-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="7867c-151">exchangeConnectorType</span></span>|[<span data-ttu-id="7867c-152">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="7867c-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="7867c-153">配置的 Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="7867c-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="7867c-154">可取值为：`onPremises`、`hosted`、`serviceToService`、`dedicated`。</span><span class="sxs-lookup"><span data-stu-id="7867c-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="7867c-155">version</span><span class="sxs-lookup"><span data-stu-id="7867c-155">version</span></span>|<span data-ttu-id="7867c-156">String</span><span class="sxs-lookup"><span data-stu-id="7867c-156">String</span></span>|<span data-ttu-id="7867c-157">ExchangeConnectorAgent 版本</span><span class="sxs-lookup"><span data-stu-id="7867c-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="7867c-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="7867c-158">exchangeAlias</span></span>|<span data-ttu-id="7867c-159">String</span><span class="sxs-lookup"><span data-stu-id="7867c-159">String</span></span>|<span data-ttu-id="7867c-160">分配到 Exchange 服务器的别名</span><span class="sxs-lookup"><span data-stu-id="7867c-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="7867c-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="7867c-161">exchangeOrganization</span></span>|<span data-ttu-id="7867c-162">String</span><span class="sxs-lookup"><span data-stu-id="7867c-162">String</span></span>|<span data-ttu-id="7867c-163">Exchange 服务器的 Exchange 组织</span><span class="sxs-lookup"><span data-stu-id="7867c-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="7867c-164">响应</span><span class="sxs-lookup"><span data-stu-id="7867c-164">Response</span></span>
<span data-ttu-id="7867c-165">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7867c-165">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7867c-166">示例</span><span class="sxs-lookup"><span data-stu-id="7867c-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="7867c-167">请求</span><span class="sxs-lookup"><span data-stu-id="7867c-167">Request</span></span>
<span data-ttu-id="7867c-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7867c-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
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

### <a name="response"></a><span data-ttu-id="7867c-169">响应</span><span class="sxs-lookup"><span data-stu-id="7867c-169">Response</span></span>
<span data-ttu-id="7867c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7867c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





