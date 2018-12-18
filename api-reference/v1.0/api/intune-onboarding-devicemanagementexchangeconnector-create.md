---
title: 创建 deviceManagementExchangeConnector
description: 创建新的 deviceManagementExchangeConnector 对象。
author: tfitzmac
ms.openlocfilehash: f1abc9478eb3f845477049ab4007ad16a7434d24
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350972"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="dc5cc-103">创建 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="dc5cc-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="dc5cc-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc5cc-105">创建新的 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-105">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc5cc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="dc5cc-106">Prerequisites</span></span>
<span data-ttu-id="dc5cc-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="dc5cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc5cc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc5cc-109">Permission type</span></span>|<span data-ttu-id="dc5cc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dc5cc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc5cc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc5cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc5cc-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc5cc-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dc5cc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc5cc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc5cc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-114">Not supported.</span></span>|
|<span data-ttu-id="dc5cc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc5cc-115">Application</span></span>|<span data-ttu-id="dc5cc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc5cc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc5cc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="dc5cc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc5cc-118">Request headers</span></span>
|<span data-ttu-id="dc5cc-119">标头</span><span class="sxs-lookup"><span data-stu-id="dc5cc-119">Header</span></span>|<span data-ttu-id="dc5cc-120">值</span><span class="sxs-lookup"><span data-stu-id="dc5cc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc5cc-121">授权</span><span class="sxs-lookup"><span data-stu-id="dc5cc-121">Authorization</span></span>|<span data-ttu-id="dc5cc-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc5cc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dc5cc-123">Accept</span></span>|<span data-ttu-id="dc5cc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dc5cc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc5cc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc5cc-125">Request body</span></span>
<span data-ttu-id="dc5cc-126">在请求正文中，提供 deviceManagementExchangeConnector 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-126">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="dc5cc-127">下表显示创建 deviceManagementExchangeConnector 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-127">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="dc5cc-128">属性</span><span class="sxs-lookup"><span data-stu-id="dc5cc-128">Property</span></span>|<span data-ttu-id="dc5cc-129">类型</span><span class="sxs-lookup"><span data-stu-id="dc5cc-129">Type</span></span>|<span data-ttu-id="dc5cc-130">说明</span><span class="sxs-lookup"><span data-stu-id="dc5cc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc5cc-131">id</span><span class="sxs-lookup"><span data-stu-id="dc5cc-131">id</span></span>|<span data-ttu-id="dc5cc-132">字符串</span><span class="sxs-lookup"><span data-stu-id="dc5cc-132">String</span></span>|<span data-ttu-id="dc5cc-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dc5cc-133">Not yet documented</span></span>|
|<span data-ttu-id="dc5cc-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="dc5cc-134">lastSyncDateTime</span></span>|<span data-ttu-id="dc5cc-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc5cc-135">DateTimeOffset</span></span>|<span data-ttu-id="dc5cc-136">Exchange Connector 的上一次同步时间</span><span class="sxs-lookup"><span data-stu-id="dc5cc-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="dc5cc-137">status</span><span class="sxs-lookup"><span data-stu-id="dc5cc-137">status</span></span>|[<span data-ttu-id="dc5cc-138">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="dc5cc-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="dc5cc-139">Exchange 连接器状态。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-139">Exchange Connector Status.</span></span> <span data-ttu-id="dc5cc-140">可取值为：`none`、`connectionPending`、`connected`、`disconnected`。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="dc5cc-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="dc5cc-141">primarySmtpAddress</span></span>|<span data-ttu-id="dc5cc-142">String</span><span class="sxs-lookup"><span data-stu-id="dc5cc-142">String</span></span>|<span data-ttu-id="dc5cc-143">用于配置服务到服务 Exchange Connector 的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="dc5cc-144">serverName</span><span class="sxs-lookup"><span data-stu-id="dc5cc-144">serverName</span></span>|<span data-ttu-id="dc5cc-145">String</span><span class="sxs-lookup"><span data-stu-id="dc5cc-145">String</span></span>|<span data-ttu-id="dc5cc-146">Exchange server 的名称。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="dc5cc-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="dc5cc-147">connectorServerName</span></span>|<span data-ttu-id="dc5cc-148">String</span><span class="sxs-lookup"><span data-stu-id="dc5cc-148">String</span></span>|<span data-ttu-id="dc5cc-149">托管 Exchange Connector 的服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="dc5cc-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="dc5cc-150">exchangeConnectorType</span></span>|[<span data-ttu-id="dc5cc-151">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="dc5cc-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="dc5cc-152">配置的 Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="dc5cc-153">可取值为：`onPremises`、`hosted`、`serviceToService`、`dedicated`。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="dc5cc-154">version</span><span class="sxs-lookup"><span data-stu-id="dc5cc-154">version</span></span>|<span data-ttu-id="dc5cc-155">String</span><span class="sxs-lookup"><span data-stu-id="dc5cc-155">String</span></span>|<span data-ttu-id="dc5cc-156">ExchangeConnectorAgent 版本</span><span class="sxs-lookup"><span data-stu-id="dc5cc-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="dc5cc-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="dc5cc-157">exchangeAlias</span></span>|<span data-ttu-id="dc5cc-158">String</span><span class="sxs-lookup"><span data-stu-id="dc5cc-158">String</span></span>|<span data-ttu-id="dc5cc-159">分配到 Exchange 服务器的别名</span><span class="sxs-lookup"><span data-stu-id="dc5cc-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="dc5cc-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="dc5cc-160">exchangeOrganization</span></span>|<span data-ttu-id="dc5cc-161">String</span><span class="sxs-lookup"><span data-stu-id="dc5cc-161">String</span></span>|<span data-ttu-id="dc5cc-162">Exchange 服务器的 Exchange 组织</span><span class="sxs-lookup"><span data-stu-id="dc5cc-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="dc5cc-163">响应</span><span class="sxs-lookup"><span data-stu-id="dc5cc-163">Response</span></span>
<span data-ttu-id="dc5cc-164">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-164">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc5cc-165">示例</span><span class="sxs-lookup"><span data-stu-id="dc5cc-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc5cc-166">请求</span><span class="sxs-lookup"><span data-stu-id="dc5cc-166">Request</span></span>
<span data-ttu-id="dc5cc-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dc5cc-168">响应</span><span class="sxs-lookup"><span data-stu-id="dc5cc-168">Response</span></span>
<span data-ttu-id="dc5cc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dc5cc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



