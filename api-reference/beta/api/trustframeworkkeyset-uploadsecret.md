---
title: 'trustFrameworkKeySet: uploadSecret'
description: 将密码上载到键集。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0323e861e1ffa83eb3bedf2e850f8580f858d642
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452111"
---
# <a name="trustframeworkkeyset-uploadsecret"></a><span data-ttu-id="273c0-103">trustFrameworkKeySet: uploadSecret</span><span class="sxs-lookup"><span data-stu-id="273c0-103">trustFrameworkKeySet: uploadSecret</span></span>

<span data-ttu-id="273c0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="273c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="273c0-105">将纯文本机密上载到[trustFrameworkKeyset](../resources/trustframeworkkeyset.md)。</span><span class="sxs-lookup"><span data-stu-id="273c0-105">Upload a plain text secret to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="273c0-106">密码示例包括 Azure Active Directory、Google、Facebook 或任何其他标识提供程序中的应用程序机密。</span><span class="sxs-lookup"><span data-stu-id="273c0-106">Examples of secrets are application secrets in Azure Active Directory, Google, Facebook, or any other identity provider.</span></span> <span data-ttu-id="273c0-107">他的方法返回[trustFrameworkKey](../resources/trustframeworkkey.md)。</span><span class="sxs-lookup"><span data-stu-id="273c0-107">his method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="273c0-108">权限</span><span class="sxs-lookup"><span data-stu-id="273c0-108">Permissions</span></span>

<span data-ttu-id="273c0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="273c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="273c0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="273c0-111">Permission type</span></span>                        | <span data-ttu-id="273c0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="273c0-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="273c0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="273c0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="273c0-114">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="273c0-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="273c0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="273c0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="273c0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="273c0-116">Not supported.</span></span> |
| <span data-ttu-id="273c0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="273c0-117">Application</span></span>                            | <span data-ttu-id="273c0-118">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="273c0-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="273c0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="273c0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadSecret
```

## <a name="request-headers"></a><span data-ttu-id="273c0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="273c0-120">Request headers</span></span>

| <span data-ttu-id="273c0-121">名称</span><span class="sxs-lookup"><span data-stu-id="273c0-121">Name</span></span>          | <span data-ttu-id="273c0-122">说明</span><span class="sxs-lookup"><span data-stu-id="273c0-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="273c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="273c0-123">Authorization</span></span> | <span data-ttu-id="273c0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="273c0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="273c0-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="273c0-126">Content-type</span></span>  | <span data-ttu-id="273c0-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="273c0-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="273c0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="273c0-129">Request body</span></span>

<span data-ttu-id="273c0-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="273c0-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="273c0-131">参数</span><span class="sxs-lookup"><span data-stu-id="273c0-131">Parameter</span></span>    | <span data-ttu-id="273c0-132">类型</span><span class="sxs-lookup"><span data-stu-id="273c0-132">Type</span></span>        | <span data-ttu-id="273c0-133">说明</span><span class="sxs-lookup"><span data-stu-id="273c0-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="273c0-134">改用</span><span class="sxs-lookup"><span data-stu-id="273c0-134">use</span></span>|<span data-ttu-id="273c0-135">String</span><span class="sxs-lookup"><span data-stu-id="273c0-135">String</span></span>|<span data-ttu-id="273c0-136">与**trustFrameworkKey**的**use**属性类似。</span><span class="sxs-lookup"><span data-stu-id="273c0-136">Similar to the **use** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="273c0-137">kb</span><span class="sxs-lookup"><span data-stu-id="273c0-137">k</span></span>|<span data-ttu-id="273c0-138">String</span><span class="sxs-lookup"><span data-stu-id="273c0-138">String</span></span>|<span data-ttu-id="273c0-139">类似于**trustFrameworkKey**的**k**属性。</span><span class="sxs-lookup"><span data-stu-id="273c0-139">Similar to the **k** property of **trustFrameworkKey**.</span></span> <span data-ttu-id="273c0-140">这是用于发送密码的字段。</span><span class="sxs-lookup"><span data-stu-id="273c0-140">This is the field that is used to send the secret.</span></span>|
|<span data-ttu-id="273c0-141">nbf</span><span class="sxs-lookup"><span data-stu-id="273c0-141">nbf</span></span>|<span data-ttu-id="273c0-142">Int64</span><span class="sxs-lookup"><span data-stu-id="273c0-142">Int64</span></span>|<span data-ttu-id="273c0-143">类似于**trustFrameworkKey**的**nbf**属性。</span><span class="sxs-lookup"><span data-stu-id="273c0-143">Similar to the **nbf** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="273c0-144">exp</span><span class="sxs-lookup"><span data-stu-id="273c0-144">exp</span></span>|<span data-ttu-id="273c0-145">Int64</span><span class="sxs-lookup"><span data-stu-id="273c0-145">Int64</span></span>|<span data-ttu-id="273c0-146">与**trustFrameworkKey**的**exp**属性类似。</span><span class="sxs-lookup"><span data-stu-id="273c0-146">Similar to the **exp** property of **trustFrameworkKey**.</span></span>|

## <a name="response"></a><span data-ttu-id="273c0-147">响应</span><span class="sxs-lookup"><span data-stu-id="273c0-147">Response</span></span>

<span data-ttu-id="273c0-148">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[trustFrameworkKey](../resources/trustframeworkkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="273c0-148">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="273c0-149">示例</span><span class="sxs-lookup"><span data-stu-id="273c0-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="273c0-150">请求</span><span class="sxs-lookup"><span data-stu-id="273c0-150">Request</span></span>

<span data-ttu-id="273c0-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="273c0-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="273c0-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="273c0-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="273c0-153">C#</span><span class="sxs-lookup"><span data-stu-id="273c0-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadsecret-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="273c0-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="273c0-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadsecret-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="273c0-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="273c0-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadsecret-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="273c0-156">响应</span><span class="sxs-lookup"><span data-stu-id="273c0-156">Response</span></span>

<span data-ttu-id="273c0-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="273c0-157">The following is an example of the response.</span></span>

> <span data-ttu-id="273c0-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="273c0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
