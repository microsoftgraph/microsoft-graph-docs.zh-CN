---
title: 创建 deviceManagementExchangeConnector
description: 创建新的 deviceManagementExchangeConnector 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b28bea7bf25050003784b6f8488db81c1d9f651
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156947"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="a6dcb-103">创建 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="a6dcb-103">Create deviceManagementExchangeConnector</span></span>

<span data-ttu-id="a6dcb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6dcb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6dcb-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6dcb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6dcb-107">创建新的 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-107">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6dcb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6dcb-108">Prerequisites</span></span>
<span data-ttu-id="a6dcb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6dcb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6dcb-111">Permission type</span></span>|<span data-ttu-id="a6dcb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a6dcb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6dcb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6dcb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6dcb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6dcb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a6dcb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6dcb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6dcb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-116">Not supported.</span></span>|
|<span data-ttu-id="a6dcb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6dcb-117">Application</span></span>|<span data-ttu-id="a6dcb-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6dcb-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6dcb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6dcb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="a6dcb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6dcb-120">Request headers</span></span>
|<span data-ttu-id="a6dcb-121">标头</span><span class="sxs-lookup"><span data-stu-id="a6dcb-121">Header</span></span>|<span data-ttu-id="a6dcb-122">值</span><span class="sxs-lookup"><span data-stu-id="a6dcb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6dcb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6dcb-123">Authorization</span></span>|<span data-ttu-id="a6dcb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6dcb-125">接受</span><span class="sxs-lookup"><span data-stu-id="a6dcb-125">Accept</span></span>|<span data-ttu-id="a6dcb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6dcb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6dcb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6dcb-127">Request body</span></span>
<span data-ttu-id="a6dcb-128">在请求正文中，提供 deviceManagementExchangeConnector 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-128">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="a6dcb-129">下表显示创建 deviceManagementExchangeConnector 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-129">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="a6dcb-130">属性</span><span class="sxs-lookup"><span data-stu-id="a6dcb-130">Property</span></span>|<span data-ttu-id="a6dcb-131">类型</span><span class="sxs-lookup"><span data-stu-id="a6dcb-131">Type</span></span>|<span data-ttu-id="a6dcb-132">说明</span><span class="sxs-lookup"><span data-stu-id="a6dcb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6dcb-133">id</span><span class="sxs-lookup"><span data-stu-id="a6dcb-133">id</span></span>|<span data-ttu-id="a6dcb-134">String</span><span class="sxs-lookup"><span data-stu-id="a6dcb-134">String</span></span>|<span data-ttu-id="a6dcb-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a6dcb-135">Not yet documented</span></span>|
|<span data-ttu-id="a6dcb-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a6dcb-136">lastSyncDateTime</span></span>|<span data-ttu-id="a6dcb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6dcb-137">DateTimeOffset</span></span>|<span data-ttu-id="a6dcb-138">Exchange Connector 的上一次同步时间</span><span class="sxs-lookup"><span data-stu-id="a6dcb-138">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="a6dcb-139">status</span><span class="sxs-lookup"><span data-stu-id="a6dcb-139">status</span></span>|[<span data-ttu-id="a6dcb-140">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="a6dcb-140">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="a6dcb-141">Exchange 连接器状态。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-141">Exchange Connector Status.</span></span> <span data-ttu-id="a6dcb-142">可取值为：`none`、`connectionPending`、`connected`、`disconnected`。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-142">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="a6dcb-143">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="a6dcb-143">primarySmtpAddress</span></span>|<span data-ttu-id="a6dcb-144">String</span><span class="sxs-lookup"><span data-stu-id="a6dcb-144">String</span></span>|<span data-ttu-id="a6dcb-145">用于配置服务到服务 Exchange Connector 的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-145">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="a6dcb-146">serverName</span><span class="sxs-lookup"><span data-stu-id="a6dcb-146">serverName</span></span>|<span data-ttu-id="a6dcb-147">String</span><span class="sxs-lookup"><span data-stu-id="a6dcb-147">String</span></span>|<span data-ttu-id="a6dcb-148">Exchange 服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-148">The name of the Exchange server.</span></span>|
|<span data-ttu-id="a6dcb-149">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="a6dcb-149">connectorServerName</span></span>|<span data-ttu-id="a6dcb-150">String</span><span class="sxs-lookup"><span data-stu-id="a6dcb-150">String</span></span>|<span data-ttu-id="a6dcb-151">托管 Exchange Connector 的服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-151">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="a6dcb-152">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="a6dcb-152">exchangeConnectorType</span></span>|[<span data-ttu-id="a6dcb-153">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="a6dcb-153">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="a6dcb-154">配置的 Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-154">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="a6dcb-155">可取值为：`onPremises`、`hosted`、`serviceToService`、`dedicated`。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-155">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="a6dcb-156">version</span><span class="sxs-lookup"><span data-stu-id="a6dcb-156">version</span></span>|<span data-ttu-id="a6dcb-157">String</span><span class="sxs-lookup"><span data-stu-id="a6dcb-157">String</span></span>|<span data-ttu-id="a6dcb-158">ExchangeConnectorAgent 版本</span><span class="sxs-lookup"><span data-stu-id="a6dcb-158">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="a6dcb-159">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="a6dcb-159">exchangeAlias</span></span>|<span data-ttu-id="a6dcb-160">String</span><span class="sxs-lookup"><span data-stu-id="a6dcb-160">String</span></span>|<span data-ttu-id="a6dcb-161">分配到 Exchange 服务器的别名</span><span class="sxs-lookup"><span data-stu-id="a6dcb-161">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="a6dcb-162">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="a6dcb-162">exchangeOrganization</span></span>|<span data-ttu-id="a6dcb-163">String</span><span class="sxs-lookup"><span data-stu-id="a6dcb-163">String</span></span>|<span data-ttu-id="a6dcb-164">Exchange 服务器的 Exchange 组织</span><span class="sxs-lookup"><span data-stu-id="a6dcb-164">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="a6dcb-165">响应</span><span class="sxs-lookup"><span data-stu-id="a6dcb-165">Response</span></span>
<span data-ttu-id="a6dcb-166">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-166">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6dcb-167">示例</span><span class="sxs-lookup"><span data-stu-id="a6dcb-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6dcb-168">请求</span><span class="sxs-lookup"><span data-stu-id="a6dcb-168">Request</span></span>
<span data-ttu-id="a6dcb-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a6dcb-170">响应</span><span class="sxs-lookup"><span data-stu-id="a6dcb-170">Response</span></span>
<span data-ttu-id="a6dcb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6dcb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




