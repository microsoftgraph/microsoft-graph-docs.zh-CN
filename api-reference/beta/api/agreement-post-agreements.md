---
title: 创建协议
description: 创建新的协议对象。
localization_priority: Normal
ms.openlocfilehash: 5040651e032a4f5d0ef2340646f11eb51bfff5eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514423"
---
# <a name="create-agreement"></a><span data-ttu-id="91fe6-103">创建协议</span><span class="sxs-lookup"><span data-stu-id="91fe6-103">Create agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91fe6-104">创建新的[协议](../resources/agreement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="91fe6-104">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="91fe6-105">权限</span><span class="sxs-lookup"><span data-stu-id="91fe6-105">Permissions</span></span>
<span data-ttu-id="91fe6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91fe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91fe6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="91fe6-108">Permission type</span></span>                        | <span data-ttu-id="91fe6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91fe6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="91fe6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91fe6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="91fe6-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91fe6-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="91fe6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91fe6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91fe6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="91fe6-113">Not supported.</span></span> |
|<span data-ttu-id="91fe6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="91fe6-114">Application</span></span>                            | <span data-ttu-id="91fe6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="91fe6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91fe6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91fe6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="91fe6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="91fe6-117">Request headers</span></span>
| <span data-ttu-id="91fe6-118">名称</span><span class="sxs-lookup"><span data-stu-id="91fe6-118">Name</span></span>         | <span data-ttu-id="91fe6-119">类型</span><span class="sxs-lookup"><span data-stu-id="91fe6-119">Type</span></span>        | <span data-ttu-id="91fe6-120">说明</span><span class="sxs-lookup"><span data-stu-id="91fe6-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="91fe6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="91fe6-121">Authorization</span></span> | <span data-ttu-id="91fe6-122">字符串</span><span class="sxs-lookup"><span data-stu-id="91fe6-122">string</span></span> | <span data-ttu-id="91fe6-123">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="91fe6-123">Bearer \{token\}.</span></span> <span data-ttu-id="91fe6-124">必需。</span><span class="sxs-lookup"><span data-stu-id="91fe6-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91fe6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="91fe6-125">Request body</span></span>
<span data-ttu-id="91fe6-126">在请求正文中，提供[协议](../resources/agreement.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91fe6-126">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="91fe6-127">下表显示创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="91fe6-127">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="91fe6-128">属性</span><span class="sxs-lookup"><span data-stu-id="91fe6-128">Property</span></span>     | <span data-ttu-id="91fe6-129">类型</span><span class="sxs-lookup"><span data-stu-id="91fe6-129">Type</span></span>        | <span data-ttu-id="91fe6-130">说明</span><span class="sxs-lookup"><span data-stu-id="91fe6-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="91fe6-131">displayName</span><span class="sxs-lookup"><span data-stu-id="91fe6-131">displayName</span></span>|<span data-ttu-id="91fe6-132">String</span><span class="sxs-lookup"><span data-stu-id="91fe6-132">String</span></span>|<span data-ttu-id="91fe6-133">协议中的显示名称。</span><span class="sxs-lookup"><span data-stu-id="91fe6-133">Display name of the agreement.</span></span>|
|<span data-ttu-id="91fe6-134">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="91fe6-134">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="91fe6-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="91fe6-135">Boolean</span></span>|<span data-ttu-id="91fe6-136">指示用户是否能够展开和查看接受之前协议。</span><span class="sxs-lookup"><span data-stu-id="91fe6-136">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="91fe6-137">文件/文件名</span><span class="sxs-lookup"><span data-stu-id="91fe6-137">files/fileName</span></span>|<span data-ttu-id="91fe6-138">String</span><span class="sxs-lookup"><span data-stu-id="91fe6-138">String</span></span>|<span data-ttu-id="91fe6-139">协议文件 (例如，TOU.pdf) 的名称。</span><span class="sxs-lookup"><span data-stu-id="91fe6-139">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="91fe6-140">文件/isDefault</span><span class="sxs-lookup"><span data-stu-id="91fe6-140">files/isDefault</span></span>|<span data-ttu-id="91fe6-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="91fe6-141">Boolean</span></span>|<span data-ttu-id="91fe6-142">指示是否这是默认协议文件，是否无区域性匹配的客户端首选项。</span><span class="sxs-lookup"><span data-stu-id="91fe6-142">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="91fe6-143">如果没有文件被标记为默认，第一个将被视为默认。</span><span class="sxs-lookup"><span data-stu-id="91fe6-143">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="91fe6-144">文件/语言</span><span class="sxs-lookup"><span data-stu-id="91fe6-144">files/language</span></span>|<span data-ttu-id="91fe6-145">String</span><span class="sxs-lookup"><span data-stu-id="91fe6-145">String</span></span>|<span data-ttu-id="91fe6-146">区域性格式 languagecode2-国家/地区/regioncode2 中的协议文件。</span><span class="sxs-lookup"><span data-stu-id="91fe6-146">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="91fe6-147">languagecode2 是小写字母双字母代码派生自 ISO 639-1。</span><span class="sxs-lookup"><span data-stu-id="91fe6-147">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="91fe6-148">国家/地区/regioncode2 派生自 ISO 3166，它通常包括两个大写字母或 BCP 47 语言标记 (例如，EN-US)。</span><span class="sxs-lookup"><span data-stu-id="91fe6-148">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="91fe6-149">文件/fileData/数据</span><span class="sxs-lookup"><span data-stu-id="91fe6-149">files/fileData/data</span></span>|<span data-ttu-id="91fe6-150">Binary</span><span class="sxs-lookup"><span data-stu-id="91fe6-150">Binary</span></span>|<span data-ttu-id="91fe6-151">代表使用条款 PDF 文档的数据。</span><span class="sxs-lookup"><span data-stu-id="91fe6-151">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="91fe6-152">响应</span><span class="sxs-lookup"><span data-stu-id="91fe6-152">Response</span></span>
<span data-ttu-id="91fe6-153">如果成功，此方法返回`201, Created`响应正文中的响应代码和[协议](../resources/agreement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="91fe6-153">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91fe6-154">示例</span><span class="sxs-lookup"><span data-stu-id="91fe6-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91fe6-155">请求</span><span class="sxs-lookup"><span data-stu-id="91fe6-155">Request</span></span>
<span data-ttu-id="91fe6-156">在请求正文中，提供[协议](../resources/agreement.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91fe6-156">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="91fe6-157">响应</span><span class="sxs-lookup"><span data-stu-id="91fe6-157">Response</span></span>
><span data-ttu-id="91fe6-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="91fe6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/agreement-post-agreements.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
