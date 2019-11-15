---
title: servicePrincipal： updatePasswordSingleSignOnCredentials
description: 使用用户或组的密码更新单一登录凭据。
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef480c7f40fe74a46ded87c588f4a7c4eb628d26
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658812"
---
# <a name="serviceprincipal-updatepasswordsinglesignoncredentials"></a><span data-ttu-id="78137-103">servicePrincipal： updatePasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="78137-103">servicePrincipal: updatePasswordSingleSignOnCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78137-104">使用用户或组的密码更新单一登录凭据。</span><span class="sxs-lookup"><span data-stu-id="78137-104">Update single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="78137-105">权限</span><span class="sxs-lookup"><span data-stu-id="78137-105">Permissions</span></span>

<span data-ttu-id="78137-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="78137-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="78137-108">Permission type</span></span>                        | <span data-ttu-id="78137-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78137-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="78137-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78137-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="78137-111">应用程序的 ReadWrite （也需要 Directory.accessasuser.all），all，All，All，All</span><span class="sxs-lookup"><span data-stu-id="78137-111">Application.ReadWrite.All (also needs Directory.Read.All), Directory.AccessAsUser.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="78137-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78137-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78137-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="78137-113">Not supported.</span></span> |
| <span data-ttu-id="78137-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="78137-114">Application</span></span>                            | <span data-ttu-id="78137-115">应用程序的 ReadWrite （也需要全部为目录）、</span><span class="sxs-lookup"><span data-stu-id="78137-115">Application.ReadWrite.All (also needs Directory.Read.All), Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="78137-116">用户可以为自己创建凭据。</span><span class="sxs-lookup"><span data-stu-id="78137-116">Users can create credentials for themselves.</span></span> <span data-ttu-id="78137-117">具有以下角色的服务主体所有者和管理员可以为任何用户或组创建凭据： GlobalAdministrator、ApplicationAdministrator、CloudApplicationAdministrator。</span><span class="sxs-lookup"><span data-stu-id="78137-117">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="78137-118">若要了解详细信息，请参阅[目录角色](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="78137-118">To learn more, see [Directory roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="78137-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78137-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/updatePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="78137-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="78137-120">Request headers</span></span>

| <span data-ttu-id="78137-121">名称</span><span class="sxs-lookup"><span data-stu-id="78137-121">Name</span></span>          | <span data-ttu-id="78137-122">说明</span><span class="sxs-lookup"><span data-stu-id="78137-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="78137-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78137-123">Authorization</span></span> | <span data-ttu-id="78137-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78137-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="78137-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="78137-126">Content-Type</span></span>  | <span data-ttu-id="78137-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="78137-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="78137-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="78137-129">Request body</span></span>

<span data-ttu-id="78137-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="78137-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="78137-131">参数</span><span class="sxs-lookup"><span data-stu-id="78137-131">Parameter</span></span>    | <span data-ttu-id="78137-132">类型</span><span class="sxs-lookup"><span data-stu-id="78137-132">Type</span></span>        | <span data-ttu-id="78137-133">说明</span><span class="sxs-lookup"><span data-stu-id="78137-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="78137-134">id</span><span class="sxs-lookup"><span data-stu-id="78137-134">id</span></span>|<span data-ttu-id="78137-135">字符串</span><span class="sxs-lookup"><span data-stu-id="78137-135">String</span></span>|<span data-ttu-id="78137-136">此凭据集所属的用户或组的 ID。</span><span class="sxs-lookup"><span data-stu-id="78137-136">The ID of the user or group this credential set belongs to.</span></span>|
|<span data-ttu-id="78137-137">凭据</span><span class="sxs-lookup"><span data-stu-id="78137-137">credentials</span></span>|<span data-ttu-id="78137-138">[凭据](../resources/credential.md)集合</span><span class="sxs-lookup"><span data-stu-id="78137-138">[credential](../resources/credential.md) collection</span></span>|<span data-ttu-id="78137-139">定义完整的登录流的 credential 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="78137-139">A list of credential objects that define the complete sign in flow.</span></span>|

## <a name="response"></a><span data-ttu-id="78137-140">响应</span><span class="sxs-lookup"><span data-stu-id="78137-140">Response</span></span>

<span data-ttu-id="78137-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="78137-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="78137-143">示例</span><span class="sxs-lookup"><span data-stu-id="78137-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="78137-144">请求</span><span class="sxs-lookup"><span data-stu-id="78137-144">Request</span></span>

<span data-ttu-id="78137-145">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="78137-145">The following is an example of a request.</span></span>
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

### <a name="response"></a><span data-ttu-id="78137-146">响应</span><span class="sxs-lookup"><span data-stu-id="78137-146">Response</span></span>

<span data-ttu-id="78137-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="78137-147">The following is an example of the response.</span></span>
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
