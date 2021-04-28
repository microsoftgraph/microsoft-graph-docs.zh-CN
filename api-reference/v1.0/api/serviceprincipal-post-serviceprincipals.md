---
title: 创建 serviceprincipal
description: 创建新的 serviceprincipal 对象。
author: sureshja
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
ms.openlocfilehash: 83410afe63fadfc0d9e04e10cf8f8d66bb37c530
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053809"
---
# <a name="create-serviceprincipal"></a><span data-ttu-id="b8fc6-103">创建 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="b8fc6-103">Create servicePrincipal</span></span>

<span data-ttu-id="b8fc6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8fc6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8fc6-105">创建一个新的 [servicePrincipal](../resources/serviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b8fc6-105">Create a new [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b8fc6-106">不支持在创建 servicePrincipals 时添加 [**passwordCredential**](../resources/passwordcredential.md)。</span><span class="sxs-lookup"><span data-stu-id="b8fc6-106">Adding [**passwordCredential**](../resources/passwordcredential.md) when creating servicePrincipals is not supported.</span></span> <span data-ttu-id="b8fc6-107">使用 [addPassword](serviceprincipal-addpassword.md) 方法为 servicePrincipal 添加密码。</span><span class="sxs-lookup"><span data-stu-id="b8fc6-107">Use the [addPassword](serviceprincipal-addpassword.md) method to add passwords for a servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8fc6-108">权限</span><span class="sxs-lookup"><span data-stu-id="b8fc6-108">Permissions</span></span>
<span data-ttu-id="b8fc6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8fc6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b8fc6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8fc6-111">Permission type</span></span>      | <span data-ttu-id="b8fc6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8fc6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8fc6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8fc6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b8fc6-114">Application.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b8fc6-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b8fc6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8fc6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8fc6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8fc6-116">Not supported.</span></span>    |
|<span data-ttu-id="b8fc6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8fc6-117">Application</span></span> | <span data-ttu-id="b8fc6-118">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8fc6-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8fc6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8fc6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals
```

## <a name="request-headers"></a><span data-ttu-id="b8fc6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8fc6-120">Request headers</span></span>
| <span data-ttu-id="b8fc6-121">名称</span><span class="sxs-lookup"><span data-stu-id="b8fc6-121">Name</span></span>       | <span data-ttu-id="b8fc6-122">说明</span><span class="sxs-lookup"><span data-stu-id="b8fc6-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="b8fc6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8fc6-123">Authorization</span></span> | <span data-ttu-id="b8fc6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b8fc6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b8fc6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8fc6-126">Content-Type</span></span> | <span data-ttu-id="b8fc6-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b8fc6-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8fc6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8fc6-129">Request body</span></span>
<span data-ttu-id="b8fc6-130">在请求正文中，提供 [servicePrincipal](../resources/serviceprincipal.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8fc6-130">In the request body, supply a JSON representation of a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span> <span data-ttu-id="b8fc6-131">请求正文必须包含 **appId**。</span><span class="sxs-lookup"><span data-stu-id="b8fc6-131">The request body must contain  **appId**.</span></span>

## <a name="response"></a><span data-ttu-id="b8fc6-132">响应</span><span class="sxs-lookup"><span data-stu-id="b8fc6-132">Response</span></span>

<span data-ttu-id="b8fc6-133">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [servicePrincipal](../resources/serviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b8fc6-133">If successful, this method returns a `201 Created` response code and a [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b8fc6-134">示例</span><span class="sxs-lookup"><span data-stu-id="b8fc6-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="b8fc6-135">请求</span><span class="sxs-lookup"><span data-stu-id="b8fc6-135">Request</span></span>
<span data-ttu-id="b8fc6-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8fc6-136">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b8fc6-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8fc6-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_serviceprincipal_from_serviceprincipals"
}-->
```http
POST https://graph.microsoft.com/v1.0/servicePrincipals
Content-type: application/json

{
  "appId": "65415bb1-9267-4313-bbf5-ae259732ee12"
}
```
# <a name="c"></a>[<span data-ttu-id="b8fc6-138">C#</span><span class="sxs-lookup"><span data-stu-id="b8fc6-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-serviceprincipal-from-serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8fc6-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8fc6-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-serviceprincipal-from-serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8fc6-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8fc6-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-serviceprincipal-from-serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b8fc6-141">Java</span><span class="sxs-lookup"><span data-stu-id="b8fc6-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-serviceprincipal-from-serviceprincipals-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b8fc6-142">响应</span><span class="sxs-lookup"><span data-stu-id="b8fc6-142">Response</span></span>
<span data-ttu-id="b8fc6-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b8fc6-143">Here is an example of the response.</span></span> 

> <span data-ttu-id="b8fc6-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b8fc6-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals/$entity",
    "id": "59e617e5-e447-4adc-8b88-00af644d7c92",
    "deletedDateTime": null,
    "accountEnabled": true,
    "appDisplayName": "My App",
    "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
    "appOwnerOrganizationId": "1bc1c026-2f7b-48a5-98da-afa2fd8bc7bc",
    "appRoleAssignmentRequired": false,
    "displayName": "foo",
    "homepage": null,
    "logoutUrl": null,
    "publisherName": "Contoso",
    "replyUrls": [],
    "servicePrincipalNames": [
        "f1bd758f-4a1a-4b71-aa20-a248a22a8928"
    ],
    "tags": [],
    "addIns": [],
    "appRoles": [],
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "oauth2PermissionScopes": [],
    "passwordCredentials": []
}
```

