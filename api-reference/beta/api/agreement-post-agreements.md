---
title: 创建协议
description: 创建新的协议对象。
ms.openlocfilehash: bfcab53b4233d133309c99a4825e184a42670458
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042702"
---
# <a name="create-agreement"></a><span data-ttu-id="162a8-103">创建协议</span><span class="sxs-lookup"><span data-stu-id="162a8-103">Create agreement</span></span>

> <span data-ttu-id="162a8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="162a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="162a8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="162a8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="162a8-106">创建新的[协议](../resources/agreement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="162a8-106">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="162a8-107">权限</span><span class="sxs-lookup"><span data-stu-id="162a8-107">Permissions</span></span>
<span data-ttu-id="162a8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="162a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="162a8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="162a8-110">Permission type</span></span>                        | <span data-ttu-id="162a8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="162a8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="162a8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="162a8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="162a8-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="162a8-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="162a8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="162a8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="162a8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="162a8-115">Not supported.</span></span> |
|<span data-ttu-id="162a8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="162a8-116">Application</span></span>                            | <span data-ttu-id="162a8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="162a8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="162a8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="162a8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="162a8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="162a8-119">Request headers</span></span>
| <span data-ttu-id="162a8-120">名称</span><span class="sxs-lookup"><span data-stu-id="162a8-120">Name</span></span>         | <span data-ttu-id="162a8-121">类型</span><span class="sxs-lookup"><span data-stu-id="162a8-121">Type</span></span>        | <span data-ttu-id="162a8-122">说明</span><span class="sxs-lookup"><span data-stu-id="162a8-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="162a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="162a8-123">Authorization</span></span> | <span data-ttu-id="162a8-124">string</span><span class="sxs-lookup"><span data-stu-id="162a8-124">string</span></span> | <span data-ttu-id="162a8-125">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="162a8-125">Bearer \{token\}.</span></span> <span data-ttu-id="162a8-126">必需。</span><span class="sxs-lookup"><span data-stu-id="162a8-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="162a8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="162a8-127">Request body</span></span>
<span data-ttu-id="162a8-128">在请求正文中，提供[协议](../resources/agreement.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="162a8-128">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="162a8-129">下表显示创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="162a8-129">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="162a8-130">属性</span><span class="sxs-lookup"><span data-stu-id="162a8-130">Property</span></span>     | <span data-ttu-id="162a8-131">类型</span><span class="sxs-lookup"><span data-stu-id="162a8-131">Type</span></span>        | <span data-ttu-id="162a8-132">说明</span><span class="sxs-lookup"><span data-stu-id="162a8-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="162a8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="162a8-133">displayName</span></span>|<span data-ttu-id="162a8-134">字符串</span><span class="sxs-lookup"><span data-stu-id="162a8-134">String</span></span>|<span data-ttu-id="162a8-135">协议中的显示名称。</span><span class="sxs-lookup"><span data-stu-id="162a8-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="162a8-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="162a8-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="162a8-137">布尔</span><span class="sxs-lookup"><span data-stu-id="162a8-137">Boolean</span></span>|<span data-ttu-id="162a8-138">指示用户是否能够展开和查看接受之前协议。</span><span class="sxs-lookup"><span data-stu-id="162a8-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="162a8-139">文件/文件名</span><span class="sxs-lookup"><span data-stu-id="162a8-139">files/fileName</span></span>|<span data-ttu-id="162a8-140">字符串</span><span class="sxs-lookup"><span data-stu-id="162a8-140">String</span></span>|<span data-ttu-id="162a8-141">协议文件 (例如，TOU.pdf) 的名称。</span><span class="sxs-lookup"><span data-stu-id="162a8-141">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="162a8-142">文件/isDefault</span><span class="sxs-lookup"><span data-stu-id="162a8-142">files/isDefault</span></span>|<span data-ttu-id="162a8-143">布尔</span><span class="sxs-lookup"><span data-stu-id="162a8-143">Boolean</span></span>|<span data-ttu-id="162a8-144">指示是否这是默认协议文件，是否无区域性匹配的客户端首选项。</span><span class="sxs-lookup"><span data-stu-id="162a8-144">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="162a8-145">如果没有文件被标记为默认，第一个将被视为默认。</span><span class="sxs-lookup"><span data-stu-id="162a8-145">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="162a8-146">文件/语言</span><span class="sxs-lookup"><span data-stu-id="162a8-146">files/language</span></span>|<span data-ttu-id="162a8-147">字符串</span><span class="sxs-lookup"><span data-stu-id="162a8-147">String</span></span>|<span data-ttu-id="162a8-148">区域性格式 languagecode2-国家/地区/regioncode2 中的协议文件。</span><span class="sxs-lookup"><span data-stu-id="162a8-148">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="162a8-149">languagecode2 是小写字母双字母代码派生自 ISO 639-1。</span><span class="sxs-lookup"><span data-stu-id="162a8-149">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="162a8-150">国家/地区/regioncode2 派生自 ISO 3166，它通常包括两个大写字母或 BCP 47 语言标记 (例如，EN-US)。</span><span class="sxs-lookup"><span data-stu-id="162a8-150">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="162a8-151">文件/fileData/数据</span><span class="sxs-lookup"><span data-stu-id="162a8-151">files/fileData/data</span></span>|<span data-ttu-id="162a8-152">二进制数</span><span class="sxs-lookup"><span data-stu-id="162a8-152">Binary</span></span>|<span data-ttu-id="162a8-153">代表使用条款 PDF 文档的数据。</span><span class="sxs-lookup"><span data-stu-id="162a8-153">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="162a8-154">响应</span><span class="sxs-lookup"><span data-stu-id="162a8-154">Response</span></span>
<span data-ttu-id="162a8-155">如果成功，此方法返回`201, Created`响应正文中的响应代码和[协议](../resources/agreement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="162a8-155">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="162a8-156">示例</span><span class="sxs-lookup"><span data-stu-id="162a8-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="162a8-157">请求</span><span class="sxs-lookup"><span data-stu-id="162a8-157">Request</span></span>
<span data-ttu-id="162a8-158">在请求正文中，提供[协议](../resources/agreement.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="162a8-158">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="162a8-159">响应</span><span class="sxs-lookup"><span data-stu-id="162a8-159">Response</span></span>
><span data-ttu-id="162a8-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="162a8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
