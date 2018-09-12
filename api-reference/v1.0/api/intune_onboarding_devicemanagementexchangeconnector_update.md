# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="5db71-101">更新 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="5db71-101">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="5db71-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5db71-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5db71-103">更新 [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5db71-103">Update the properties of a [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5db71-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="5db71-104">Prerequisites</span></span>
<span data-ttu-id="5db71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5db71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5db71-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="5db71-107">Permission type</span></span>|<span data-ttu-id="5db71-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5db71-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5db71-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5db71-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5db71-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5db71-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5db71-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5db71-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5db71-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5db71-112">Not supported.</span></span>|
|<span data-ttu-id="5db71-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="5db71-113">Application</span></span>|<span data-ttu-id="5db71-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5db71-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5db71-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5db71-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="5db71-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="5db71-116">Request headers</span></span>
|<span data-ttu-id="5db71-117">标头</span><span class="sxs-lookup"><span data-stu-id="5db71-117">Header</span></span>|<span data-ttu-id="5db71-118">值</span><span class="sxs-lookup"><span data-stu-id="5db71-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5db71-119">授权</span><span class="sxs-lookup"><span data-stu-id="5db71-119">Authorization</span></span>|<span data-ttu-id="5db71-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5db71-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5db71-121">接受</span><span class="sxs-lookup"><span data-stu-id="5db71-121">Accept</span></span>|<span data-ttu-id="5db71-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5db71-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5db71-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5db71-123">Request body</span></span>
<span data-ttu-id="5db71-124">在请求正文中，提供 [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5db71-124">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="5db71-125">下表显示创建 [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5db71-125">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="5db71-126">属性</span><span class="sxs-lookup"><span data-stu-id="5db71-126">Property</span></span>|<span data-ttu-id="5db71-127">类型</span><span class="sxs-lookup"><span data-stu-id="5db71-127">Type</span></span>|<span data-ttu-id="5db71-128">说明</span><span class="sxs-lookup"><span data-stu-id="5db71-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5db71-129">ID</span><span class="sxs-lookup"><span data-stu-id="5db71-129">id</span></span>|<span data-ttu-id="5db71-130">字符串</span><span class="sxs-lookup"><span data-stu-id="5db71-130">String</span></span>|<span data-ttu-id="5db71-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5db71-131">Not yet documented</span></span>|
|<span data-ttu-id="5db71-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5db71-132">lastSyncDateTime</span></span>|<span data-ttu-id="5db71-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5db71-133">DateTimeOffset</span></span>|<span data-ttu-id="5db71-134">Exchange Connector 的上一次同步时间</span><span class="sxs-lookup"><span data-stu-id="5db71-134">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="5db71-135">status</span><span class="sxs-lookup"><span data-stu-id="5db71-135">status</span></span>|[<span data-ttu-id="5db71-136">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="5db71-136">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune_onboarding_devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="5db71-p102">Exchange 连接器状态。 可取值为：`none`、`connectionPending`、`connected`、`disconnected`。</span><span class="sxs-lookup"><span data-stu-id="5db71-p102">Exchange Connector Status Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="5db71-139">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="5db71-139">primarySmtpAddress</span></span>|<span data-ttu-id="5db71-140">字符串</span><span class="sxs-lookup"><span data-stu-id="5db71-140">String</span></span>|<span data-ttu-id="5db71-141">用于配置服务到服务 Exchange Connector 的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5db71-141">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="5db71-142">serverName</span><span class="sxs-lookup"><span data-stu-id="5db71-142">serverName</span></span>|<span data-ttu-id="5db71-143">字符串</span><span class="sxs-lookup"><span data-stu-id="5db71-143">String</span></span>|<span data-ttu-id="5db71-144">Exchange Server 名称。</span><span class="sxs-lookup"><span data-stu-id="5db71-144">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="5db71-145">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="5db71-145">connectorServerName</span></span>|<span data-ttu-id="5db71-146">字符串</span><span class="sxs-lookup"><span data-stu-id="5db71-146">String</span></span>|<span data-ttu-id="5db71-147">托管 Exchange Connector 的服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="5db71-147">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="5db71-148">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="5db71-148">exchangeConnectorType</span></span>|[<span data-ttu-id="5db71-149">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="5db71-149">deviceManagementExchangeConnectorType</span></span>](../resources/intune_onboarding_devicemanagementexchangeconnectortype.md)|<span data-ttu-id="5db71-p103">配置的 Exchange 连接器的类型。 可取值为：`onPremises`、`hosted`、`serviceToService`、`dedicated`。</span><span class="sxs-lookup"><span data-stu-id="5db71-p103">The type of Exchange Connector Configured. The possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="5db71-152">version</span><span class="sxs-lookup"><span data-stu-id="5db71-152">version</span></span>|<span data-ttu-id="5db71-153">字符串</span><span class="sxs-lookup"><span data-stu-id="5db71-153">String</span></span>|<span data-ttu-id="5db71-154">ExchangeConnectorAgent 版本</span><span class="sxs-lookup"><span data-stu-id="5db71-154">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="5db71-155">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="5db71-155">exchangeAlias</span></span>|<span data-ttu-id="5db71-156">字符串</span><span class="sxs-lookup"><span data-stu-id="5db71-156">String</span></span>|<span data-ttu-id="5db71-157">分配到 Exchange 服务器的别名</span><span class="sxs-lookup"><span data-stu-id="5db71-157">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="5db71-158">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="5db71-158">exchangeOrganization</span></span>|<span data-ttu-id="5db71-159">字符串</span><span class="sxs-lookup"><span data-stu-id="5db71-159">String</span></span>|<span data-ttu-id="5db71-160">Exchange 服务器的 Exchange 组织</span><span class="sxs-lookup"><span data-stu-id="5db71-160">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="5db71-161">响应</span><span class="sxs-lookup"><span data-stu-id="5db71-161">Response</span></span>
<span data-ttu-id="5db71-162">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5db71-162">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5db71-163">示例</span><span class="sxs-lookup"><span data-stu-id="5db71-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="5db71-164">请求</span><span class="sxs-lookup"><span data-stu-id="5db71-164">Request</span></span>
<span data-ttu-id="5db71-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5db71-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
Content-type: application/json
Content-length: 418

{
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

### <a name="response"></a><span data-ttu-id="5db71-166">响应</span><span class="sxs-lookup"><span data-stu-id="5db71-166">Response</span></span>
<span data-ttu-id="5db71-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5db71-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








