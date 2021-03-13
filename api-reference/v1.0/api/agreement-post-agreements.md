---
title: 创建协议
description: 创建新的协议对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 1a3e30754a9359d26c41bad35407674c9b5c88c5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774969"
---
# <a name="create-agreement"></a><span data-ttu-id="c0982-103">创建协议</span><span class="sxs-lookup"><span data-stu-id="c0982-103">Create agreement</span></span>

<span data-ttu-id="c0982-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0982-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0982-105">创建新的 [协议](../resources/agreement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0982-105">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0982-106">权限</span><span class="sxs-lookup"><span data-stu-id="c0982-106">Permissions</span></span>
<span data-ttu-id="c0982-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0982-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0982-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0982-109">Permission type</span></span>                        | <span data-ttu-id="c0982-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0982-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0982-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0982-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0982-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0982-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="c0982-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0982-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0982-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0982-114">Not supported.</span></span> |
|<span data-ttu-id="c0982-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0982-115">Application</span></span>                            | <span data-ttu-id="c0982-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0982-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0982-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0982-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/termsOfUse/agreements
```
## <a name="request-headers"></a><span data-ttu-id="c0982-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0982-118">Request headers</span></span>
| <span data-ttu-id="c0982-119">名称</span><span class="sxs-lookup"><span data-stu-id="c0982-119">Name</span></span>         | <span data-ttu-id="c0982-120">说明</span><span class="sxs-lookup"><span data-stu-id="c0982-120">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="c0982-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0982-121">Authorization</span></span> | <span data-ttu-id="c0982-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="c0982-122">Bearer \{token\}.</span></span> <span data-ttu-id="c0982-123">必需。</span><span class="sxs-lookup"><span data-stu-id="c0982-123">Required.</span></span> |
| <span data-ttu-id="c0982-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="c0982-124">Content-type</span></span>  | <span data-ttu-id="c0982-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c0982-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0982-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0982-127">Request body</span></span>
<span data-ttu-id="c0982-128">在请求正文中，提供协议对象的 JSON [表示](../resources/agreement.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="c0982-128">In the request body, supply a JSON representation of an [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="c0982-129">下表显示创建协议时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c0982-129">The following table shows the properties that are required when you create an agreement.</span></span>

| <span data-ttu-id="c0982-130">属性</span><span class="sxs-lookup"><span data-stu-id="c0982-130">Property</span></span>     | <span data-ttu-id="c0982-131">类型</span><span class="sxs-lookup"><span data-stu-id="c0982-131">Type</span></span>        | <span data-ttu-id="c0982-132">说明</span><span class="sxs-lookup"><span data-stu-id="c0982-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c0982-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c0982-133">displayName</span></span>|<span data-ttu-id="c0982-134">字符串</span><span class="sxs-lookup"><span data-stu-id="c0982-134">String</span></span>|<span data-ttu-id="c0982-135">协议的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c0982-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="c0982-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="c0982-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="c0982-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0982-137">Boolean</span></span>|<span data-ttu-id="c0982-138">指示用户在接受之前是否必须展开和查看协议。</span><span class="sxs-lookup"><span data-stu-id="c0982-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="c0982-139">fileName</span><span class="sxs-lookup"><span data-stu-id="c0982-139">fileName</span></span>|<span data-ttu-id="c0982-140">String</span><span class="sxs-lookup"><span data-stu-id="c0982-140">String</span></span>|<span data-ttu-id="c0982-141">协议文件的名称 (例如，TOU.pdf) 。</span><span class="sxs-lookup"><span data-stu-id="c0982-141">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="c0982-142">isDefault</span><span class="sxs-lookup"><span data-stu-id="c0982-142">isDefault</span></span>|<span data-ttu-id="c0982-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0982-143">Boolean</span></span>|<span data-ttu-id="c0982-144">指示如果语言与客户端首选项匹配，这是否是默认协议文件。</span><span class="sxs-lookup"><span data-stu-id="c0982-144">Indicates whether this is the default agreement file if the language matches the client preference.</span></span> <span data-ttu-id="c0982-145">如果未将任何文件标记为默认文件，则第一个文件将被视为默认文件。</span><span class="sxs-lookup"><span data-stu-id="c0982-145">If none of the files are marked as default, the first one is treated as default.</span></span>|
|<span data-ttu-id="c0982-146">language</span><span class="sxs-lookup"><span data-stu-id="c0982-146">language</span></span>|<span data-ttu-id="c0982-147">String</span><span class="sxs-lookup"><span data-stu-id="c0982-147">String</span></span>|<span data-ttu-id="c0982-148">协议文件的语言，格式为 languagecode2-country/regioncode2。</span><span class="sxs-lookup"><span data-stu-id="c0982-148">The language of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="c0982-149">languagecode2 是从 ISO 639-1 派生的两个字母小写代码。</span><span class="sxs-lookup"><span data-stu-id="c0982-149">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="c0982-150">country/regioncode2 派生自 ISO 3166，通常由两个小写字母或 BCP-47 语言标记 (例如 en-US) 。</span><span class="sxs-lookup"><span data-stu-id="c0982-150">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="c0982-151">data</span><span class="sxs-lookup"><span data-stu-id="c0982-151">data</span></span>|<span data-ttu-id="c0982-152">Binary</span><span class="sxs-lookup"><span data-stu-id="c0982-152">Binary</span></span>|<span data-ttu-id="c0982-153">表示 PDF 文档的使用条款的数据。</span><span class="sxs-lookup"><span data-stu-id="c0982-153">Data that represents the terms of use for the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="c0982-154">响应</span><span class="sxs-lookup"><span data-stu-id="c0982-154">Response</span></span>
<span data-ttu-id="c0982-155">如果成功，此方法在响应 `201, Created` 正文中返回 响应[](../resources/agreement.md)代码和 agreement 对象。</span><span class="sxs-lookup"><span data-stu-id="c0982-155">If successful, this method returns a `201, Created` response code and an [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0982-156">示例</span><span class="sxs-lookup"><span data-stu-id="c0982-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0982-157">请求</span><span class="sxs-lookup"><span data-stu-id="c0982-157">Request</span></span>
<span data-ttu-id="c0982-158">在请求正文中，提供协议对象的 JSON [表示](../resources/agreement.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="c0982-158">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="c0982-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0982-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "files": [
    {
      "fileName": "TOU.pdf",
      "language": "en",
      "isDefault": true,
      "fileData": {
        "data": "SGVsbG8gd29ybGQ="
      }
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="c0982-160">C#</span><span class="sxs-lookup"><span data-stu-id="c0982-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0982-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0982-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0982-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0982-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0982-163">Java</span><span class="sxs-lookup"><span data-stu-id="c0982-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-agreement-from-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c0982-164">响应</span><span class="sxs-lookup"><span data-stu-id="c0982-164">Response</span></span>
><span data-ttu-id="c0982-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c0982-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "093b947f-8363-4979-a47d-4c52b33ee1be"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


