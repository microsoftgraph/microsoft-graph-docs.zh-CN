---
title: 获取警报
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: 5f5a7330476de71308680b41e87e51d5d228b2e0
ms.sourcegitcommit: 4aebfaefc23e02a98b2fec35958cd2110020f15f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/06/2018
ms.locfileid: "27184481"
---
# <a name="get-alert"></a><span data-ttu-id="5b16c-104">获取警报</span><span class="sxs-lookup"><span data-stu-id="5b16c-104">Get alert</span></span>

 > <span data-ttu-id="5b16c-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5b16c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b16c-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5b16c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b16c-107">检索的属性和[通知](../resources/alert.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="5b16c-107">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b16c-108">权限</span><span class="sxs-lookup"><span data-stu-id="5b16c-108">Permissions</span></span>

<span data-ttu-id="5b16c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b16c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b16c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b16c-111">Permission type</span></span>      | <span data-ttu-id="5b16c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b16c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b16c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b16c-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="5b16c-114">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b16c-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="5b16c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b16c-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5b16c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b16c-116">Not supported.</span></span>  |
|<span data-ttu-id="5b16c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b16c-117">Application</span></span> | <span data-ttu-id="5b16c-118">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b16c-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b16c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b16c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5b16c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b16c-120">Request headers</span></span>

| <span data-ttu-id="5b16c-121">名称</span><span class="sxs-lookup"><span data-stu-id="5b16c-121">Name</span></span>      |<span data-ttu-id="5b16c-122">说明</span><span class="sxs-lookup"><span data-stu-id="5b16c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5b16c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b16c-123">Authorization</span></span>  | <span data-ttu-id="5b16c-p104">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b16c-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b16c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b16c-126">Request body</span></span>

<span data-ttu-id="5b16c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5b16c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b16c-128">响应</span><span class="sxs-lookup"><span data-stu-id="5b16c-128">Response</span></span>

<span data-ttu-id="5b16c-129">如果成功，此方法返回`200 OK`响应代码和响应正文中的**通知**对象。</span><span class="sxs-lookup"><span data-stu-id="5b16c-129">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="5b16c-130">如果从提供程序返回状态代码之外的 2xx 或 404 或提供程序超时，如果响应将`206 Partial Content`与警告标头中的提供程序的响应状态代码。</span><span class="sxs-lookup"><span data-stu-id="5b16c-130">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="5b16c-131">有关详细信息，请参阅[Microsoft Graph 安全 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="5b16c-131">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="5b16c-132">示例</span><span class="sxs-lookup"><span data-stu-id="5b16c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b16c-133">请求</span><span class="sxs-lookup"><span data-stu-id="5b16c-133">Request</span></span>

<span data-ttu-id="5b16c-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5b16c-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts/{id}
```

### <a name="response"></a><span data-ttu-id="5b16c-135">响应</span><span class="sxs-lookup"><span data-stu-id="5b16c-135">Response</span></span>

<span data-ttu-id="5b16c-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5b16c-136">The following is an example of the response.</span></span>
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
