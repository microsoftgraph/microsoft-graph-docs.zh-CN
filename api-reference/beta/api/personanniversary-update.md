---
title: 更新 personAnniversary
description: 更新 personanniversary 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fd3ba313d992f2904ac57a1d650af6245a337b3d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455926"
---
# <a name="update-personanniversary"></a><span data-ttu-id="227cd-103">更新 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="227cd-103">Update personAnniversary</span></span>

<span data-ttu-id="227cd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="227cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="227cd-105">更新用户的[配置文件](../resources/profile.md)中的[personAnniversary](../resources/personanniversary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="227cd-105">Update the properties of a [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="227cd-106">权限</span><span class="sxs-lookup"><span data-stu-id="227cd-106">Permissions</span></span>

<span data-ttu-id="227cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="227cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="227cd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="227cd-109">Permission type</span></span>                        | <span data-ttu-id="227cd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="227cd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="227cd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="227cd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="227cd-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="227cd-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="227cd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="227cd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="227cd-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="227cd-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="227cd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="227cd-115">Application</span></span>                            | <span data-ttu-id="227cd-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227cd-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="227cd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="227cd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/anniversaries/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="227cd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="227cd-118">Request headers</span></span>

| <span data-ttu-id="227cd-119">名称</span><span class="sxs-lookup"><span data-stu-id="227cd-119">Name</span></span>           |<span data-ttu-id="227cd-120">说明</span><span class="sxs-lookup"><span data-stu-id="227cd-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="227cd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="227cd-121">Authorization</span></span>  | <span data-ttu-id="227cd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="227cd-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="227cd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="227cd-124">Content-Type</span></span>   | <span data-ttu-id="227cd-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="227cd-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="227cd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="227cd-127">Request body</span></span>

<span data-ttu-id="227cd-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="227cd-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="227cd-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="227cd-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="227cd-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="227cd-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="227cd-131">属性</span><span class="sxs-lookup"><span data-stu-id="227cd-131">Property</span></span>     | <span data-ttu-id="227cd-132">类型</span><span class="sxs-lookup"><span data-stu-id="227cd-132">Type</span></span>        | <span data-ttu-id="227cd-133">说明</span><span class="sxs-lookup"><span data-stu-id="227cd-133">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="227cd-134">date</span><span class="sxs-lookup"><span data-stu-id="227cd-134">date</span></span>          |<span data-ttu-id="227cd-135">Date</span><span class="sxs-lookup"><span data-stu-id="227cd-135">Date</span></span>         | <span data-ttu-id="227cd-136">包含与周年纪念类型相关联的日期。</span><span class="sxs-lookup"><span data-stu-id="227cd-136">Contains the date associated with the anniversary type.</span></span>          |
|<span data-ttu-id="227cd-137">类型</span><span class="sxs-lookup"><span data-stu-id="227cd-137">type</span></span>          |<span data-ttu-id="227cd-138">string</span><span class="sxs-lookup"><span data-stu-id="227cd-138">string</span></span>       | <span data-ttu-id="227cd-139">可取值为：`birthday`、`wedding`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="227cd-139">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="227cd-140">响应</span><span class="sxs-lookup"><span data-stu-id="227cd-140">Response</span></span>

<span data-ttu-id="227cd-141">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[personAnniversary](../resources/personanniversary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="227cd-141">If successful, this method returns a `200 OK` response code and an updated [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="227cd-142">示例</span><span class="sxs-lookup"><span data-stu-id="227cd-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="227cd-143">请求</span><span class="sxs-lookup"><span data-stu-id="227cd-143">Request</span></span>

<span data-ttu-id="227cd-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="227cd-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="227cd-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="227cd-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="227cd-146">C#</span><span class="sxs-lookup"><span data-stu-id="227cd-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="227cd-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="227cd-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="227cd-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="227cd-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="227cd-149">响应</span><span class="sxs-lookup"><span data-stu-id="227cd-149">Response</span></span>

<span data-ttu-id="227cd-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="227cd-150">The following is an example of the response.</span></span>

> <span data-ttu-id="227cd-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="227cd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
