---
title: application： addPassword
description: 向应用程序添加强密码。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 90fc14f3d56c9ca815d7abd721cdeef48dfdb23b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721976"
---
# <a name="application-addpassword"></a><span data-ttu-id="07850-103">application： addPassword</span><span class="sxs-lookup"><span data-stu-id="07850-103">application: addPassword</span></span>

<span data-ttu-id="07850-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07850-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="07850-105">将强密码添加到 [应用程序](../resources/application.md)。</span><span class="sxs-lookup"><span data-stu-id="07850-105">Adds a strong password to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="07850-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="07850-106">Permissions</span></span>

<span data-ttu-id="07850-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07850-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07850-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="07850-109">Permission type</span></span>                        | <span data-ttu-id="07850-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07850-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="07850-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07850-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="07850-112">Application.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07850-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="07850-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07850-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07850-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07850-114">Application.ReadWrite.All</span></span> |
| <span data-ttu-id="07850-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="07850-115">Application</span></span>                            | <span data-ttu-id="07850-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="07850-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07850-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07850-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="07850-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="07850-118">Request headers</span></span>

| <span data-ttu-id="07850-119">名称</span><span class="sxs-lookup"><span data-stu-id="07850-119">Name</span></span>           | <span data-ttu-id="07850-120">说明</span><span class="sxs-lookup"><span data-stu-id="07850-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="07850-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="07850-121">Authorization</span></span>  | <span data-ttu-id="07850-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="07850-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="07850-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="07850-124">Content-Type</span></span>   | <span data-ttu-id="07850-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="07850-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="07850-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="07850-127">Request body</span></span>

<span data-ttu-id="07850-128">在请求正文中，提供具有以下 `passwordCredential` 属性的可选对象。</span><span class="sxs-lookup"><span data-stu-id="07850-128">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="07850-129">属性</span><span class="sxs-lookup"><span data-stu-id="07850-129">Property</span></span>     | <span data-ttu-id="07850-130">类型</span><span class="sxs-lookup"><span data-stu-id="07850-130">Type</span></span>   |<span data-ttu-id="07850-131">说明</span><span class="sxs-lookup"><span data-stu-id="07850-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="07850-132">displayName</span><span class="sxs-lookup"><span data-stu-id="07850-132">displayName</span></span> | <span data-ttu-id="07850-133">字符串</span><span class="sxs-lookup"><span data-stu-id="07850-133">String</span></span> | <span data-ttu-id="07850-134">密码的友好名称。</span><span class="sxs-lookup"><span data-stu-id="07850-134">Friendly name for the password.</span></span> <span data-ttu-id="07850-135">可选。</span><span class="sxs-lookup"><span data-stu-id="07850-135">Optional.</span></span> |
| <span data-ttu-id="07850-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="07850-136">endDateTime</span></span> | <span data-ttu-id="07850-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07850-137">DateTimeOffset</span></span> | <span data-ttu-id="07850-138">密码过期的日期和时间使用 ISO 8601 格式表示，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="07850-138">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07850-139">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="07850-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="07850-140">可选。</span><span class="sxs-lookup"><span data-stu-id="07850-140">Optional.</span></span> <span data-ttu-id="07850-141">默认值为"startDateTime + 2 年"。</span><span class="sxs-lookup"><span data-stu-id="07850-141">The default value is "startDateTime + 2 years".</span></span> |
| <span data-ttu-id="07850-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="07850-142">startDateTime</span></span> | <span data-ttu-id="07850-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07850-143">DateTimeOffset</span></span> | <span data-ttu-id="07850-144">密码生效的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="07850-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="07850-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="07850-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07850-146">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="07850-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="07850-147">可选。</span><span class="sxs-lookup"><span data-stu-id="07850-147">Optional.</span></span>  <span data-ttu-id="07850-148">默认值为"now"。</span><span class="sxs-lookup"><span data-stu-id="07850-148">The default value is "now".</span></span> |

## <a name="response"></a><span data-ttu-id="07850-149">响应</span><span class="sxs-lookup"><span data-stu-id="07850-149">Response</span></span>

<span data-ttu-id="07850-150">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和新 [passwordCredential](../resources/passwordcredential.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07850-150">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="07850-151">**响应对象中的 secretText** 属性包含 Azure Active Directory 生成的强密码，长度为 16-64 个字符。</span><span class="sxs-lookup"><span data-stu-id="07850-151">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="07850-152">将来无法检索此密码。</span><span class="sxs-lookup"><span data-stu-id="07850-152">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="07850-153">示例</span><span class="sxs-lookup"><span data-stu-id="07850-153">Examples</span></span>

<span data-ttu-id="07850-154">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="07850-154">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="07850-155">请求</span><span class="sxs-lookup"><span data-stu-id="07850-155">Request</span></span>

<span data-ttu-id="07850-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="07850-156">The following is an example of the request.</span></span> <span data-ttu-id="07850-157">请求 **中** 指定的 id 是应用程序的 **id** 属性的值，而不是 **appId 属性的值** 。</span><span class="sxs-lookup"><span data-stu-id="07850-157">The **id** that is specified in the request is the value of the **id** property of the application, not the value of the **appId** property.</span></span> 

# <a name="http"></a>[<span data-ttu-id="07850-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="07850-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addpassword"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/addPassword
Content-type: application/json

{
  "passwordCredential": {
    "displayName": "Password friendly name"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="07850-159">C#</span><span class="sxs-lookup"><span data-stu-id="07850-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addpassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07850-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07850-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07850-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07850-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="07850-162">Java</span><span class="sxs-lookup"><span data-stu-id="07850-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addpassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="07850-163">响应</span><span class="sxs-lookup"><span data-stu-id="07850-163">Response</span></span>

<span data-ttu-id="07850-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="07850-164">The following is an example of the response.</span></span>

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
  "description": "application: addPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

