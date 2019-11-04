---
title: 'trustFrameworkKeySet: uploadSecret'
description: 将密码上载到键集。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 13742cee46164eaf2e21c4eefa2e8655fa4a567e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937477"
---
# <a name="trustframeworkkeyset-uploadsecret"></a><span data-ttu-id="34a77-103">trustFrameworkKeySet: uploadSecret</span><span class="sxs-lookup"><span data-stu-id="34a77-103">trustFrameworkKeySet: uploadSecret</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34a77-104">将纯文本机密上载到[trustFrameworkKeyset](../resources/trustframeworkkeyset.md)。</span><span class="sxs-lookup"><span data-stu-id="34a77-104">Upload a plain text secret to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="34a77-105">密码示例包括 Azure Active Directory、Google、Facebook 或任何其他标识提供程序中的应用程序机密。</span><span class="sxs-lookup"><span data-stu-id="34a77-105">Examples of secrets are application secrets in Azure Active Directory, Google, Facebook, or any other identity provider.</span></span> <span data-ttu-id="34a77-106">他的方法返回[trustFrameworkKey](../resources/trustframeworkkey.md)。</span><span class="sxs-lookup"><span data-stu-id="34a77-106">his method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="34a77-107">权限</span><span class="sxs-lookup"><span data-stu-id="34a77-107">Permissions</span></span>

<span data-ttu-id="34a77-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34a77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34a77-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="34a77-110">Permission type</span></span>                        | <span data-ttu-id="34a77-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="34a77-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="34a77-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34a77-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="34a77-113">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="34a77-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="34a77-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34a77-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34a77-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="34a77-115">Not supported.</span></span> |
| <span data-ttu-id="34a77-116">Application</span><span class="sxs-lookup"><span data-stu-id="34a77-116">Application</span></span>                            | <span data-ttu-id="34a77-117">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="34a77-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34a77-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34a77-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadSecret
```

## <a name="request-headers"></a><span data-ttu-id="34a77-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="34a77-119">Request headers</span></span>

| <span data-ttu-id="34a77-120">名称</span><span class="sxs-lookup"><span data-stu-id="34a77-120">Name</span></span>          | <span data-ttu-id="34a77-121">说明</span><span class="sxs-lookup"><span data-stu-id="34a77-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="34a77-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="34a77-122">Authorization</span></span> | <span data-ttu-id="34a77-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="34a77-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34a77-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="34a77-125">Content-type</span></span>  | <span data-ttu-id="34a77-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="34a77-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34a77-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="34a77-128">Request body</span></span>

<span data-ttu-id="34a77-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="34a77-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="34a77-130">参数</span><span class="sxs-lookup"><span data-stu-id="34a77-130">Parameter</span></span>    | <span data-ttu-id="34a77-131">类型</span><span class="sxs-lookup"><span data-stu-id="34a77-131">Type</span></span>        | <span data-ttu-id="34a77-132">描述</span><span class="sxs-lookup"><span data-stu-id="34a77-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="34a77-133">改用</span><span class="sxs-lookup"><span data-stu-id="34a77-133">use</span></span>|<span data-ttu-id="34a77-134">字符串</span><span class="sxs-lookup"><span data-stu-id="34a77-134">String</span></span>|<span data-ttu-id="34a77-135">与**trustFrameworkKey**的**use**属性类似。</span><span class="sxs-lookup"><span data-stu-id="34a77-135">Similar to the **use** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="34a77-136">kb</span><span class="sxs-lookup"><span data-stu-id="34a77-136">k</span></span>|<span data-ttu-id="34a77-137">字符串</span><span class="sxs-lookup"><span data-stu-id="34a77-137">String</span></span>|<span data-ttu-id="34a77-138">类似于**trustFrameworkKey**的**k**属性。</span><span class="sxs-lookup"><span data-stu-id="34a77-138">Similar to the **k** property of **trustFrameworkKey**.</span></span> <span data-ttu-id="34a77-139">这是用于发送密码的字段。</span><span class="sxs-lookup"><span data-stu-id="34a77-139">This is the field that is used to send the secret.</span></span>|
|<span data-ttu-id="34a77-140">nbf</span><span class="sxs-lookup"><span data-stu-id="34a77-140">nbf</span></span>|<span data-ttu-id="34a77-141">Int64</span><span class="sxs-lookup"><span data-stu-id="34a77-141">Int64</span></span>|<span data-ttu-id="34a77-142">类似于**trustFrameworkKey**的**nbf**属性。</span><span class="sxs-lookup"><span data-stu-id="34a77-142">Similar to the **nbf** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="34a77-143">exp</span><span class="sxs-lookup"><span data-stu-id="34a77-143">exp</span></span>|<span data-ttu-id="34a77-144">Int64</span><span class="sxs-lookup"><span data-stu-id="34a77-144">Int64</span></span>|<span data-ttu-id="34a77-145">与**trustFrameworkKey**的**exp**属性类似。</span><span class="sxs-lookup"><span data-stu-id="34a77-145">Similar to the **exp** property of **trustFrameworkKey**.</span></span>|

## <a name="response"></a><span data-ttu-id="34a77-146">响应</span><span class="sxs-lookup"><span data-stu-id="34a77-146">Response</span></span>

<span data-ttu-id="34a77-147">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[trustFrameworkKey](../resources/trustframeworkkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="34a77-147">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="34a77-148">示例</span><span class="sxs-lookup"><span data-stu-id="34a77-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="34a77-149">请求</span><span class="sxs-lookup"><span data-stu-id="34a77-149">Request</span></span>

<span data-ttu-id="34a77-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="34a77-150">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="34a77-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="34a77-151">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="34a77-152">C#</span><span class="sxs-lookup"><span data-stu-id="34a77-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadsecret-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="34a77-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34a77-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadsecret-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="34a77-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34a77-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadsecret-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="34a77-155">响应</span><span class="sxs-lookup"><span data-stu-id="34a77-155">Response</span></span>

<span data-ttu-id="34a77-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="34a77-156">The following is an example of the response.</span></span>

> <span data-ttu-id="34a77-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="34a77-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
