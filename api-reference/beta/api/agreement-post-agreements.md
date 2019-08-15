---
title: 创建协议
description: 创建新的协议对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3d948fa3d642302a8e75fb474edf26df08092b49
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408487"
---
# <a name="create-agreement"></a><span data-ttu-id="fe5ef-103">创建协议</span><span class="sxs-lookup"><span data-stu-id="fe5ef-103">Create agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe5ef-104">创建新的[协议](../resources/agreement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-104">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe5ef-105">权限</span><span class="sxs-lookup"><span data-stu-id="fe5ef-105">Permissions</span></span>
<span data-ttu-id="fe5ef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe5ef-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe5ef-108">Permission type</span></span>                        | <span data-ttu-id="fe5ef-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe5ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe5ef-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe5ef-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe5ef-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe5ef-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="fe5ef-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe5ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe5ef-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-113">Not supported.</span></span> |
|<span data-ttu-id="fe5ef-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe5ef-114">Application</span></span>                            | <span data-ttu-id="fe5ef-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe5ef-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe5ef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="fe5ef-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe5ef-117">Request headers</span></span>
| <span data-ttu-id="fe5ef-118">名称</span><span class="sxs-lookup"><span data-stu-id="fe5ef-118">Name</span></span>         | <span data-ttu-id="fe5ef-119">类型</span><span class="sxs-lookup"><span data-stu-id="fe5ef-119">Type</span></span>        | <span data-ttu-id="fe5ef-120">说明</span><span class="sxs-lookup"><span data-stu-id="fe5ef-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fe5ef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe5ef-121">Authorization</span></span> | <span data-ttu-id="fe5ef-122">string</span><span class="sxs-lookup"><span data-stu-id="fe5ef-122">string</span></span> | <span data-ttu-id="fe5ef-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe5ef-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe5ef-125">Request body</span></span>
<span data-ttu-id="fe5ef-126">在请求正文中, 提供[协议](../resources/agreement.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-126">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="fe5ef-127">下表显示创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-127">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="fe5ef-128">属性</span><span class="sxs-lookup"><span data-stu-id="fe5ef-128">Property</span></span>     | <span data-ttu-id="fe5ef-129">类型</span><span class="sxs-lookup"><span data-stu-id="fe5ef-129">Type</span></span>        | <span data-ttu-id="fe5ef-130">说明</span><span class="sxs-lookup"><span data-stu-id="fe5ef-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fe5ef-131">displayName</span><span class="sxs-lookup"><span data-stu-id="fe5ef-131">displayName</span></span>|<span data-ttu-id="fe5ef-132">String</span><span class="sxs-lookup"><span data-stu-id="fe5ef-132">String</span></span>|<span data-ttu-id="fe5ef-133">协议的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-133">Display name of the agreement.</span></span>|
|<span data-ttu-id="fe5ef-134">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="fe5ef-134">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="fe5ef-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe5ef-135">Boolean</span></span>|<span data-ttu-id="fe5ef-136">指示用户是否必须在接受前展开并查看协议。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-136">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="fe5ef-137">files/fileName</span><span class="sxs-lookup"><span data-stu-id="fe5ef-137">files/fileName</span></span>|<span data-ttu-id="fe5ef-138">String</span><span class="sxs-lookup"><span data-stu-id="fe5ef-138">String</span></span>|<span data-ttu-id="fe5ef-139">协议文件的名称 (例如, TOU)。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-139">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="fe5ef-140">files/isDefault</span><span class="sxs-lookup"><span data-stu-id="fe5ef-140">files/isDefault</span></span>|<span data-ttu-id="fe5ef-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe5ef-141">Boolean</span></span>|<span data-ttu-id="fe5ef-142">指示是否为默认协议文件 (如果没有任何区域性与客户端首选项匹配)。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-142">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="fe5ef-143">如果没有任何文件被标记为默认值, 则第一项将被视为默认值。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-143">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="fe5ef-144">文件/语言</span><span class="sxs-lookup"><span data-stu-id="fe5ef-144">files/language</span></span>|<span data-ttu-id="fe5ef-145">String</span><span class="sxs-lookup"><span data-stu-id="fe5ef-145">String</span></span>|<span data-ttu-id="fe5ef-146">协议文件的区域性 (格式为 languagecode2/regioncode2)。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-146">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="fe5ef-147">languagecode2 是从 ISO 639-1 派生的一个由两个小写字母组成的代码。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-147">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="fe5ef-148">国家/regioncode2 派生自 ISO 3166, 通常包含两个大写字母或一个 BCP-47 语言标记 (例如 en-us)。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-148">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="fe5ef-149">files/fileData/data</span><span class="sxs-lookup"><span data-stu-id="fe5ef-149">files/fileData/data</span></span>|<span data-ttu-id="fe5ef-150">Binary</span><span class="sxs-lookup"><span data-stu-id="fe5ef-150">Binary</span></span>|<span data-ttu-id="fe5ef-151">表示使用 PDF 文档的术语的数据。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-151">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="fe5ef-152">响应</span><span class="sxs-lookup"><span data-stu-id="fe5ef-152">Response</span></span>
<span data-ttu-id="fe5ef-153">如果成功, 此方法在响应`201, Created`正文中返回响应代码和[协议](../resources/agreement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-153">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe5ef-154">示例</span><span class="sxs-lookup"><span data-stu-id="fe5ef-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe5ef-155">请求</span><span class="sxs-lookup"><span data-stu-id="fe5ef-155">Request</span></span>
<span data-ttu-id="fe5ef-156">在请求正文中, 提供[协议](../resources/agreement.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-156">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fe5ef-157">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fe5ef-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/beta/agreements
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fe5ef-158">C#</span><span class="sxs-lookup"><span data-stu-id="fe5ef-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe5ef-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe5ef-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fe5ef-160">目标-C</span><span class="sxs-lookup"><span data-stu-id="fe5ef-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fe5ef-161">响应</span><span class="sxs-lookup"><span data-stu-id="fe5ef-161">Response</span></span>
><span data-ttu-id="fe5ef-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fe5ef-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
