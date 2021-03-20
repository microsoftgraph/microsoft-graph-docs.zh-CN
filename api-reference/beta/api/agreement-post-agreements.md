---
title: 创建协议
description: 创建新的协议对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 491c91bb36d2ad3ba55f0f9ad8c2ad2765f15a2c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942888"
---
# <a name="create-agreement"></a><span data-ttu-id="90d5e-103">创建协议</span><span class="sxs-lookup"><span data-stu-id="90d5e-103">Create agreement</span></span>

<span data-ttu-id="90d5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90d5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90d5e-105">创建新的 [协议](../resources/agreement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90d5e-105">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="90d5e-106">权限</span><span class="sxs-lookup"><span data-stu-id="90d5e-106">Permissions</span></span>
<span data-ttu-id="90d5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90d5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90d5e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="90d5e-109">Permission type</span></span>                        | <span data-ttu-id="90d5e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90d5e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="90d5e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90d5e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="90d5e-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90d5e-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="90d5e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90d5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90d5e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="90d5e-114">Not supported.</span></span> |
|<span data-ttu-id="90d5e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="90d5e-115">Application</span></span>                            | <span data-ttu-id="90d5e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="90d5e-116">Not supported.</span></span> |

<span data-ttu-id="90d5e-117">代表用户进行呼叫时，用户需要属于以下目录角色之一。</span><span class="sxs-lookup"><span data-stu-id="90d5e-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="90d5e-118">若要了解有关目录角色的信息，请参阅 [Azure AD 内置角色](/azure/active-directory/roles/permissions-reference)：</span><span class="sxs-lookup"><span data-stu-id="90d5e-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="90d5e-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="90d5e-119">Global Administrator</span></span>
+ <span data-ttu-id="90d5e-120">条件访问管理员</span><span class="sxs-lookup"><span data-stu-id="90d5e-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="90d5e-121">安全管理员</span><span class="sxs-lookup"><span data-stu-id="90d5e-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="90d5e-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90d5e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/termsOfUse/agreements
```
## <a name="request-headers"></a><span data-ttu-id="90d5e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="90d5e-123">Request headers</span></span>
| <span data-ttu-id="90d5e-124">名称</span><span class="sxs-lookup"><span data-stu-id="90d5e-124">Name</span></span>         | <span data-ttu-id="90d5e-125">类型</span><span class="sxs-lookup"><span data-stu-id="90d5e-125">Type</span></span>        | <span data-ttu-id="90d5e-126">说明</span><span class="sxs-lookup"><span data-stu-id="90d5e-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="90d5e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="90d5e-127">Authorization</span></span> | <span data-ttu-id="90d5e-128">string</span><span class="sxs-lookup"><span data-stu-id="90d5e-128">string</span></span> | <span data-ttu-id="90d5e-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="90d5e-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90d5e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="90d5e-131">Request body</span></span>
<span data-ttu-id="90d5e-132">在请求正文中，提供 agreement 对象的 JSON [表示](../resources/agreement.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="90d5e-132">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="90d5e-133">下表显示创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="90d5e-133">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="90d5e-134">属性</span><span class="sxs-lookup"><span data-stu-id="90d5e-134">Property</span></span>     | <span data-ttu-id="90d5e-135">类型</span><span class="sxs-lookup"><span data-stu-id="90d5e-135">Type</span></span>        | <span data-ttu-id="90d5e-136">说明</span><span class="sxs-lookup"><span data-stu-id="90d5e-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="90d5e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="90d5e-137">displayName</span></span>|<span data-ttu-id="90d5e-138">String</span><span class="sxs-lookup"><span data-stu-id="90d5e-138">String</span></span>|<span data-ttu-id="90d5e-139">协议的显示名称。</span><span class="sxs-lookup"><span data-stu-id="90d5e-139">Display name of the agreement.</span></span>|
|<span data-ttu-id="90d5e-140">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="90d5e-140">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="90d5e-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d5e-141">Boolean</span></span>|<span data-ttu-id="90d5e-142">指示用户在接受之前是否必须展开和查看协议。</span><span class="sxs-lookup"><span data-stu-id="90d5e-142">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="90d5e-143">files/fileName</span><span class="sxs-lookup"><span data-stu-id="90d5e-143">files/fileName</span></span>|<span data-ttu-id="90d5e-144">String</span><span class="sxs-lookup"><span data-stu-id="90d5e-144">String</span></span>|<span data-ttu-id="90d5e-145">协议文件的名称 (例如，TOU.pdf) 。</span><span class="sxs-lookup"><span data-stu-id="90d5e-145">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="90d5e-146">files/isDefault</span><span class="sxs-lookup"><span data-stu-id="90d5e-146">files/isDefault</span></span>|<span data-ttu-id="90d5e-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="90d5e-147">Boolean</span></span>|<span data-ttu-id="90d5e-148">指示当没有任何区域性与客户端首选项匹配时，这是否是默认协议文件。</span><span class="sxs-lookup"><span data-stu-id="90d5e-148">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="90d5e-149">如果没有文件标记为默认文件，则第一个文件将被视为默认文件。</span><span class="sxs-lookup"><span data-stu-id="90d5e-149">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="90d5e-150">文件/语言</span><span class="sxs-lookup"><span data-stu-id="90d5e-150">files/language</span></span>|<span data-ttu-id="90d5e-151">String</span><span class="sxs-lookup"><span data-stu-id="90d5e-151">String</span></span>|<span data-ttu-id="90d5e-152">格式为 languagecode2-country/regioncode2 的协议文件的区域性。</span><span class="sxs-lookup"><span data-stu-id="90d5e-152">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="90d5e-153">languagecode2 是从 ISO 639-1 派生的两个字母小写代码。</span><span class="sxs-lookup"><span data-stu-id="90d5e-153">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="90d5e-154">country/regioncode2 派生自 ISO 3166，通常由两个小写字母或 BCP-47 语言标记 (例如 en-US) 。</span><span class="sxs-lookup"><span data-stu-id="90d5e-154">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="90d5e-155">files/fileData/data</span><span class="sxs-lookup"><span data-stu-id="90d5e-155">files/fileData/data</span></span>|<span data-ttu-id="90d5e-156">Binary</span><span class="sxs-lookup"><span data-stu-id="90d5e-156">Binary</span></span>|<span data-ttu-id="90d5e-157">表示 PDF 文档的使用条款的数据。</span><span class="sxs-lookup"><span data-stu-id="90d5e-157">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="90d5e-158">响应</span><span class="sxs-lookup"><span data-stu-id="90d5e-158">Response</span></span>
<span data-ttu-id="90d5e-159">如果成功，此方法在响应 `201, Created` 正文中返回 [响应](../resources/agreement.md) 代码和 agreement 对象。</span><span class="sxs-lookup"><span data-stu-id="90d5e-159">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90d5e-160">示例</span><span class="sxs-lookup"><span data-stu-id="90d5e-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90d5e-161">请求</span><span class="sxs-lookup"><span data-stu-id="90d5e-161">Request</span></span>
<span data-ttu-id="90d5e-162">在请求正文中，提供协议对象的 JSON [表示](../resources/agreement.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="90d5e-162">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="90d5e-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="90d5e-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements
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
# <a name="c"></a>[<span data-ttu-id="90d5e-164">C#</span><span class="sxs-lookup"><span data-stu-id="90d5e-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90d5e-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90d5e-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90d5e-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90d5e-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90d5e-167">Java</span><span class="sxs-lookup"><span data-stu-id="90d5e-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-agreement-from-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="90d5e-168">响应</span><span class="sxs-lookup"><span data-stu-id="90d5e-168">Response</span></span>
><span data-ttu-id="90d5e-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="90d5e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "id": "id-value"
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


