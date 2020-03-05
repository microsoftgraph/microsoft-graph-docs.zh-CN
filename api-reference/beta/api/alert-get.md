---
title: 获取警报
description: 检索 alert 对象的属性和关系
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 3bcb4d9c198d4b53e589322d0f597cfb5fd88350
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441625"
---
# <a name="get-alert"></a><span data-ttu-id="421f5-103">获取警报</span><span class="sxs-lookup"><span data-stu-id="421f5-103">Get alert</span></span>

<span data-ttu-id="421f5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="421f5-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="421f5-105">检索[alert](../resources/alert.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="421f5-105">Retrieve the properties and relationships of an [alert](../resources/alert.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="421f5-106">权限</span><span class="sxs-lookup"><span data-stu-id="421f5-106">Permissions</span></span>

<span data-ttu-id="421f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="421f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="421f5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="421f5-109">Permission type</span></span>      | <span data-ttu-id="421f5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="421f5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="421f5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="421f5-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="421f5-112">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="421f5-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="421f5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="421f5-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="421f5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="421f5-114">Not supported.</span></span>  |
|<span data-ttu-id="421f5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="421f5-115">Application</span></span> | <span data-ttu-id="421f5-116">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="421f5-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="421f5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="421f5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="421f5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="421f5-118">Request headers</span></span>

| <span data-ttu-id="421f5-119">名称</span><span class="sxs-lookup"><span data-stu-id="421f5-119">Name</span></span>      |<span data-ttu-id="421f5-120">说明</span><span class="sxs-lookup"><span data-stu-id="421f5-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="421f5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="421f5-121">Authorization</span></span>  | <span data-ttu-id="421f5-122">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="421f5-122">Bearer {code}.</span></span> <span data-ttu-id="421f5-123">必需。</span><span class="sxs-lookup"><span data-stu-id="421f5-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="421f5-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="421f5-124">Request body</span></span>

<span data-ttu-id="421f5-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="421f5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="421f5-126">响应</span><span class="sxs-lookup"><span data-stu-id="421f5-126">Response</span></span>

<span data-ttu-id="421f5-127">如果成功，此方法在响应`200 OK`正文中返回响应代码和**alert**对象。</span><span class="sxs-lookup"><span data-stu-id="421f5-127">If successful, this method returns a `200 OK` response code and an **alert** object in the response body.</span></span> <span data-ttu-id="421f5-128">如果从提供程序返回了 2xx 或 404 以外的状态代码，或者提供程序超时，则响应将是 `206 Partial Content` 状态代码，提供程序的响应位于警告标头中。</span><span class="sxs-lookup"><span data-stu-id="421f5-128">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="421f5-129">有关详细信息，请参阅 [Microsoft Graph 安全性 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="421f5-129">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="421f5-130">示例</span><span class="sxs-lookup"><span data-stu-id="421f5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="421f5-131">请求</span><span class="sxs-lookup"><span data-stu-id="421f5-131">Request</span></span>

<span data-ttu-id="421f5-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="421f5-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="421f5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="421f5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alert"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/alerts/{id}
```
# <a name="c"></a>[<span data-ttu-id="421f5-134">C#</span><span class="sxs-lookup"><span data-stu-id="421f5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="421f5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="421f5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="421f5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="421f5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="421f5-137">响应</span><span class="sxs-lookup"><span data-stu-id="421f5-137">Response</span></span>

<span data-ttu-id="421f5-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="421f5-138">The following is an example of the response.</span></span>
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
  "suppressions": [
  ]
}
-->
