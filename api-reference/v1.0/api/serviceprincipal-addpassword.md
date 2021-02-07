---
title: servicePrincipal：addPassword
description: 向 servicePrincipal 添加强密码。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 518d7b696d214ead133bcf869381099034094359
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132011"
---
# <a name="serviceprincipal-addpassword"></a><span data-ttu-id="2c2ae-103">servicePrincipal：addPassword</span><span class="sxs-lookup"><span data-stu-id="2c2ae-103">servicePrincipal: addPassword</span></span>

<span data-ttu-id="2c2ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c2ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2c2ae-105">向 [servicePrincipal](../resources/serviceprincipal.md) 对象添加强密码。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-105">Add a strong password to a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c2ae-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2c2ae-106">Permissions</span></span>

<span data-ttu-id="2c2ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2c2ae-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c2ae-109">Permission type</span></span>                        | <span data-ttu-id="2c2ae-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c2ae-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2c2ae-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c2ae-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c2ae-112">Application.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c2ae-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="2c2ae-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c2ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c2ae-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-114">Not supported.</span></span> |
| <span data-ttu-id="2c2ae-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c2ae-115">Application</span></span>                            | <span data-ttu-id="2c2ae-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c2ae-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c2ae-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c2ae-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="2c2ae-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c2ae-118">Request headers</span></span>

| <span data-ttu-id="2c2ae-119">名称</span><span class="sxs-lookup"><span data-stu-id="2c2ae-119">Name</span></span>           | <span data-ttu-id="2c2ae-120">说明</span><span class="sxs-lookup"><span data-stu-id="2c2ae-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="2c2ae-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c2ae-121">Authorization</span></span>  | <span data-ttu-id="2c2ae-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2c2ae-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2c2ae-124">Content-Type</span></span>   | <span data-ttu-id="2c2ae-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2c2ae-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c2ae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c2ae-127">Request body</span></span>

<span data-ttu-id="2c2ae-128">在请求正文中，提供 `passwordCredential` 具有以下属性的可选对象。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-128">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="2c2ae-129">属性</span><span class="sxs-lookup"><span data-stu-id="2c2ae-129">Property</span></span>     | <span data-ttu-id="2c2ae-130">类型</span><span class="sxs-lookup"><span data-stu-id="2c2ae-130">Type</span></span>   |<span data-ttu-id="2c2ae-131">说明</span><span class="sxs-lookup"><span data-stu-id="2c2ae-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2c2ae-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2c2ae-132">displayName</span></span> | <span data-ttu-id="2c2ae-133">String</span><span class="sxs-lookup"><span data-stu-id="2c2ae-133">String</span></span> | <span data-ttu-id="2c2ae-134">密码的友好名称。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-134">Friendly name for the password.</span></span> <span data-ttu-id="2c2ae-135">可选。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-135">Optional.</span></span> |
| <span data-ttu-id="2c2ae-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2c2ae-136">endDateTime</span></span> | <span data-ttu-id="2c2ae-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c2ae-137">DateTimeOffset</span></span> | <span data-ttu-id="2c2ae-138">密码过期的日期和时间使用 ISO 8601 格式表示，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-138">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2c2ae-139">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="2c2ae-140">可选。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-140">Optional.</span></span> <span data-ttu-id="2c2ae-141">默认值为"startDateTime + 2 年"。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-141">The default value is "startDateTime + 2 years".</span></span> |
| <span data-ttu-id="2c2ae-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2c2ae-142">startDateTime</span></span> | <span data-ttu-id="2c2ae-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c2ae-143">DateTimeOffset</span></span> | <span data-ttu-id="2c2ae-144">密码生效的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="2c2ae-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2c2ae-146">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="2c2ae-147">可选。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-147">Optional.</span></span> <span data-ttu-id="2c2ae-148">默认值为"now"。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-148">The default value is "now".</span></span>|

## <a name="response"></a><span data-ttu-id="2c2ae-149">响应</span><span class="sxs-lookup"><span data-stu-id="2c2ae-149">Response</span></span>

<span data-ttu-id="2c2ae-150">如果成功，此方法在响应正文中返回响应代码和新 `200 OK` [passwordCredential](../resources/passwordcredential.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-150">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="2c2ae-151">响应 **对象中的 secretText** 属性包含 Azure Active Directory 生成的强密码，长度为 16-64 个字符。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-151">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="2c2ae-152">以后无法检索此密码。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-152">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="2c2ae-153">示例</span><span class="sxs-lookup"><span data-stu-id="2c2ae-153">Examples</span></span>

<span data-ttu-id="2c2ae-154">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-154">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2c2ae-155">请求</span><span class="sxs-lookup"><span data-stu-id="2c2ae-155">Request</span></span>

<span data-ttu-id="2c2ae-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c2ae-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c2ae-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_addpassword"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/addPassword
Content-type: application/json

{
  "passwordCredential": {
    "displayName": "Password friendly name"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="2c2ae-158">C#</span><span class="sxs-lookup"><span data-stu-id="2c2ae-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-addpassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c2ae-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c2ae-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c2ae-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c2ae-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-addpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c2ae-161">Java</span><span class="sxs-lookup"><span data-stu-id="2c2ae-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-addpassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2c2ae-162">响应</span><span class="sxs-lookup"><span data-stu-id="2c2ae-162">Response</span></span>

<span data-ttu-id="2c2ae-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2c2ae-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordCredential"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "customKeyIdentifier": null,
    "endDateTime": "2021-09-09T19:50:29.3086381Z",
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "startDateTime": "2019-09-09T19:50:29.3086381Z",
    "secretText": "[6gyXA5S20@MN+WRXAJ]I-TO7g1:h2P8",
    "hint": "[6g",
    "displayName": "Password friendly name"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: addPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

