---
title: 应用程序： addPassword
description: 向应用程序添加强密码。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6ea99f8d60b4210c906333a9b01013ff035628c1
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939752"
---
# <a name="application-addpassword"></a><span data-ttu-id="abb93-103">应用程序： addPassword</span><span class="sxs-lookup"><span data-stu-id="abb93-103">application: addPassword</span></span>

<span data-ttu-id="abb93-104">向[应用程序](../resources/application.md)添加强密码。</span><span class="sxs-lookup"><span data-stu-id="abb93-104">Adds a strong password to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="abb93-105">权限</span><span class="sxs-lookup"><span data-stu-id="abb93-105">Permissions</span></span>

<span data-ttu-id="abb93-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="abb93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="abb93-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="abb93-108">Permission type</span></span>                        | <span data-ttu-id="abb93-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="abb93-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="abb93-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="abb93-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="abb93-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="abb93-111">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="abb93-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="abb93-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abb93-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="abb93-113">Not supported.</span></span> |
| <span data-ttu-id="abb93-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="abb93-114">Application</span></span>                            | <span data-ttu-id="abb93-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="abb93-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="abb93-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="abb93-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="abb93-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="abb93-117">Request headers</span></span>

| <span data-ttu-id="abb93-118">名称</span><span class="sxs-lookup"><span data-stu-id="abb93-118">Name</span></span>           | <span data-ttu-id="abb93-119">说明</span><span class="sxs-lookup"><span data-stu-id="abb93-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="abb93-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="abb93-120">Authorization</span></span>  | <span data-ttu-id="abb93-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="abb93-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="abb93-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="abb93-123">Content-type</span></span>   | <span data-ttu-id="abb93-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="abb93-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="abb93-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="abb93-126">Request body</span></span>

<span data-ttu-id="abb93-127">在请求正文中，提供具有以下`passwordCredential`属性的可选对象。</span><span class="sxs-lookup"><span data-stu-id="abb93-127">In the request body, provide an optional `passwordCredential` object with the following properties.</span></span>

| <span data-ttu-id="abb93-128">属性</span><span class="sxs-lookup"><span data-stu-id="abb93-128">Property</span></span>     | <span data-ttu-id="abb93-129">类型</span><span class="sxs-lookup"><span data-stu-id="abb93-129">Type</span></span>   |<span data-ttu-id="abb93-130">描述</span><span class="sxs-lookup"><span data-stu-id="abb93-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="abb93-131">displayName</span><span class="sxs-lookup"><span data-stu-id="abb93-131">displayName</span></span> | <span data-ttu-id="abb93-132">String</span><span class="sxs-lookup"><span data-stu-id="abb93-132">String</span></span> | <span data-ttu-id="abb93-133">密码的友好名称。</span><span class="sxs-lookup"><span data-stu-id="abb93-133">Friendly name for the password.</span></span> <span data-ttu-id="abb93-134">可选。</span><span class="sxs-lookup"><span data-stu-id="abb93-134">Optional.</span></span> |
| <span data-ttu-id="abb93-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="abb93-135">endDateTime</span></span> | <span data-ttu-id="abb93-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abb93-136">DateTimeOffset</span></span> | <span data-ttu-id="abb93-137">密码过期的日期和时间，使用 ISO 8601 格式表示，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="abb93-137">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="abb93-138">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="abb93-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="abb93-139">可选。</span><span class="sxs-lookup"><span data-stu-id="abb93-139">Optional.</span></span> |
| <span data-ttu-id="abb93-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="abb93-140">startDateTime</span></span> | <span data-ttu-id="abb93-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abb93-141">DateTimeOffset</span></span> | <span data-ttu-id="abb93-142">密码生效的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="abb93-142">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="abb93-143">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="abb93-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="abb93-144">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="abb93-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="abb93-145">可选。</span><span class="sxs-lookup"><span data-stu-id="abb93-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="abb93-146">响应</span><span class="sxs-lookup"><span data-stu-id="abb93-146">Response</span></span>

<span data-ttu-id="abb93-147">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[passwordCredential](../resources/passwordcredential.md)对象。</span><span class="sxs-lookup"><span data-stu-id="abb93-147">If successful, this method returns a `200 OK` response code and a new [passwordCredential](../resources/passwordcredential.md) object in the response body.</span></span> <span data-ttu-id="abb93-148">Response 对象中的**secretText**属性包含由 Azure Active Directory 生成的强密码，其长度为16-64 个字符。</span><span class="sxs-lookup"><span data-stu-id="abb93-148">The **secretText** property in the response object contains the strong passwords generated by Azure Active Directory that are 16-64 characters in length.</span></span> <span data-ttu-id="abb93-149">将来无法检索此密码。</span><span class="sxs-lookup"><span data-stu-id="abb93-149">There is no way to retrieve this password in the future.</span></span>

## <a name="examples"></a><span data-ttu-id="abb93-150">示例</span><span class="sxs-lookup"><span data-stu-id="abb93-150">Examples</span></span>

<span data-ttu-id="abb93-151">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="abb93-151">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="abb93-152">请求</span><span class="sxs-lookup"><span data-stu-id="abb93-152">Request</span></span>

<span data-ttu-id="abb93-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="abb93-153">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="abb93-154">响应</span><span class="sxs-lookup"><span data-stu-id="abb93-154">Response</span></span>

<span data-ttu-id="abb93-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="abb93-155">The following is an example of the response.</span></span>

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
