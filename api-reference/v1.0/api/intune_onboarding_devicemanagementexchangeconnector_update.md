# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="1f19c-101">更新 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="1f19c-101">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="1f19c-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1f19c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f19c-103">更新 [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1f19c-103">Update the properties of a [calendar](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f19c-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="1f19c-104">Prerequisites</span></span>
<span data-ttu-id="1f19c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1f19c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1f19c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f19c-107">Permission type</span></span>|<span data-ttu-id="1f19c-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1f19c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f19c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f19c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1f19c-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f19c-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1f19c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f19c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f19c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f19c-112">Not supported.</span></span>|
|<span data-ttu-id="1f19c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f19c-113">Application</span></span>|<span data-ttu-id="1f19c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f19c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f19c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f19c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="1f19c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f19c-116">Request headers</span></span>
|<span data-ttu-id="1f19c-117">标头</span><span class="sxs-lookup"><span data-stu-id="1f19c-117">Header</span></span>|<span data-ttu-id="1f19c-118">值</span><span class="sxs-lookup"><span data-stu-id="1f19c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f19c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f19c-119">Authorization</span></span>|<span data-ttu-id="1f19c-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1f19c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1f19c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1f19c-121">Accept</span></span>|<span data-ttu-id="1f19c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1f19c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f19c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f19c-123">Request body</span></span>
<span data-ttu-id="1f19c-124">在请求正文中，提供 [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f19c-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="1f19c-125">下表显示创建 [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1f19c-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="1f19c-126">属性</span><span class="sxs-lookup"><span data-stu-id="1f19c-126">Property</span></span>|<span data-ttu-id="1f19c-127">类型</span><span class="sxs-lookup"><span data-stu-id="1f19c-127">Type</span></span>|<span data-ttu-id="1f19c-128">说明</span><span class="sxs-lookup"><span data-stu-id="1f19c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f19c-129">id</span><span class="sxs-lookup"><span data-stu-id="1f19c-129">id</span></span>|<span data-ttu-id="1f19c-130">String</span><span class="sxs-lookup"><span data-stu-id="1f19c-130">String</span></span>|<span data-ttu-id="1f19c-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1f19c-131">Not yet documented</span></span>|
|<span data-ttu-id="1f19c-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1f19c-132">lastSyncDateTime</span></span>|<span data-ttu-id="1f19c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f19c-133">DateTimeOffset</span></span>|<span data-ttu-id="1f19c-134">Exchange Connector 的上一次同步时间</span><span class="sxs-lookup"><span data-stu-id="1f19c-134">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="1f19c-135">status</span><span class="sxs-lookup"><span data-stu-id="1f19c-135">status</span></span>|<span data-ttu-id="1f19c-136">String</span><span class="sxs-lookup"><span data-stu-id="1f19c-136">String</span></span>|<span data-ttu-id="1f19c-137">Exchange Connector 状态。可取值为：`none`、`connectionPending`、`connected`、`disconnected`。</span><span class="sxs-lookup"><span data-stu-id="1f19c-137">Exchange Connector Status Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="1f19c-138">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1f19c-138">primarySmtpAddress</span></span>|<span data-ttu-id="1f19c-139">String</span><span class="sxs-lookup"><span data-stu-id="1f19c-139">String</span></span>|<span data-ttu-id="1f19c-140">用于配置服务到服务 Exchange Connector 的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1f19c-140">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="1f19c-141">serverName</span><span class="sxs-lookup"><span data-stu-id="1f19c-141">ServerName</span></span>|<span data-ttu-id="1f19c-142">String</span><span class="sxs-lookup"><span data-stu-id="1f19c-142">String</span></span>|<span data-ttu-id="1f19c-143">托管 Exchange Connector 的服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="1f19c-143">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="1f19c-144">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="1f19c-144">exchangeConnectorType</span></span>|<span data-ttu-id="1f19c-145">String</span><span class="sxs-lookup"><span data-stu-id="1f19c-145">String</span></span>|<span data-ttu-id="1f19c-146">配置的 Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="1f19c-146">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="1f19c-147">可取值为：`onPremises`、`hosted`、`serviceToService`、`dedicated`。</span><span class="sxs-lookup"><span data-stu-id="1f19c-147">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="1f19c-148">version</span><span class="sxs-lookup"><span data-stu-id="1f19c-148">version</span></span>|<span data-ttu-id="1f19c-149">String</span><span class="sxs-lookup"><span data-stu-id="1f19c-149">String</span></span>|<span data-ttu-id="1f19c-150">ExchangeConnectorAgent 版本</span><span class="sxs-lookup"><span data-stu-id="1f19c-150">The version of the message.</span></span>|
|<span data-ttu-id="1f19c-151">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="1f19c-151">exchangeAlias</span></span>|<span data-ttu-id="1f19c-152">String</span><span class="sxs-lookup"><span data-stu-id="1f19c-152">String</span></span>|<span data-ttu-id="1f19c-153">分配到 Exchange 服务器的别名</span><span class="sxs-lookup"><span data-stu-id="1f19c-153">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="1f19c-154">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="1f19c-154">exchangeOrganization</span></span>|<span data-ttu-id="1f19c-155">String</span><span class="sxs-lookup"><span data-stu-id="1f19c-155">String</span></span>|<span data-ttu-id="1f19c-156">Exchange 服务器的 Exchange 组织</span><span class="sxs-lookup"><span data-stu-id="1f19c-156">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="1f19c-157">响应</span><span class="sxs-lookup"><span data-stu-id="1f19c-157">Response</span></span>
<span data-ttu-id="1f19c-158">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f19c-158">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f19c-159">示例</span><span class="sxs-lookup"><span data-stu-id="1f19c-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f19c-160">请求</span><span class="sxs-lookup"><span data-stu-id="1f19c-160">Request</span></span>
<span data-ttu-id="1f19c-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1f19c-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
Content-type: application/json
Content-length: 361

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="1f19c-162">响应</span><span class="sxs-lookup"><span data-stu-id="1f19c-162">Response</span></span>
<span data-ttu-id="1f19c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1f19c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 482

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```



