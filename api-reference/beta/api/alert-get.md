---
title: 获取警报
description: 检索 alert 对象的属性和关系
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 08691cc0122c44703d9a95625c9eabb5d70422fe
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322691"
---
# <a name="get-alert"></a><span data-ttu-id="53d24-103">获取警报</span><span class="sxs-lookup"><span data-stu-id="53d24-103">Get alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53d24-104">检索[alert](../resources/alert.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="53d24-104">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53d24-105">权限</span><span class="sxs-lookup"><span data-stu-id="53d24-105">Permissions</span></span>

<span data-ttu-id="53d24-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53d24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53d24-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="53d24-108">Permission type</span></span>      | <span data-ttu-id="53d24-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53d24-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53d24-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53d24-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="53d24-111">securityevents.readwrite.all、securityevents.readwrite.all 和所有</span><span class="sxs-lookup"><span data-stu-id="53d24-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="53d24-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53d24-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="53d24-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="53d24-113">Not supported.</span></span>  |
|<span data-ttu-id="53d24-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="53d24-114">Application</span></span> | <span data-ttu-id="53d24-115">securityevents.readwrite.all、securityevents.readwrite.all 和所有</span><span class="sxs-lookup"><span data-stu-id="53d24-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53d24-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53d24-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="53d24-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="53d24-117">Request headers</span></span>

| <span data-ttu-id="53d24-118">名称</span><span class="sxs-lookup"><span data-stu-id="53d24-118">Name</span></span>      |<span data-ttu-id="53d24-119">说明</span><span class="sxs-lookup"><span data-stu-id="53d24-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="53d24-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="53d24-120">Authorization</span></span>  | <span data-ttu-id="53d24-121">持有者 {代码}。</span><span class="sxs-lookup"><span data-stu-id="53d24-121">Bearer {code}.</span></span> <span data-ttu-id="53d24-122">必填。</span><span class="sxs-lookup"><span data-stu-id="53d24-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53d24-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="53d24-123">Request body</span></span>

<span data-ttu-id="53d24-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53d24-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53d24-125">响应</span><span class="sxs-lookup"><span data-stu-id="53d24-125">Response</span></span>

<span data-ttu-id="53d24-126">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**alert**对象。</span><span class="sxs-lookup"><span data-stu-id="53d24-126">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="53d24-127">如果从提供程序返回的状态代码或者提供程序超时, 则响应将是一个`206 Partial Content`状态代码, 提供程序的响应在警告标头中。</span><span class="sxs-lookup"><span data-stu-id="53d24-127">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="53d24-128">有关详细信息, 请参阅[Microsoft Graph 安全 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="53d24-128">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="53d24-129">示例</span><span class="sxs-lookup"><span data-stu-id="53d24-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="53d24-130">请求</span><span class="sxs-lookup"><span data-stu-id="53d24-130">Request</span></span>

<span data-ttu-id="53d24-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53d24-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts/{id}
```

### <a name="response"></a><span data-ttu-id="53d24-132">响应</span><span class="sxs-lookup"><span data-stu-id="53d24-132">Response</span></span>

<span data-ttu-id="53d24-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="53d24-133">The following is an example of the response.</span></span>
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
  "historyStates": [
    {
      "appId": "appId-value",
      "assignedTo": "assignedTo-value",
      "comments": [
        "comments-value"
      ],
      "feedback": "feedback-value",
      "status": "status-value",
      "updatedDateTime": "datetime-value",
      "user": "user-value"
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
      "protocol": "String",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get glert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
