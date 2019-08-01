---
title: 更新 deviceManagementExchangeConnector
description: 更新 deviceManagementExchangeConnector 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3df6bd94985a3f3c3ff5eac25c08eb80a156dfaa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974694"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="58fb5-103">更新 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="58fb5-103">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="58fb5-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58fb5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58fb5-105">更新 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="58fb5-105">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58fb5-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="58fb5-106">Prerequisites</span></span>
<span data-ttu-id="58fb5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58fb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58fb5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="58fb5-109">Permission type</span></span>|<span data-ttu-id="58fb5-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="58fb5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58fb5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58fb5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="58fb5-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58fb5-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="58fb5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58fb5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58fb5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="58fb5-114">Not supported.</span></span>|
|<span data-ttu-id="58fb5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="58fb5-115">Application</span></span>|<span data-ttu-id="58fb5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="58fb5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58fb5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58fb5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="58fb5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="58fb5-118">Request headers</span></span>
|<span data-ttu-id="58fb5-119">标头</span><span class="sxs-lookup"><span data-stu-id="58fb5-119">Header</span></span>|<span data-ttu-id="58fb5-120">值</span><span class="sxs-lookup"><span data-stu-id="58fb5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58fb5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="58fb5-121">Authorization</span></span>|<span data-ttu-id="58fb5-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="58fb5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58fb5-123">接受</span><span class="sxs-lookup"><span data-stu-id="58fb5-123">Accept</span></span>|<span data-ttu-id="58fb5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="58fb5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58fb5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="58fb5-125">Request body</span></span>
<span data-ttu-id="58fb5-126">在请求正文中，提供 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58fb5-126">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="58fb5-127">下表显示创建 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="58fb5-127">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="58fb5-128">属性</span><span class="sxs-lookup"><span data-stu-id="58fb5-128">Property</span></span>|<span data-ttu-id="58fb5-129">类型</span><span class="sxs-lookup"><span data-stu-id="58fb5-129">Type</span></span>|<span data-ttu-id="58fb5-130">说明</span><span class="sxs-lookup"><span data-stu-id="58fb5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58fb5-131">id</span><span class="sxs-lookup"><span data-stu-id="58fb5-131">id</span></span>|<span data-ttu-id="58fb5-132">String</span><span class="sxs-lookup"><span data-stu-id="58fb5-132">String</span></span>|<span data-ttu-id="58fb5-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="58fb5-133">Not yet documented</span></span>|
|<span data-ttu-id="58fb5-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="58fb5-134">lastSyncDateTime</span></span>|<span data-ttu-id="58fb5-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58fb5-135">DateTimeOffset</span></span>|<span data-ttu-id="58fb5-136">Exchange Connector 的上一次同步时间</span><span class="sxs-lookup"><span data-stu-id="58fb5-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="58fb5-137">status</span><span class="sxs-lookup"><span data-stu-id="58fb5-137">status</span></span>|[<span data-ttu-id="58fb5-138">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="58fb5-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="58fb5-139">Exchange Connector 状态。</span><span class="sxs-lookup"><span data-stu-id="58fb5-139">Exchange Connector Status.</span></span> <span data-ttu-id="58fb5-140">可取值为：`none`、`connectionPending`、`connected`、`disconnected`。</span><span class="sxs-lookup"><span data-stu-id="58fb5-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="58fb5-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="58fb5-141">primarySmtpAddress</span></span>|<span data-ttu-id="58fb5-142">String</span><span class="sxs-lookup"><span data-stu-id="58fb5-142">String</span></span>|<span data-ttu-id="58fb5-143">用于配置服务到服务 Exchange Connector 的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="58fb5-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="58fb5-144">serverName</span><span class="sxs-lookup"><span data-stu-id="58fb5-144">serverName</span></span>|<span data-ttu-id="58fb5-145">String</span><span class="sxs-lookup"><span data-stu-id="58fb5-145">String</span></span>|<span data-ttu-id="58fb5-146">Exchange 服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="58fb5-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="58fb5-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="58fb5-147">connectorServerName</span></span>|<span data-ttu-id="58fb5-148">String</span><span class="sxs-lookup"><span data-stu-id="58fb5-148">String</span></span>|<span data-ttu-id="58fb5-149">托管 Exchange Connector 的服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="58fb5-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="58fb5-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="58fb5-150">exchangeConnectorType</span></span>|[<span data-ttu-id="58fb5-151">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="58fb5-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="58fb5-152">配置的 Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="58fb5-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="58fb5-153">可取值为：`onPremises`、`hosted`、`serviceToService`、`dedicated`。</span><span class="sxs-lookup"><span data-stu-id="58fb5-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="58fb5-154">version</span><span class="sxs-lookup"><span data-stu-id="58fb5-154">version</span></span>|<span data-ttu-id="58fb5-155">String</span><span class="sxs-lookup"><span data-stu-id="58fb5-155">String</span></span>|<span data-ttu-id="58fb5-156">ExchangeConnectorAgent 版本</span><span class="sxs-lookup"><span data-stu-id="58fb5-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="58fb5-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="58fb5-157">exchangeAlias</span></span>|<span data-ttu-id="58fb5-158">String</span><span class="sxs-lookup"><span data-stu-id="58fb5-158">String</span></span>|<span data-ttu-id="58fb5-159">分配到 Exchange 服务器的别名</span><span class="sxs-lookup"><span data-stu-id="58fb5-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="58fb5-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="58fb5-160">exchangeOrganization</span></span>|<span data-ttu-id="58fb5-161">String</span><span class="sxs-lookup"><span data-stu-id="58fb5-161">String</span></span>|<span data-ttu-id="58fb5-162">Exchange 服务器的 Exchange 组织</span><span class="sxs-lookup"><span data-stu-id="58fb5-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="58fb5-163">响应</span><span class="sxs-lookup"><span data-stu-id="58fb5-163">Response</span></span>
<span data-ttu-id="58fb5-164">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58fb5-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58fb5-165">示例</span><span class="sxs-lookup"><span data-stu-id="58fb5-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="58fb5-166">请求</span><span class="sxs-lookup"><span data-stu-id="58fb5-166">Request</span></span>
<span data-ttu-id="58fb5-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="58fb5-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58fb5-168">响应</span><span class="sxs-lookup"><span data-stu-id="58fb5-168">Response</span></span>
<span data-ttu-id="58fb5-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="58fb5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



