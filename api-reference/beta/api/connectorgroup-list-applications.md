---
title: 列出应用程序
description: 检索与 connectorGroup 相关联的 application 对象的列表。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a79db391761220f8bae7cfd3c81fe210ce8926e3
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681405"
---
# <a name="list-applications-assigned-to-a-connectorgroup"></a><span data-ttu-id="ef262-103">列出分配给 connectorGroup 的应用程序</span><span class="sxs-lookup"><span data-stu-id="ef262-103">List applications assigned to a connectorGroup</span></span>

<span data-ttu-id="ef262-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef262-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef262-105">检索与[connectorGroup](../resources/connectorgroup.md)相关联的[application](../resources/application.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ef262-105">Retrieve a list of [application](../resources/application.md) objects associated with the [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="ef262-106">此列表包含分配给特定连接器组的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="ef262-106">This list contains all applications assigned to the specific connector group.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef262-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ef262-107">Permissions</span></span>
<span data-ttu-id="ef262-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef262-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef262-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef262-110">Permission type</span></span>      | <span data-ttu-id="ef262-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ef262-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef262-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef262-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ef262-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ef262-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ef262-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef262-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef262-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef262-115">Not supported.</span></span>    |
|<span data-ttu-id="ef262-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef262-116">Application</span></span> | <span data-ttu-id="ef262-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef262-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ef262-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef262-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ef262-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ef262-119">Optional query parameters</span></span>
<span data-ttu-id="ef262-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ef262-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef262-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef262-121">Request headers</span></span>
| <span data-ttu-id="ef262-122">名称</span><span class="sxs-lookup"><span data-stu-id="ef262-122">Name</span></span>      |<span data-ttu-id="ef262-123">说明</span><span class="sxs-lookup"><span data-stu-id="ef262-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ef262-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef262-124">Authorization</span></span>  | <span data-ttu-id="ef262-125">负载.</span><span class="sxs-lookup"><span data-stu-id="ef262-125">Bearer.</span></span> <span data-ttu-id="ef262-126">必需</span><span class="sxs-lookup"><span data-stu-id="ef262-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef262-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef262-127">Request body</span></span>
<span data-ttu-id="ef262-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ef262-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef262-129">响应</span><span class="sxs-lookup"><span data-stu-id="ef262-129">Response</span></span>

<span data-ttu-id="ef262-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[application](../resources/application.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ef262-130">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef262-131">示例</span><span class="sxs-lookup"><span data-stu-id="ef262-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef262-132">请求</span><span class="sxs-lookup"><span data-stu-id="ef262-132">Request</span></span>
<span data-ttu-id="ef262-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ef262-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ef262-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef262-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
# <a name="c"></a>[<span data-ttu-id="ef262-135">C#</span><span class="sxs-lookup"><span data-stu-id="ef262-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef262-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef262-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef262-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef262-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ef262-138">响应</span><span class="sxs-lookup"><span data-stu-id="ef262-138">Response</span></span>
<span data-ttu-id="ef262-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ef262-139">The following is an example of the response.</span></span> <span data-ttu-id="ef262-140">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ef262-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ef262-141">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ef262-141">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 420

{
  "value": [
    {
      "id": "id-value",
      "onPremisesPublishing": {
        "externalUrl": "externalUrl-value",
        "internalUrl": "internalUrl-value",
        "externalAuthenticationType": "externalAuthenticationType-value",
        "isTranslateHostHeaderEnabled": true,
        "isTranslateLinksInBodyEnabled": true,
        "isOnPremPublishingEnabled": true,
        "applicationServerTimeout": "applicationServerTimeout-value",
        "applicationType": "applicationType-value",
        "verifiedCustomDomainKeyCredential": {
          "customKeyIdentifier": "customKeyIdentifier-value",
          "endDate": "datetime-value",
          "keyId": "keyId-value",
          "startDate": "datetime-value",
          "type": "type-value",
          "usage": "usage-value",
          "value": "value-value"
        },
        "verifiedCustomDomainPasswordCredential": {
          "customKeyIdentifier": "customKeyIdentifier-value",
          "endDate": "datetime-value",
          "keyId": "keyId-value",
          "startDate": "datetime-value",
          "value": "value-value"
        },
        "verifiedCustomDomainCertificatesMetadata": {
          "thumbprint": "thumbprint-value",
          "subjectName": "subjectName-value",
          "issuerName": "issuerName-value",
          "issueDate": "datetime-value",
          "expiryDate": "datetime-value"
        },
        "singleSignOnSettings": {
          "SingleSignOnMode": "SingleSignOnMode-value",
          "KerberosSignOnSettings": {
            "KerberosServicePrincipalName": "KerberosServicePrincipalName-value",
            "KerberosSignOnMappingAttributeType": "KerberosSignOnMappingAttributeType-value"
          }
        },
        "isHttpOnlyCookieEnabled": true,
        "isSecureCookieEnabled": true,
        "isPersistentCookieEnabled": true
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
