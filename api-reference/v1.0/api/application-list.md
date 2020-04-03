---
title: 列出应用程序
description: 获取该组织中应用程序的列表。
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9a12773de45e8f79fca57d17df1668ccd3a32c9d
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108373"
---
# <a name="list-applications"></a><span data-ttu-id="0fc0e-103">列出应用程序</span><span class="sxs-lookup"><span data-stu-id="0fc0e-103">List applications</span></span>

<span data-ttu-id="0fc0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fc0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0fc0e-105">获取该组织中[应用程序](../resources/application.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="0fc0e-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fc0e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0fc0e-106">Permissions</span></span>
<span data-ttu-id="0fc0e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0fc0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0fc0e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0fc0e-109">Permission type</span></span>      | <span data-ttu-id="0fc0e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0fc0e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fc0e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0fc0e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0fc0e-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0fc0e-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0fc0e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0fc0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fc0e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0fc0e-114">Not supported.</span></span>    |
|<span data-ttu-id="0fc0e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0fc0e-115">Application</span></span> | <span data-ttu-id="0fc0e-116">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fc0e-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fc0e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0fc0e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0fc0e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0fc0e-118">Optional query parameters</span></span>
<span data-ttu-id="0fc0e-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0fc0e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fc0e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0fc0e-120">Request headers</span></span>
| <span data-ttu-id="0fc0e-121">名称</span><span class="sxs-lookup"><span data-stu-id="0fc0e-121">Name</span></span>       | <span data-ttu-id="0fc0e-122">类型</span><span class="sxs-lookup"><span data-stu-id="0fc0e-122">Type</span></span> | <span data-ttu-id="0fc0e-123">说明</span><span class="sxs-lookup"><span data-stu-id="0fc0e-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0fc0e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fc0e-124">Authorization</span></span>  | <span data-ttu-id="0fc0e-125">string</span><span class="sxs-lookup"><span data-stu-id="0fc0e-125">string</span></span>  | <span data-ttu-id="0fc0e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0fc0e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0fc0e-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="0fc0e-128">Content-type</span></span>   | <span data-ttu-id="0fc0e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fc0e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="0fc0e-131">Request body</span></span>
<span data-ttu-id="0fc0e-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0fc0e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fc0e-133">响应</span><span class="sxs-lookup"><span data-stu-id="0fc0e-133">Response</span></span>

<span data-ttu-id="0fc0e-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [application](../resources/application.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0fc0e-134">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="0fc0e-135">示例</span><span class="sxs-lookup"><span data-stu-id="0fc0e-135">Examples</span></span>
### <a name="request"></a><span data-ttu-id="0fc0e-136">请求</span><span class="sxs-lookup"><span data-stu-id="0fc0e-136">Request</span></span>
<span data-ttu-id="0fc0e-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0fc0e-137">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0fc0e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fc0e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications
```
# <a name="c"></a>[<span data-ttu-id="0fc0e-139">C#</span><span class="sxs-lookup"><span data-stu-id="0fc0e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fc0e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fc0e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fc0e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fc0e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fc0e-142">Java</span><span class="sxs-lookup"><span data-stu-id="0fc0e-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0fc0e-143">响应</span><span class="sxs-lookup"><span data-stu-id="0fc0e-143">Response</span></span>
<span data-ttu-id="0fc0e-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0fc0e-144">Here is an example of the response.</span></span> 

> <span data-ttu-id="0fc0e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0fc0e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1229

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications",
    "value": [
        {
            "id": "00af5dfb-85da-4b41-a677-0c6b86dd34f8",
            "deletedDateTime": null,
            "isFallbackPublicClient": false,
            "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
            "applicationTemplateId": null,
            "identifierUris": [
                "http://contoso/a7770d29-4321-41a6-b863-ca11d6639448"
            ],
            "createdDateTime": "2019-09-15T05:23:08Z",
            "displayName": "My app",
            "isDeviceOnlyAuthSupported": null,
            "groupMembershipClaims": null,
            "optionalClaims": null,
            "orgRestrictions": [],
            "publisherDomain": "contoso.onmicrosoft.com",
            "signInAudience": "AzureADMyOrg",
            "tags": [],
            "tokenEncryptionKeyId": null,
            "api": {
                "requestedAccessTokenVersion": null,
                "acceptMappedClaims": null,
                "knownClientApplications": [],
                "oauth2PermissionScopes": [],
                "preAuthorizedApplications": []
            },
            "appRoles": [],
            "publicClient": {
                "redirectUris": []
            },
            "info": {
                "termsOfServiceUrl": null,
                "supportUrl": null,
                "privacyStatementUrl": null,
                "marketingUrl": null,
                "logoUrl": null
            },
            "keyCredentials": [],
            "parentalControlSettings": {
                "countriesBlockedForMinors": [],
                "legalAgeGroupRule": "Allow"
            },
            "passwordCredentials": [],
            "requiredResourceAccess": [],
            "web": {
                "redirectUris": [
                    "https://127.0.0.1:444/applications/default.aspx"
                ],
                "homePageUrl": "http://www.contoso.com/landingPage",
                "logoutUrl": null,
                "implicitGrantSettings": {
                    "enableIdTokenIssuance": true,
                    "enableAccessTokenIssuance": false
                }
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
  "suppressions": [
  ]
}
-->
