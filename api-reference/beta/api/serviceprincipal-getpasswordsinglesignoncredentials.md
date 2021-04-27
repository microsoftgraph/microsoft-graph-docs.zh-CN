---
title: servicePrincipal：getPasswordSingleSignOnCredentials
description: 使用用户或组的密码获取单一登录凭据列表。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 39286664f3191dfc12a0bf5866e19f3ff73de1d0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051905"
---
# <a name="serviceprincipal-getpasswordsinglesignoncredentials"></a><span data-ttu-id="02332-103">servicePrincipal：getPasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="02332-103">servicePrincipal: getPasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="02332-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02332-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02332-105">使用用户或组的密码获取单一登录凭据列表。</span><span class="sxs-lookup"><span data-stu-id="02332-105">Get a list of single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="02332-106">权限</span><span class="sxs-lookup"><span data-stu-id="02332-106">Permissions</span></span>

<span data-ttu-id="02332-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02332-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="02332-109">Permission type</span></span>                        | <span data-ttu-id="02332-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="02332-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="02332-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02332-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="02332-112">Application.ReadWrite.All 和 Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="02332-112">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="02332-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02332-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02332-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="02332-114">Not supported.</span></span> |
| <span data-ttu-id="02332-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="02332-115">Application</span></span>                            | <span data-ttu-id="02332-116">Application.ReadWrite.OwnedBy 和 Directory.Read.All、Application.ReadWrite.All 和 Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02332-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="02332-117">用户可以为自己创建凭据。</span><span class="sxs-lookup"><span data-stu-id="02332-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="02332-118">具有以下角色的服务主体所有者和管理员可以为任何用户或组创建凭据：GlobalAdministrator、ApplicationAdministrator、CloudApplicationAdministrator。</span><span class="sxs-lookup"><span data-stu-id="02332-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="02332-119">若要了解更多信息，请参阅 [目录角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="02332-119">To learn more, see [Directory roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="02332-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02332-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/getPasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="02332-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="02332-121">Request headers</span></span>

| <span data-ttu-id="02332-122">名称</span><span class="sxs-lookup"><span data-stu-id="02332-122">Name</span></span>          | <span data-ttu-id="02332-123">说明</span><span class="sxs-lookup"><span data-stu-id="02332-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="02332-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="02332-124">Authorization</span></span> | <span data-ttu-id="02332-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="02332-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="02332-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02332-127">Content-Type</span></span>  | <span data-ttu-id="02332-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="02332-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02332-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="02332-130">Request body</span></span>

<span data-ttu-id="02332-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="02332-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="02332-132">参数</span><span class="sxs-lookup"><span data-stu-id="02332-132">Parameter</span></span>    | <span data-ttu-id="02332-133">类型</span><span class="sxs-lookup"><span data-stu-id="02332-133">Type</span></span>        | <span data-ttu-id="02332-134">说明</span><span class="sxs-lookup"><span data-stu-id="02332-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="02332-135">id</span><span class="sxs-lookup"><span data-stu-id="02332-135">id</span></span>|<span data-ttu-id="02332-136">String</span><span class="sxs-lookup"><span data-stu-id="02332-136">String</span></span>|<span data-ttu-id="02332-137">此凭据集所属的用户或组的 ID。</span><span class="sxs-lookup"><span data-stu-id="02332-137">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="response"></a><span data-ttu-id="02332-138">响应</span><span class="sxs-lookup"><span data-stu-id="02332-138">Response</span></span>

<span data-ttu-id="02332-139">如果成功，此方法在响应正文中返回 响应代码和新 `200 OK` [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="02332-139">If successful, this method returns a `200 OK` response code and a new [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02332-140">示例</span><span class="sxs-lookup"><span data-stu-id="02332-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02332-141">请求</span><span class="sxs-lookup"><span data-stu-id="02332-141">Request</span></span>

<span data-ttu-id="02332-142">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="02332-142">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="02332-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="02332-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getpasswordsinglesignoncredentials"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getPasswordSingleSignOnCredentials
Content-type: application/json

{
  "id": "5793aa3b-cca9-4794-679a240f8b58"
}
```
# <a name="c"></a>[<span data-ttu-id="02332-144">C#</span><span class="sxs-lookup"><span data-stu-id="02332-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getpasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02332-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02332-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getpasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02332-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02332-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getpasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02332-147">Java</span><span class="sxs-lookup"><span data-stu-id="02332-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-getpasswordsinglesignoncredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02332-148">响应</span><span class="sxs-lookup"><span data-stu-id="02332-148">Response</span></span>

<span data-ttu-id="02332-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="02332-149">The following is an example of the response.</span></span>

> <span data-ttu-id="02332-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="02332-150">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordSingleSignOnCredentialSet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5793aa3b-cca9-4794-679a240f8b58",
  "credentials": [
    {
      "fieldId": "param_username",
      "value": "myusername",
      "type": "username"
    },
    {
      "fieldId": "param_password",
      "value": null,
      "type": "password"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: getPasswordSingleSignOnCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
