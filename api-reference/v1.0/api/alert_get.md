# <a name="get-alert"></a><span data-ttu-id="186ce-101">Get alert</span><span class="sxs-lookup"><span data-stu-id="186ce-101">Get alert</span></span>

 <span data-ttu-id="186ce-102">检索 [alert](../resources/alert.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="186ce-102">Retrieve the properties and relationships of [plannertaskdetails](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="186ce-103">权限</span><span class="sxs-lookup"><span data-stu-id="186ce-103">Permissions</span></span>

<span data-ttu-id="186ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="186ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="186ce-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="186ce-106">Permission type</span></span>      | <span data-ttu-id="186ce-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="186ce-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="186ce-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="186ce-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="186ce-109">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="186ce-109">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="186ce-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="186ce-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="186ce-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="186ce-111">Not supported.</span></span>  |
|<span data-ttu-id="186ce-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="186ce-112">Application</span></span> | <span data-ttu-id="186ce-113">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="186ce-113">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="186ce-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="186ce-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="186ce-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="186ce-115">Request headers</span></span>

| <span data-ttu-id="186ce-116">名称</span><span class="sxs-lookup"><span data-stu-id="186ce-116">Name</span></span>      |<span data-ttu-id="186ce-117">说明</span><span class="sxs-lookup"><span data-stu-id="186ce-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="186ce-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="186ce-118">Authorization</span></span>  | <span data-ttu-id="186ce-p102">持有者 {代码}。必填。</span><span class="sxs-lookup"><span data-stu-id="186ce-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="186ce-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="186ce-121">Request body</span></span>

<span data-ttu-id="186ce-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="186ce-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="186ce-123">响应</span><span class="sxs-lookup"><span data-stu-id="186ce-123">Response</span></span>

<span data-ttu-id="186ce-124">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 **alert** 对象。</span><span class="sxs-lookup"><span data-stu-id="186ce-124">If successful, this method returns a `200 OK` response code and an updated **windows10CompliancePolicy** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="186ce-125">示例</span><span class="sxs-lookup"><span data-stu-id="186ce-125">Example</span></span>

### <a name="request"></a><span data-ttu-id="186ce-126">请求</span><span class="sxs-lookup"><span data-stu-id="186ce-126">Request</span></span>

<span data-ttu-id="186ce-127">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="186ce-127">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
```

### <a name="response"></a><span data-ttu-id="186ce-128">响应</span><span class="sxs-lookup"><span data-stu-id="186ce-128">Response</span></span>

<span data-ttu-id="186ce-129">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="186ce-129">The following is an example of the response.</span></span>
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
