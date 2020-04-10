---
title: servicePrincipal： updatePasswordSingleSignOnCredentials
description: 使用用户或组的密码更新单一登录凭据。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ab8a6d256c3f90dbaaa7197f87dec4fd230c73d0
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218589"
---
# <a name="serviceprincipal-updatepasswordsinglesignoncredentials"></a><span data-ttu-id="b3036-103">servicePrincipal： updatePasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="b3036-103">servicePrincipal: updatePasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="b3036-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3036-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3036-105">使用用户或组的密码更新单一登录凭据。</span><span class="sxs-lookup"><span data-stu-id="b3036-105">Update single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3036-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b3036-106">Permissions</span></span>

<span data-ttu-id="b3036-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3036-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3036-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3036-109">Permission type</span></span>                        | <span data-ttu-id="b3036-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3036-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b3036-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3036-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3036-112">应用程序的 ReadWrite （也需要 Directory.accessasuser.all），all，All，All，All</span><span class="sxs-lookup"><span data-stu-id="b3036-112">Application.ReadWrite.All (also needs Directory.Read.All), Directory.AccessAsUser.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="b3036-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3036-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3036-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3036-114">Not supported.</span></span> |
| <span data-ttu-id="b3036-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3036-115">Application</span></span>                            | <span data-ttu-id="b3036-116">应用程序的 ReadWrite （也需要全部为目录）、</span><span class="sxs-lookup"><span data-stu-id="b3036-116">Application.ReadWrite.All (also needs Directory.Read.All), Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="b3036-117">用户可以为自己创建凭据。</span><span class="sxs-lookup"><span data-stu-id="b3036-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="b3036-118">具有以下角色的服务主体所有者和管理员可以为任何用户或组创建凭据： GlobalAdministrator、ApplicationAdministrator、CloudApplicationAdministrator。</span><span class="sxs-lookup"><span data-stu-id="b3036-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="b3036-119">若要了解详细信息，请参阅[目录角色](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="b3036-119">To learn more, see [Directory roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="b3036-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3036-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/updatePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="b3036-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3036-121">Request headers</span></span>

| <span data-ttu-id="b3036-122">名称</span><span class="sxs-lookup"><span data-stu-id="b3036-122">Name</span></span>          | <span data-ttu-id="b3036-123">说明</span><span class="sxs-lookup"><span data-stu-id="b3036-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b3036-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3036-124">Authorization</span></span> | <span data-ttu-id="b3036-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b3036-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3036-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3036-127">Content-Type</span></span>  | <span data-ttu-id="b3036-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b3036-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b3036-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3036-130">Request body</span></span>

<span data-ttu-id="b3036-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b3036-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b3036-132">参数</span><span class="sxs-lookup"><span data-stu-id="b3036-132">Parameter</span></span>    | <span data-ttu-id="b3036-133">类型</span><span class="sxs-lookup"><span data-stu-id="b3036-133">Type</span></span>        | <span data-ttu-id="b3036-134">说明</span><span class="sxs-lookup"><span data-stu-id="b3036-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b3036-135">id</span><span class="sxs-lookup"><span data-stu-id="b3036-135">id</span></span>|<span data-ttu-id="b3036-136">字符串</span><span class="sxs-lookup"><span data-stu-id="b3036-136">String</span></span>|<span data-ttu-id="b3036-137">此凭据集所属的用户或组的 ID。</span><span class="sxs-lookup"><span data-stu-id="b3036-137">The ID of the user or group this credential set belongs to.</span></span>|
|<span data-ttu-id="b3036-138">凭据</span><span class="sxs-lookup"><span data-stu-id="b3036-138">credentials</span></span>|<span data-ttu-id="b3036-139">[凭据](../resources/credential.md)集合</span><span class="sxs-lookup"><span data-stu-id="b3036-139">[credential](../resources/credential.md) collection</span></span>|<span data-ttu-id="b3036-140">定义完整的登录流的 credential 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="b3036-140">A list of credential objects that define the complete sign in flow.</span></span>|

## <a name="response"></a><span data-ttu-id="b3036-141">响应</span><span class="sxs-lookup"><span data-stu-id="b3036-141">Response</span></span>

<span data-ttu-id="b3036-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b3036-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3036-144">示例</span><span class="sxs-lookup"><span data-stu-id="b3036-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3036-145">请求</span><span class="sxs-lookup"><span data-stu-id="b3036-145">Request</span></span>

<span data-ttu-id="b3036-146">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="b3036-146">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b3036-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3036-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_updatepasswordsinglesignoncredentials"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/updatePasswordSingleSignOnCredentials
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
      "value": "pa$$w0rd",
      "type": "password"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="b3036-148">C#</span><span class="sxs-lookup"><span data-stu-id="b3036-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-updatepasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3036-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3036-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-updatepasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3036-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3036-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-updatepasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b3036-151">响应</span><span class="sxs-lookup"><span data-stu-id="b3036-151">Response</span></span>

<span data-ttu-id="b3036-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b3036-152">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: updatePasswordSingleSignOnCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
