---
title: 更新 deviceManagementExchangeConnector
description: 更新 deviceManagementExchangeConnector 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3f7a656e2959e7afc40639a00f7373fb2aa3811d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075096"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="73804-103">更新 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="73804-103">Update deviceManagementExchangeConnector</span></span>

<span data-ttu-id="73804-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73804-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73804-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73804-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73804-106">更新 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="73804-106">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73804-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="73804-107">Prerequisites</span></span>
<span data-ttu-id="73804-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73804-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73804-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="73804-110">Permission type</span></span>|<span data-ttu-id="73804-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="73804-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73804-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73804-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73804-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73804-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="73804-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73804-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73804-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="73804-115">Not supported.</span></span>|
|<span data-ttu-id="73804-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="73804-116">Application</span></span>|<span data-ttu-id="73804-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="73804-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73804-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73804-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="73804-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="73804-119">Request headers</span></span>
|<span data-ttu-id="73804-120">标头</span><span class="sxs-lookup"><span data-stu-id="73804-120">Header</span></span>|<span data-ttu-id="73804-121">值</span><span class="sxs-lookup"><span data-stu-id="73804-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73804-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73804-122">Authorization</span></span>|<span data-ttu-id="73804-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="73804-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73804-124">接受</span><span class="sxs-lookup"><span data-stu-id="73804-124">Accept</span></span>|<span data-ttu-id="73804-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73804-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73804-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="73804-126">Request body</span></span>
<span data-ttu-id="73804-127">在请求正文中，提供 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73804-127">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="73804-128">下表显示创建 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="73804-128">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="73804-129">属性</span><span class="sxs-lookup"><span data-stu-id="73804-129">Property</span></span>|<span data-ttu-id="73804-130">类型</span><span class="sxs-lookup"><span data-stu-id="73804-130">Type</span></span>|<span data-ttu-id="73804-131">说明</span><span class="sxs-lookup"><span data-stu-id="73804-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73804-132">id</span><span class="sxs-lookup"><span data-stu-id="73804-132">id</span></span>|<span data-ttu-id="73804-133">String</span><span class="sxs-lookup"><span data-stu-id="73804-133">String</span></span>|<span data-ttu-id="73804-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="73804-134">Not yet documented</span></span>|
|<span data-ttu-id="73804-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="73804-135">lastSyncDateTime</span></span>|<span data-ttu-id="73804-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73804-136">DateTimeOffset</span></span>|<span data-ttu-id="73804-137">Exchange Connector 的上一次同步时间</span><span class="sxs-lookup"><span data-stu-id="73804-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="73804-138">status</span><span class="sxs-lookup"><span data-stu-id="73804-138">status</span></span>|[<span data-ttu-id="73804-139">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="73804-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="73804-140">Exchange Connector 状态。</span><span class="sxs-lookup"><span data-stu-id="73804-140">Exchange Connector Status.</span></span> <span data-ttu-id="73804-141">可取值为：`none`、`connectionPending`、`connected`、`disconnected`。</span><span class="sxs-lookup"><span data-stu-id="73804-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="73804-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="73804-142">primarySmtpAddress</span></span>|<span data-ttu-id="73804-143">String</span><span class="sxs-lookup"><span data-stu-id="73804-143">String</span></span>|<span data-ttu-id="73804-144">用于配置服务到服务 Exchange Connector 的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="73804-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="73804-145">serverName</span><span class="sxs-lookup"><span data-stu-id="73804-145">serverName</span></span>|<span data-ttu-id="73804-146">String</span><span class="sxs-lookup"><span data-stu-id="73804-146">String</span></span>|<span data-ttu-id="73804-147">Exchange 服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="73804-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="73804-148">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="73804-148">connectorServerName</span></span>|<span data-ttu-id="73804-149">String</span><span class="sxs-lookup"><span data-stu-id="73804-149">String</span></span>|<span data-ttu-id="73804-150">托管 Exchange Connector 的服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="73804-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="73804-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="73804-151">exchangeConnectorType</span></span>|[<span data-ttu-id="73804-152">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="73804-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="73804-153">配置的 Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="73804-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="73804-154">可取值为：`onPremises`、`hosted`、`serviceToService`、`dedicated`。</span><span class="sxs-lookup"><span data-stu-id="73804-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="73804-155">version</span><span class="sxs-lookup"><span data-stu-id="73804-155">version</span></span>|<span data-ttu-id="73804-156">String</span><span class="sxs-lookup"><span data-stu-id="73804-156">String</span></span>|<span data-ttu-id="73804-157">ExchangeConnectorAgent 版本</span><span class="sxs-lookup"><span data-stu-id="73804-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="73804-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="73804-158">exchangeAlias</span></span>|<span data-ttu-id="73804-159">String</span><span class="sxs-lookup"><span data-stu-id="73804-159">String</span></span>|<span data-ttu-id="73804-160">分配到 Exchange 服务器的别名</span><span class="sxs-lookup"><span data-stu-id="73804-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="73804-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="73804-161">exchangeOrganization</span></span>|<span data-ttu-id="73804-162">String</span><span class="sxs-lookup"><span data-stu-id="73804-162">String</span></span>|<span data-ttu-id="73804-163">Exchange 服务器的 Exchange 组织</span><span class="sxs-lookup"><span data-stu-id="73804-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="73804-164">响应</span><span class="sxs-lookup"><span data-stu-id="73804-164">Response</span></span>
<span data-ttu-id="73804-165">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73804-165">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73804-166">示例</span><span class="sxs-lookup"><span data-stu-id="73804-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="73804-167">请求</span><span class="sxs-lookup"><span data-stu-id="73804-167">Request</span></span>
<span data-ttu-id="73804-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73804-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="73804-169">响应</span><span class="sxs-lookup"><span data-stu-id="73804-169">Response</span></span>
<span data-ttu-id="73804-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73804-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









