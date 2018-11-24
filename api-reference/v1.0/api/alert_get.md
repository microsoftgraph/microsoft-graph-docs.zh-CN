# <a name="get-alert"></a><span data-ttu-id="16bb6-101">获取警报</span><span class="sxs-lookup"><span data-stu-id="16bb6-101">Get alert</span></span>

 <span data-ttu-id="16bb6-102">检索的属性和[通知](../resources/alert.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="16bb6-102">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="16bb6-103">权限</span><span class="sxs-lookup"><span data-stu-id="16bb6-103">Permissions</span></span>

<span data-ttu-id="16bb6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="16bb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="16bb6-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="16bb6-106">Permission type</span></span>      | <span data-ttu-id="16bb6-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16bb6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16bb6-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16bb6-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="16bb6-109">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16bb6-109">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="16bb6-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16bb6-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="16bb6-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="16bb6-111">Not supported.</span></span>  |
|<span data-ttu-id="16bb6-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="16bb6-112">Application</span></span> | <span data-ttu-id="16bb6-113">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16bb6-113">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16bb6-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16bb6-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="16bb6-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="16bb6-115">Request headers</span></span>

| <span data-ttu-id="16bb6-116">名称</span><span class="sxs-lookup"><span data-stu-id="16bb6-116">Name</span></span>      |<span data-ttu-id="16bb6-117">说明</span><span class="sxs-lookup"><span data-stu-id="16bb6-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="16bb6-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="16bb6-118">Authorization</span></span>  | <span data-ttu-id="16bb6-p102">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="16bb6-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16bb6-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="16bb6-121">Request body</span></span>

<span data-ttu-id="16bb6-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16bb6-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16bb6-123">响应</span><span class="sxs-lookup"><span data-stu-id="16bb6-123">Response</span></span>

<span data-ttu-id="16bb6-124">如果成功，此方法返回`200 OK`响应代码和响应正文中的**通知**对象。</span><span class="sxs-lookup"><span data-stu-id="16bb6-124">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="16bb6-125">如果从提供程序返回状态代码之外的 2xx 或 404 或提供程序超时，如果响应将`206 Partial Content`与提供程序响应警告标头中的状态代码。</span><span class="sxs-lookup"><span data-stu-id="16bb6-125">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the providers response in a warning header.</span></span> <span data-ttu-id="16bb6-126">有关详细信息，请参阅[Microsoft Graph 安全 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="16bb6-126">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="16bb6-127">示例</span><span class="sxs-lookup"><span data-stu-id="16bb6-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="16bb6-128">请求</span><span class="sxs-lookup"><span data-stu-id="16bb6-128">Request</span></span>

<span data-ttu-id="16bb6-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="16bb6-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
```

### <a name="response"></a><span data-ttu-id="16bb6-130">响应</span><span class="sxs-lookup"><span data-stu-id="16bb6-130">Response</span></span>

<span data-ttu-id="16bb6-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="16bb6-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [
    {
      "destinationServiceIp": "String",
      "destinationServiceName": "String",
      "riskScore": "String"
    }
  ],
  "comments": ["String"],
  "confidence": 1024,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": ["String"],
  "eventDateTime": "String (timestamp)",
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "fileStates": [
    {
      "fileHash": {
        "hashType": "@odata.type: microsoft.graph.fileHashType",
        "hashValue": "String"
      },
      "name": "String",
      "path": "String",
      "riskScore": "String"
    }
  ],
  "hostStates": [
    {
      "fqdn": "String",
      "isAzureAadJoined": true,
      "isAzureAadRegistered": true,
      "isHybridAzureDomainJoined": true,
      "netBiosName": "String",
      "os": "String",
      "privateIpAddress": "String",
      "publicIpAddress": "String",
      "riskScore": "String"
    }
  ],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [
    {
      "category": "String",
      "family": "String",
      "name": "String",
      "severity": "String",
      "wasRunning": true
    }
  ],
  "networkConnections": [
    {
      "applicationName": "String",
      "destinationAddress": "String",
      "destinationDomain": "String",
      "destinationPort": "String",
      "destinationUrl": "String",
      "direction": "@odata.type: microsoft.graph.connectionDirection",
      "domainRegisteredDateTime": "String (timestamp)",
      "localDnsName": "String",
      "natDestinationAddress": "String",
      "natDestinationPort": "String",
      "natSourceAddress": "String",
      "natSourcePort": "String",
      "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
      "riskScore": "String",
      "sourceAddress": "String",
      "sourcePort": "String",
      "status": "@odata.type: microsoft.graph.connectionStatus",
      "urlParameters": "String"
    }
  ],
  "processes": [
    {
      "accountName": "String",
      "commandLine": "String",
      "createdDateTime": "String (timestamp)",
      "fileHash": {
        "hashType": "@odata.type: microsoft.graph.fileHashType",
        "hashValue": "String"
      },
      "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
      "isElevated": true,
      "name": "String",
      "parentProcessCreatedDateTime": "String (timestamp)",
      "parentProcessId": 1024,
      "parentProcessName": "String",
      "path": "String",
      "processId": 1024
    }
  ],
  "recommendedActions": ["String"],
  "registryKeyStates": [
    {
      "hive": "@odata.type: microsoft.graph.registryHive",
      "key": "String",
      "oldKey": "String",
      "oldValueData": "String",
      "oldValueName": "String",
      "operation": "@odata.type: microsoft.graph.registryOperation",
      "processId": 1024,
      "valueData": "String",
      "valueName": "String",
      "valueType": "@odata.type: microsoft.graph.registryValueType"
    }
  ],
  "severity": "@odata.type: microsoft.graph.alertSeverity",
  "sourceMaterials": ["String"],
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "title": "String",
  "triggers": [
    {
      "name": "String",
      "type": "String",
      "value": "String"
    }
  ],
  "userStates": [
    {
      "aadUserId": "String",
      "accountName": "String",
      "domainName": "String",
      "emailRole": "@odata.type: microsoft.graph.emailRole",
      "isVpn": true,
      "logonDateTime": "String (timestamp)",
      "logonId": "String",
      "logonIp": "String",
      "logonLocation": "String",
      "logonType": "@odata.type: microsoft.graph.logonType",
      "onPremisesSecurityIdentifier": "String",
      "riskScore": "String",
      "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
      "userPrincipalName": "String"
    }
  ],
  "vendorInformation": {
    "provider": "String",
    "providerVersion": "String",
    "subProvider": "String",
    "vendor": "String"
  },
  "vulnerabilityStates": [
    {
      "cve": "String",
      "severity": "String",
      "wasRunning": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get glert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
