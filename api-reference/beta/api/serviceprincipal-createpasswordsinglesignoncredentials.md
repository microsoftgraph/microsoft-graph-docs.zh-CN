---
title: servicePrincipal： createPasswordSingleSignOnCredentials
description: 使用用户或组的密码创建单一登录凭据。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 844aa04d39ada59fa06c92749331f0d71714bd9b
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313238"
---
# <a name="serviceprincipal-createpasswordsinglesignoncredentials"></a><span data-ttu-id="fa7f3-103">servicePrincipal： createPasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="fa7f3-103">servicePrincipal: createPasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="fa7f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa7f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa7f3-105">使用用户或组的密码创建单一登录凭据。</span><span class="sxs-lookup"><span data-stu-id="fa7f3-105">Create single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa7f3-106">权限</span><span class="sxs-lookup"><span data-stu-id="fa7f3-106">Permissions</span></span>

<span data-ttu-id="fa7f3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa7f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa7f3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa7f3-109">Permission type</span></span>                        | <span data-ttu-id="fa7f3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa7f3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fa7f3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa7f3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa7f3-112">"ReadWrite"、"全部" 和 "Directory.accessasuser.all"、"全部"、"全部"、"所有"</span><span class="sxs-lookup"><span data-stu-id="fa7f3-112">Application.ReadWrite.All and Directory.Read.All,  Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="fa7f3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa7f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa7f3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa7f3-114">Not supported.</span></span> |
| <span data-ttu-id="fa7f3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa7f3-115">Application</span></span>                            | <span data-ttu-id="fa7f3-116">所有的读写全部和目录。全部</span><span class="sxs-lookup"><span data-stu-id="fa7f3-116">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="fa7f3-117">用户可以为自己创建凭据。</span><span class="sxs-lookup"><span data-stu-id="fa7f3-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="fa7f3-118">具有以下角色的服务主体所有者和管理员可以为任何用户或组创建凭据： GlobalAdministrator、ApplicationAdministrator、CloudApplicationAdministrator。</span><span class="sxs-lookup"><span data-stu-id="fa7f3-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="fa7f3-119">若要了解详细信息，请参阅 [目录角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="fa7f3-119">To learn more, see [Directory roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="fa7f3-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa7f3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/createPasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="fa7f3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa7f3-121">Request headers</span></span>

| <span data-ttu-id="fa7f3-122">名称</span><span class="sxs-lookup"><span data-stu-id="fa7f3-122">Name</span></span>          | <span data-ttu-id="fa7f3-123">说明</span><span class="sxs-lookup"><span data-stu-id="fa7f3-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fa7f3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa7f3-124">Authorization</span></span> | <span data-ttu-id="fa7f3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa7f3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa7f3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa7f3-127">Content-Type</span></span>  | <span data-ttu-id="fa7f3-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fa7f3-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa7f3-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa7f3-130">Request body</span></span>

<span data-ttu-id="fa7f3-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fa7f3-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fa7f3-132">参数</span><span class="sxs-lookup"><span data-stu-id="fa7f3-132">Parameter</span></span>    | <span data-ttu-id="fa7f3-133">类型</span><span class="sxs-lookup"><span data-stu-id="fa7f3-133">Type</span></span>        | <span data-ttu-id="fa7f3-134">说明</span><span class="sxs-lookup"><span data-stu-id="fa7f3-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fa7f3-135">id</span><span class="sxs-lookup"><span data-stu-id="fa7f3-135">id</span></span>|<span data-ttu-id="fa7f3-136">字符串</span><span class="sxs-lookup"><span data-stu-id="fa7f3-136">String</span></span>|<span data-ttu-id="fa7f3-137">此凭据集所属的用户或组的 ID。</span><span class="sxs-lookup"><span data-stu-id="fa7f3-137">The ID of the user or group this credential set belongs to.</span></span>|
|<span data-ttu-id="fa7f3-138">凭据</span><span class="sxs-lookup"><span data-stu-id="fa7f3-138">credentials</span></span>|<span data-ttu-id="fa7f3-139">[凭据](../resources/credential.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fa7f3-139">[credential](../resources/credential.md) collection</span></span>|<span data-ttu-id="fa7f3-140">定义完整的登录流的 credential 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="fa7f3-140">A list of credential objects that define the complete sign in flow.</span></span>|

## <a name="response"></a><span data-ttu-id="fa7f3-141">响应</span><span class="sxs-lookup"><span data-stu-id="fa7f3-141">Response</span></span>

<span data-ttu-id="fa7f3-142">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和新的 [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fa7f3-142">If successful, this method returns a `200 OK` response code and a new [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa7f3-143">示例</span><span class="sxs-lookup"><span data-stu-id="fa7f3-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa7f3-144">请求</span><span class="sxs-lookup"><span data-stu-id="fa7f3-144">Request</span></span>

<span data-ttu-id="fa7f3-145">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="fa7f3-145">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fa7f3-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa7f3-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_createpasswordsinglesignoncredentials"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/createPasswordSingleSignOnCredentials
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
# <a name="c"></a>[<span data-ttu-id="fa7f3-147">C#</span><span class="sxs-lookup"><span data-stu-id="fa7f3-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-createpasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa7f3-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa7f3-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-createpasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa7f3-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa7f3-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-createpasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fa7f3-150">响应</span><span class="sxs-lookup"><span data-stu-id="fa7f3-150">Response</span></span>

<span data-ttu-id="fa7f3-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fa7f3-151">The following is an example of the response.</span></span>

> <span data-ttu-id="fa7f3-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fa7f3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "servicePrincipal: createPasswordSingleSignOnCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->