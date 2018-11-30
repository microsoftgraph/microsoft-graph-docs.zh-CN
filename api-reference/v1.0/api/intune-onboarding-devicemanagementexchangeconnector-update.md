---
title: 更新 deviceManagementExchangeConnector
description: 更新 deviceManagementExchangeConnector 对象的属性。
ms.openlocfilehash: ed63339a390a5fcba377236de8ddfe6c9b57bd5c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009440"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="5a30e-103">更新 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="5a30e-103">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="5a30e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5a30e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a30e-105">更新 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5a30e-105">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a30e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="5a30e-106">Prerequisites</span></span>
<span data-ttu-id="5a30e-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="5a30e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a30e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a30e-109">Permission type</span></span>|<span data-ttu-id="5a30e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5a30e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a30e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a30e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5a30e-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a30e-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5a30e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a30e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a30e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a30e-114">Not supported.</span></span>|
|<span data-ttu-id="5a30e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a30e-115">Application</span></span>|<span data-ttu-id="5a30e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a30e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a30e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a30e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="5a30e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a30e-118">Request headers</span></span>
|<span data-ttu-id="5a30e-119">标头</span><span class="sxs-lookup"><span data-stu-id="5a30e-119">Header</span></span>|<span data-ttu-id="5a30e-120">值</span><span class="sxs-lookup"><span data-stu-id="5a30e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a30e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a30e-121">Authorization</span></span>|<span data-ttu-id="5a30e-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5a30e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a30e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5a30e-123">Accept</span></span>|<span data-ttu-id="5a30e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5a30e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a30e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a30e-125">Request body</span></span>
<span data-ttu-id="5a30e-126">在请求正文中，提供 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a30e-126">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="5a30e-127">下表显示创建 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5a30e-127">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="5a30e-128">属性</span><span class="sxs-lookup"><span data-stu-id="5a30e-128">Property</span></span>|<span data-ttu-id="5a30e-129">类型</span><span class="sxs-lookup"><span data-stu-id="5a30e-129">Type</span></span>|<span data-ttu-id="5a30e-130">说明</span><span class="sxs-lookup"><span data-stu-id="5a30e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a30e-131">id</span><span class="sxs-lookup"><span data-stu-id="5a30e-131">id</span></span>|<span data-ttu-id="5a30e-132">字符串</span><span class="sxs-lookup"><span data-stu-id="5a30e-132">String</span></span>|<span data-ttu-id="5a30e-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5a30e-133">Not yet documented</span></span>|
|<span data-ttu-id="5a30e-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5a30e-134">lastSyncDateTime</span></span>|<span data-ttu-id="5a30e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a30e-135">DateTimeOffset</span></span>|<span data-ttu-id="5a30e-136">Exchange Connector 的上一次同步时间</span><span class="sxs-lookup"><span data-stu-id="5a30e-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="5a30e-137">状态</span><span class="sxs-lookup"><span data-stu-id="5a30e-137">status</span></span>|[<span data-ttu-id="5a30e-138">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="5a30e-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="5a30e-139">Exchange 连接器状态。</span><span class="sxs-lookup"><span data-stu-id="5a30e-139">Exchange Connector Status.</span></span> <span data-ttu-id="5a30e-140">可取值为：`none`、`connectionPending`、`connected`、`disconnected`。</span><span class="sxs-lookup"><span data-stu-id="5a30e-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="5a30e-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5a30e-141">primarySmtpAddress</span></span>|<span data-ttu-id="5a30e-142">String</span><span class="sxs-lookup"><span data-stu-id="5a30e-142">String</span></span>|<span data-ttu-id="5a30e-143">用于配置服务到服务 Exchange Connector 的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5a30e-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="5a30e-144">serverName</span><span class="sxs-lookup"><span data-stu-id="5a30e-144">serverName</span></span>|<span data-ttu-id="5a30e-145">String</span><span class="sxs-lookup"><span data-stu-id="5a30e-145">String</span></span>|<span data-ttu-id="5a30e-146">Exchange server 的名称。</span><span class="sxs-lookup"><span data-stu-id="5a30e-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="5a30e-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="5a30e-147">connectorServerName</span></span>|<span data-ttu-id="5a30e-148">String</span><span class="sxs-lookup"><span data-stu-id="5a30e-148">String</span></span>|<span data-ttu-id="5a30e-149">托管 Exchange Connector 的服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="5a30e-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="5a30e-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="5a30e-150">exchangeConnectorType</span></span>|[<span data-ttu-id="5a30e-151">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="5a30e-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="5a30e-152">配置的 Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="5a30e-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="5a30e-153">可取值为：`onPremises`、`hosted`、`serviceToService`、`dedicated`。</span><span class="sxs-lookup"><span data-stu-id="5a30e-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="5a30e-154">version</span><span class="sxs-lookup"><span data-stu-id="5a30e-154">version</span></span>|<span data-ttu-id="5a30e-155">String</span><span class="sxs-lookup"><span data-stu-id="5a30e-155">String</span></span>|<span data-ttu-id="5a30e-156">ExchangeConnectorAgent 版本</span><span class="sxs-lookup"><span data-stu-id="5a30e-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="5a30e-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="5a30e-157">exchangeAlias</span></span>|<span data-ttu-id="5a30e-158">String</span><span class="sxs-lookup"><span data-stu-id="5a30e-158">String</span></span>|<span data-ttu-id="5a30e-159">分配到 Exchange 服务器的别名</span><span class="sxs-lookup"><span data-stu-id="5a30e-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="5a30e-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="5a30e-160">exchangeOrganization</span></span>|<span data-ttu-id="5a30e-161">String</span><span class="sxs-lookup"><span data-stu-id="5a30e-161">String</span></span>|<span data-ttu-id="5a30e-162">Exchange 服务器的 Exchange 组织</span><span class="sxs-lookup"><span data-stu-id="5a30e-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="5a30e-163">响应</span><span class="sxs-lookup"><span data-stu-id="5a30e-163">Response</span></span>
<span data-ttu-id="5a30e-164">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a30e-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a30e-165">示例</span><span class="sxs-lookup"><span data-stu-id="5a30e-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a30e-166">请求</span><span class="sxs-lookup"><span data-stu-id="5a30e-166">Request</span></span>
<span data-ttu-id="5a30e-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5a30e-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
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

### <a name="response"></a><span data-ttu-id="5a30e-168">响应</span><span class="sxs-lookup"><span data-stu-id="5a30e-168">Response</span></span>
<span data-ttu-id="5a30e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5a30e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



