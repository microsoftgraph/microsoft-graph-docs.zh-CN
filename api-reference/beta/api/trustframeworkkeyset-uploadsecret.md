---
title: trustFrameworkKeySet：uploadSecret
description: 将密码上载到密钥集。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b008e1ae41d61fb14dbd80e5a820208355bb670d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444971"
---
# <a name="trustframeworkkeyset-uploadsecret"></a><span data-ttu-id="3e640-103">trustFrameworkKeySet：uploadSecret</span><span class="sxs-lookup"><span data-stu-id="3e640-103">trustFrameworkKeySet: uploadSecret</span></span>

<span data-ttu-id="3e640-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e640-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e640-105">将纯文本密码上载到 [trustFrameworkKeyset](../resources/trustframeworkkeyset.md)。</span><span class="sxs-lookup"><span data-stu-id="3e640-105">Upload a plain text secret to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="3e640-106">密码示例包括 Azure Active Directory、Google、Facebook 或其他任何标识提供程序中的应用程序密码。</span><span class="sxs-lookup"><span data-stu-id="3e640-106">Examples of secrets are application secrets in Azure Active Directory, Google, Facebook, or any other identity provider.</span></span> <span data-ttu-id="3e640-107">他的方法返回 [trustFrameworkKey](../resources/trustframeworkkey.md)。</span><span class="sxs-lookup"><span data-stu-id="3e640-107">his method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e640-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="3e640-108">Permissions</span></span>

<span data-ttu-id="3e640-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e640-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e640-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e640-111">Permission type</span></span>                        | <span data-ttu-id="3e640-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e640-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3e640-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e640-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e640-114">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e640-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="3e640-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e640-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e640-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e640-116">Not supported.</span></span> |
| <span data-ttu-id="3e640-117">Application</span><span class="sxs-lookup"><span data-stu-id="3e640-117">Application</span></span>                            | <span data-ttu-id="3e640-118">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e640-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e640-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e640-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadSecret
```

## <a name="request-headers"></a><span data-ttu-id="3e640-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e640-120">Request headers</span></span>

| <span data-ttu-id="3e640-121">名称</span><span class="sxs-lookup"><span data-stu-id="3e640-121">Name</span></span>          | <span data-ttu-id="3e640-122">说明</span><span class="sxs-lookup"><span data-stu-id="3e640-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3e640-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e640-123">Authorization</span></span> | <span data-ttu-id="3e640-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e640-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e640-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="3e640-126">Content-type</span></span>  | <span data-ttu-id="3e640-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3e640-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e640-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e640-129">Request body</span></span>

<span data-ttu-id="3e640-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3e640-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3e640-131">参数</span><span class="sxs-lookup"><span data-stu-id="3e640-131">Parameter</span></span>    | <span data-ttu-id="3e640-132">类型</span><span class="sxs-lookup"><span data-stu-id="3e640-132">Type</span></span>        | <span data-ttu-id="3e640-133">说明</span><span class="sxs-lookup"><span data-stu-id="3e640-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e640-134">use</span><span class="sxs-lookup"><span data-stu-id="3e640-134">use</span></span>|<span data-ttu-id="3e640-135">String</span><span class="sxs-lookup"><span data-stu-id="3e640-135">String</span></span>|<span data-ttu-id="3e640-136">类似于 **trustFrameworkKey 的 use 属性**。 </span><span class="sxs-lookup"><span data-stu-id="3e640-136">Similar to the **use** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="3e640-137">k</span><span class="sxs-lookup"><span data-stu-id="3e640-137">k</span></span>|<span data-ttu-id="3e640-138">String</span><span class="sxs-lookup"><span data-stu-id="3e640-138">String</span></span>|<span data-ttu-id="3e640-139">类似于 **trustFrameworkKey** 的 **k** 属性。</span><span class="sxs-lookup"><span data-stu-id="3e640-139">Similar to the **k** property of **trustFrameworkKey**.</span></span> <span data-ttu-id="3e640-140">这是用于发送密码的字段。</span><span class="sxs-lookup"><span data-stu-id="3e640-140">This is the field that is used to send the secret.</span></span>|
|<span data-ttu-id="3e640-141">nbf</span><span class="sxs-lookup"><span data-stu-id="3e640-141">nbf</span></span>|<span data-ttu-id="3e640-142">Int64</span><span class="sxs-lookup"><span data-stu-id="3e640-142">Int64</span></span>|<span data-ttu-id="3e640-143">类似于 **trustFrameworkKey** 的 **nbf** 属性。</span><span class="sxs-lookup"><span data-stu-id="3e640-143">Similar to the **nbf** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="3e640-144">exp</span><span class="sxs-lookup"><span data-stu-id="3e640-144">exp</span></span>|<span data-ttu-id="3e640-145">Int64</span><span class="sxs-lookup"><span data-stu-id="3e640-145">Int64</span></span>|<span data-ttu-id="3e640-146">类似于 **trustFrameworkKey 的** **exp** 属性。</span><span class="sxs-lookup"><span data-stu-id="3e640-146">Similar to the **exp** property of **trustFrameworkKey**.</span></span>|

## <a name="response"></a><span data-ttu-id="3e640-147">响应</span><span class="sxs-lookup"><span data-stu-id="3e640-147">Response</span></span>

<span data-ttu-id="3e640-148">如果成功，此方法在响应正文中返回响应代码和新 `200 OK` [trustFrameworkKey](../resources/trustframeworkkey.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3e640-148">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3e640-149">示例</span><span class="sxs-lookup"><span data-stu-id="3e640-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3e640-150">请求</span><span class="sxs-lookup"><span data-stu-id="3e640-150">Request</span></span>

<span data-ttu-id="3e640-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3e640-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3e640-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e640-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadsecret"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadSecret
Content-type: application/json

{
  "use": "use-value",
  "k": "application-secret-to-be-uploaded",
  "nbf": 1508969811,
  "exp": 1508973711
}
```
# <a name="c"></a>[<span data-ttu-id="3e640-153">C#</span><span class="sxs-lookup"><span data-stu-id="3e640-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadsecret-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e640-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e640-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadsecret-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e640-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e640-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadsecret-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3e640-156">Java</span><span class="sxs-lookup"><span data-stu-id="3e640-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-uploadsecret-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3e640-157">响应</span><span class="sxs-lookup"><span data-stu-id="3e640-157">Response</span></span>

<span data-ttu-id="3e640-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3e640-158">The following is an example of the response.</span></span>

> <span data-ttu-id="3e640-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3e640-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "kid": "kid-value",
    "use": "use-value",
    "kty": "OCT",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadSecret",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


