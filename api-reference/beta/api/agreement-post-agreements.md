---
title: 创建协议
description: 创建新的协议对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 53d11dc97d2662906e06b661cd967d5536419a86
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048202"
---
# <a name="create-agreement"></a><span data-ttu-id="259f6-103">创建协议</span><span class="sxs-lookup"><span data-stu-id="259f6-103">Create agreement</span></span>

<span data-ttu-id="259f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="259f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="259f6-105">创建新的 [协议](../resources/agreement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="259f6-105">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="259f6-106">权限</span><span class="sxs-lookup"><span data-stu-id="259f6-106">Permissions</span></span>
<span data-ttu-id="259f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="259f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="259f6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="259f6-109">Permission type</span></span>                        | <span data-ttu-id="259f6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="259f6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="259f6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="259f6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="259f6-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="259f6-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="259f6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="259f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="259f6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="259f6-114">Not supported.</span></span> |
|<span data-ttu-id="259f6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="259f6-115">Application</span></span>                            | <span data-ttu-id="259f6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="259f6-116">Not supported.</span></span> |

<span data-ttu-id="259f6-117">代表用户进行呼叫时，用户需要属于以下目录角色之一。</span><span class="sxs-lookup"><span data-stu-id="259f6-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="259f6-118">若要了解有关目录角色的信息，请参阅 [Azure AD 内置角色](/azure/active-directory/roles/permissions-reference)：</span><span class="sxs-lookup"><span data-stu-id="259f6-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="259f6-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="259f6-119">Global Administrator</span></span>
+ <span data-ttu-id="259f6-120">条件访问管理员</span><span class="sxs-lookup"><span data-stu-id="259f6-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="259f6-121">安全管理员</span><span class="sxs-lookup"><span data-stu-id="259f6-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="259f6-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="259f6-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/termsOfUse/agreements
```
## <a name="request-headers"></a><span data-ttu-id="259f6-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="259f6-123">Request headers</span></span>
| <span data-ttu-id="259f6-124">名称</span><span class="sxs-lookup"><span data-stu-id="259f6-124">Name</span></span>         | <span data-ttu-id="259f6-125">类型</span><span class="sxs-lookup"><span data-stu-id="259f6-125">Type</span></span>        | <span data-ttu-id="259f6-126">说明</span><span class="sxs-lookup"><span data-stu-id="259f6-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="259f6-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="259f6-127">Authorization</span></span> | <span data-ttu-id="259f6-128">string</span><span class="sxs-lookup"><span data-stu-id="259f6-128">string</span></span> | <span data-ttu-id="259f6-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="259f6-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="259f6-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="259f6-131">Request body</span></span>
<span data-ttu-id="259f6-132">在请求正文中，提供 agreement 对象的 JSON [表示](../resources/agreement.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="259f6-132">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="259f6-133">下表显示创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="259f6-133">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="259f6-134">属性</span><span class="sxs-lookup"><span data-stu-id="259f6-134">Property</span></span>     | <span data-ttu-id="259f6-135">类型</span><span class="sxs-lookup"><span data-stu-id="259f6-135">Type</span></span>        | <span data-ttu-id="259f6-136">说明</span><span class="sxs-lookup"><span data-stu-id="259f6-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="259f6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="259f6-137">displayName</span></span>|<span data-ttu-id="259f6-138">String</span><span class="sxs-lookup"><span data-stu-id="259f6-138">String</span></span>|<span data-ttu-id="259f6-139">协议的显示名称。</span><span class="sxs-lookup"><span data-stu-id="259f6-139">Display name of the agreement.</span></span>|
|<span data-ttu-id="259f6-140">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="259f6-140">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="259f6-141">布尔值</span><span class="sxs-lookup"><span data-stu-id="259f6-141">Boolean</span></span>|<span data-ttu-id="259f6-142">指示用户在接受之前是否必须展开和查看协议。</span><span class="sxs-lookup"><span data-stu-id="259f6-142">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="259f6-143">files/fileName</span><span class="sxs-lookup"><span data-stu-id="259f6-143">files/fileName</span></span>|<span data-ttu-id="259f6-144">String</span><span class="sxs-lookup"><span data-stu-id="259f6-144">String</span></span>|<span data-ttu-id="259f6-145">协议文件的名称 (例如，TOU.pdf) 。</span><span class="sxs-lookup"><span data-stu-id="259f6-145">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="259f6-146">files/isDefault</span><span class="sxs-lookup"><span data-stu-id="259f6-146">files/isDefault</span></span>|<span data-ttu-id="259f6-147">布尔值</span><span class="sxs-lookup"><span data-stu-id="259f6-147">Boolean</span></span>|<span data-ttu-id="259f6-148">指示当没有任何区域性与客户端首选项匹配时，这是否是默认协议文件。</span><span class="sxs-lookup"><span data-stu-id="259f6-148">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="259f6-149">如果没有文件标记为默认文件，则第一个文件将被视为默认文件。</span><span class="sxs-lookup"><span data-stu-id="259f6-149">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="259f6-150">文件/语言</span><span class="sxs-lookup"><span data-stu-id="259f6-150">files/language</span></span>|<span data-ttu-id="259f6-151">String</span><span class="sxs-lookup"><span data-stu-id="259f6-151">String</span></span>|<span data-ttu-id="259f6-152">格式为 languagecode2-country/regioncode2 的协议文件的区域性。</span><span class="sxs-lookup"><span data-stu-id="259f6-152">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="259f6-153">languagecode2 是从 ISO 639-1 派生的两个字母小写代码。</span><span class="sxs-lookup"><span data-stu-id="259f6-153">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="259f6-154">country/regioncode2 派生自 ISO 3166，通常由两个小写字母或 BCP-47 语言标记 (例如 en-US) 。</span><span class="sxs-lookup"><span data-stu-id="259f6-154">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="259f6-155">files/fileData/data</span><span class="sxs-lookup"><span data-stu-id="259f6-155">files/fileData/data</span></span>|<span data-ttu-id="259f6-156">二进制</span><span class="sxs-lookup"><span data-stu-id="259f6-156">Binary</span></span>|<span data-ttu-id="259f6-157">表示 PDF 文档的使用条款的数据。</span><span class="sxs-lookup"><span data-stu-id="259f6-157">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="259f6-158">响应</span><span class="sxs-lookup"><span data-stu-id="259f6-158">Response</span></span>
<span data-ttu-id="259f6-159">如果成功，此方法在响应 `201, Created` 正文中返回 [响应](../resources/agreement.md) 代码和 agreement 对象。</span><span class="sxs-lookup"><span data-stu-id="259f6-159">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="259f6-160">示例</span><span class="sxs-lookup"><span data-stu-id="259f6-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="259f6-161">请求</span><span class="sxs-lookup"><span data-stu-id="259f6-161">Request</span></span>
<span data-ttu-id="259f6-162">在请求正文中，提供协议对象的 JSON [表示](../resources/agreement.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="259f6-162">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="259f6-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="259f6-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="259f6-164">C#</span><span class="sxs-lookup"><span data-stu-id="259f6-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="259f6-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="259f6-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="259f6-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="259f6-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="259f6-167">Java</span><span class="sxs-lookup"><span data-stu-id="259f6-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-agreement-from-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="259f6-168">响应</span><span class="sxs-lookup"><span data-stu-id="259f6-168">Response</span></span>
><span data-ttu-id="259f6-169">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="259f6-169">**Note:** The response object shown here might be shortened for readability.</span></span>
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


