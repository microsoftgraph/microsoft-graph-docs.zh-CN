---
title: servicePrincipal：deletePasswordSingleSignOnCredentials
description: 使用用户或组的密码删除单一登录凭据。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 1885fab70ab539290045242c1e43d69f214e61fb
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787210"
---
# <a name="serviceprincipal-deletepasswordsinglesignoncredentials"></a><span data-ttu-id="3a1e0-103">servicePrincipal：deletePasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="3a1e0-103">servicePrincipal: deletePasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="3a1e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a1e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a1e0-105">使用用户或组的密码删除单一登录凭据。</span><span class="sxs-lookup"><span data-stu-id="3a1e0-105">Delete single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a1e0-106">权限</span><span class="sxs-lookup"><span data-stu-id="3a1e0-106">Permissions</span></span>

<span data-ttu-id="3a1e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3a1e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a1e0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a1e0-109">Permission type</span></span>                        | <span data-ttu-id="3a1e0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a1e0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3a1e0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a1e0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a1e0-112">Application.ReadWrite.All 和 Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a1e0-112">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="3a1e0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a1e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a1e0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a1e0-114">Not supported.</span></span> |
| <span data-ttu-id="3a1e0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a1e0-115">Application</span></span>                            | <span data-ttu-id="3a1e0-116">Application.ReadWrite.All 和 Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a1e0-116">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="3a1e0-117">用户可以为自己创建凭据。</span><span class="sxs-lookup"><span data-stu-id="3a1e0-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="3a1e0-118">具有以下角色的服务主体所有者和管理员可以为任何用户或组创建凭据：GlobalAdministrator、ApplicationAdministrator、CloudApplicationAdministrator。</span><span class="sxs-lookup"><span data-stu-id="3a1e0-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="3a1e0-119">若要了解更多信息，请参阅 [目录角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="3a1e0-119">To learn more, see [Directory roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="3a1e0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a1e0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/deletePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="3a1e0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a1e0-121">Request headers</span></span>

| <span data-ttu-id="3a1e0-122">名称</span><span class="sxs-lookup"><span data-stu-id="3a1e0-122">Name</span></span>          | <span data-ttu-id="3a1e0-123">说明</span><span class="sxs-lookup"><span data-stu-id="3a1e0-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3a1e0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a1e0-124">Authorization</span></span> | <span data-ttu-id="3a1e0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3a1e0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a1e0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a1e0-127">Content-Type</span></span>  | <span data-ttu-id="3a1e0-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3a1e0-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a1e0-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a1e0-130">Request body</span></span>

<span data-ttu-id="3a1e0-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3a1e0-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3a1e0-132">参数</span><span class="sxs-lookup"><span data-stu-id="3a1e0-132">Parameter</span></span>    | <span data-ttu-id="3a1e0-133">类型</span><span class="sxs-lookup"><span data-stu-id="3a1e0-133">Type</span></span>        | <span data-ttu-id="3a1e0-134">说明</span><span class="sxs-lookup"><span data-stu-id="3a1e0-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3a1e0-135">id</span><span class="sxs-lookup"><span data-stu-id="3a1e0-135">id</span></span>|<span data-ttu-id="3a1e0-136">String</span><span class="sxs-lookup"><span data-stu-id="3a1e0-136">String</span></span>|<span data-ttu-id="3a1e0-137">此凭据集所属的用户或组的 ID。</span><span class="sxs-lookup"><span data-stu-id="3a1e0-137">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="response"></a><span data-ttu-id="3a1e0-138">响应</span><span class="sxs-lookup"><span data-stu-id="3a1e0-138">Response</span></span>

<span data-ttu-id="3a1e0-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3a1e0-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a1e0-141">示例</span><span class="sxs-lookup"><span data-stu-id="3a1e0-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a1e0-142">请求</span><span class="sxs-lookup"><span data-stu-id="3a1e0-142">Request</span></span>

<span data-ttu-id="3a1e0-143">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="3a1e0-143">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a1e0-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a1e0-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_deletepasswordsinglesignoncredentials"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/deletePasswordSingleSignOnCredentials
Content-type: application/json

{
  "id": "5793aa3b-cca9-4794-679a240f8b58"
}
```
# <a name="c"></a>[<span data-ttu-id="3a1e0-145">C#</span><span class="sxs-lookup"><span data-stu-id="3a1e0-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-deletepasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a1e0-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a1e0-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-deletepasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a1e0-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a1e0-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-deletepasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a1e0-148">Java</span><span class="sxs-lookup"><span data-stu-id="3a1e0-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-deletepasswordsinglesignoncredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3a1e0-149">响应</span><span class="sxs-lookup"><span data-stu-id="3a1e0-149">Response</span></span>

<span data-ttu-id="3a1e0-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3a1e0-150">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: deletePasswordSingleSignOnCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
