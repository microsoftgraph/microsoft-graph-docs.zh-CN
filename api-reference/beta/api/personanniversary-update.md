---
title: 更新 personAnniversary
description: 更新 personanniversary 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 938d0ef37b26221b5cdec958cff1a1bb53576ab5
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997268"
---
# <a name="update-personanniversary"></a><span data-ttu-id="c5ef9-103">更新 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="c5ef9-103">Update personAnniversary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5ef9-104">更新用户的[配置文件](../resources/profile.md)中的[personAnniversary](../resources/personanniversary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c5ef9-104">Update the properties of a [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5ef9-105">权限</span><span class="sxs-lookup"><span data-stu-id="c5ef9-105">Permissions</span></span>

<span data-ttu-id="c5ef9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5ef9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5ef9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5ef9-108">Permission type</span></span>                        | <span data-ttu-id="c5ef9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5ef9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c5ef9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5ef9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5ef9-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="c5ef9-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="c5ef9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5ef9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5ef9-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="c5ef9-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="c5ef9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5ef9-114">Application</span></span>                            | <span data-ttu-id="c5ef9-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5ef9-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="c5ef9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5ef9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/anniversaries/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="c5ef9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5ef9-117">Request headers</span></span>

| <span data-ttu-id="c5ef9-118">名称</span><span class="sxs-lookup"><span data-stu-id="c5ef9-118">Name</span></span>           |<span data-ttu-id="c5ef9-119">说明</span><span class="sxs-lookup"><span data-stu-id="c5ef9-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="c5ef9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5ef9-120">Authorization</span></span>  | <span data-ttu-id="c5ef9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5ef9-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="c5ef9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5ef9-123">Content-Type</span></span>   | <span data-ttu-id="c5ef9-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c5ef9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5ef9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5ef9-126">Request body</span></span>

<span data-ttu-id="c5ef9-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="c5ef9-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c5ef9-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="c5ef9-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c5ef9-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c5ef9-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c5ef9-130">属性</span><span class="sxs-lookup"><span data-stu-id="c5ef9-130">Property</span></span>     | <span data-ttu-id="c5ef9-131">类型</span><span class="sxs-lookup"><span data-stu-id="c5ef9-131">Type</span></span>        | <span data-ttu-id="c5ef9-132">说明</span><span class="sxs-lookup"><span data-stu-id="c5ef9-132">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="c5ef9-133">date</span><span class="sxs-lookup"><span data-stu-id="c5ef9-133">date</span></span>          |<span data-ttu-id="c5ef9-134">Date</span><span class="sxs-lookup"><span data-stu-id="c5ef9-134">Date</span></span>         | <span data-ttu-id="c5ef9-135">包含与周年纪念类型相关联的日期。</span><span class="sxs-lookup"><span data-stu-id="c5ef9-135">Contains the date associated with the anniversary type.</span></span>          |
|<span data-ttu-id="c5ef9-136">类型</span><span class="sxs-lookup"><span data-stu-id="c5ef9-136">type</span></span>          |<span data-ttu-id="c5ef9-137">string</span><span class="sxs-lookup"><span data-stu-id="c5ef9-137">string</span></span>       | <span data-ttu-id="c5ef9-138">可取值为：`birthday`、`wedding`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c5ef9-138">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="c5ef9-139">响应</span><span class="sxs-lookup"><span data-stu-id="c5ef9-139">Response</span></span>

<span data-ttu-id="c5ef9-140">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[personAnniversary](../resources/personanniversary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c5ef9-140">If successful, this method returns a `200 OK` response code and an updated [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c5ef9-141">示例</span><span class="sxs-lookup"><span data-stu-id="c5ef9-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5ef9-142">请求</span><span class="sxs-lookup"><span data-stu-id="c5ef9-142">Request</span></span>

<span data-ttu-id="c5ef9-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c5ef9-143">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c5ef9-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5ef9-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personanniversary"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c5ef9-145">C#</span><span class="sxs-lookup"><span data-stu-id="c5ef9-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5ef9-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5ef9-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c5ef9-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5ef9-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c5ef9-148">响应</span><span class="sxs-lookup"><span data-stu-id="c5ef9-148">Response</span></span>

<span data-ttu-id="c5ef9-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c5ef9-149">The following is an example of the response.</span></span>

> <span data-ttu-id="c5ef9-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c5ef9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update personanniversary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
