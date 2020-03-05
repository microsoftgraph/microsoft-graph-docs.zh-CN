---
title: 更新 personInterest
description: 更新 personinterest 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 36d83b710e19c1bcfc92ebae4c61efd2c6fb434b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455905"
---
# <a name="update-personinterest"></a><span data-ttu-id="13f3c-103">更新 personinterest</span><span class="sxs-lookup"><span data-stu-id="13f3c-103">Update personinterest</span></span>

<span data-ttu-id="13f3c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="13f3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13f3c-105">更新用户的[配置文件](../resources/profile.md)中的[personInterest](../resources/personinterest.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="13f3c-105">Update the properties of a [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="13f3c-106">权限</span><span class="sxs-lookup"><span data-stu-id="13f3c-106">Permissions</span></span>

<span data-ttu-id="13f3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13f3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="13f3c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="13f3c-109">Permission type</span></span>                        | <span data-ttu-id="13f3c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13f3c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="13f3c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13f3c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="13f3c-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="13f3c-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="13f3c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13f3c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13f3c-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="13f3c-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="13f3c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="13f3c-115">Application</span></span>                            | <span data-ttu-id="13f3c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13f3c-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="13f3c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13f3c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="13f3c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="13f3c-118">Request headers</span></span>

| <span data-ttu-id="13f3c-119">名称</span><span class="sxs-lookup"><span data-stu-id="13f3c-119">Name</span></span>           |<span data-ttu-id="13f3c-120">说明</span><span class="sxs-lookup"><span data-stu-id="13f3c-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="13f3c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="13f3c-121">Authorization</span></span>  | <span data-ttu-id="13f3c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="13f3c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="13f3c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="13f3c-124">Content-Type</span></span>   | <span data-ttu-id="13f3c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="13f3c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13f3c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="13f3c-127">Request body</span></span>

<span data-ttu-id="13f3c-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="13f3c-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="13f3c-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="13f3c-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="13f3c-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="13f3c-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="13f3c-131">属性</span><span class="sxs-lookup"><span data-stu-id="13f3c-131">Property</span></span>     | <span data-ttu-id="13f3c-132">类型</span><span class="sxs-lookup"><span data-stu-id="13f3c-132">Type</span></span>             | <span data-ttu-id="13f3c-133">说明</span><span class="sxs-lookup"><span data-stu-id="13f3c-133">Description</span></span>                                                                         |
|:-------------|:-----------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="13f3c-134">categories</span><span class="sxs-lookup"><span data-stu-id="13f3c-134">categories</span></span>    |<span data-ttu-id="13f3c-135">String 集合</span><span class="sxs-lookup"><span data-stu-id="13f3c-135">String collection</span></span> | <span data-ttu-id="13f3c-136">包含用户与兴趣相关联的类别（例如： personal、recipies）</span><span class="sxs-lookup"><span data-stu-id="13f3c-136">Contains categories a user has associated with the interest (eg: personal, recipies)</span></span>|
|<span data-ttu-id="13f3c-137">说明</span><span class="sxs-lookup"><span data-stu-id="13f3c-137">description</span></span>   |<span data-ttu-id="13f3c-138">字符串</span><span class="sxs-lookup"><span data-stu-id="13f3c-138">String</span></span>            | <span data-ttu-id="13f3c-139">包含对利息的说明。</span><span class="sxs-lookup"><span data-stu-id="13f3c-139">Contains a description of the interest.</span></span>                                             |
|<span data-ttu-id="13f3c-140">displayName</span><span class="sxs-lookup"><span data-stu-id="13f3c-140">displayName</span></span>   |<span data-ttu-id="13f3c-141">String</span><span class="sxs-lookup"><span data-stu-id="13f3c-141">String</span></span>            | <span data-ttu-id="13f3c-142">包含利息的友好名称。</span><span class="sxs-lookup"><span data-stu-id="13f3c-142">Contains a friendly name for the interest.</span></span>                                          |
|<span data-ttu-id="13f3c-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="13f3c-143">webUrl</span></span>        |<span data-ttu-id="13f3c-144">String</span><span class="sxs-lookup"><span data-stu-id="13f3c-144">String</span></span>            | <span data-ttu-id="13f3c-145">包含指向有关该兴趣的信息源的链接。</span><span class="sxs-lookup"><span data-stu-id="13f3c-145">Contains a link to an information source about the interest.</span></span>                        |

## <a name="response"></a><span data-ttu-id="13f3c-146">响应</span><span class="sxs-lookup"><span data-stu-id="13f3c-146">Response</span></span>

<span data-ttu-id="13f3c-147">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[personInterest](../resources/personinterest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="13f3c-147">If successful, this method returns a `200 OK` response code and an updated [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13f3c-148">示例</span><span class="sxs-lookup"><span data-stu-id="13f3c-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="13f3c-149">请求</span><span class="sxs-lookup"><span data-stu-id="13f3c-149">Request</span></span>

<span data-ttu-id="13f3c-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="13f3c-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="13f3c-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="13f3c-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personinterest"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/interests/{id}
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```
# <a name="c"></a>[<span data-ttu-id="13f3c-152">C#</span><span class="sxs-lookup"><span data-stu-id="13f3c-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13f3c-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13f3c-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13f3c-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13f3c-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="13f3c-155">响应</span><span class="sxs-lookup"><span data-stu-id="13f3c-155">Response</span></span>

<span data-ttu-id="13f3c-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="13f3c-156">The following is an example of the response.</span></span>

> <span data-ttu-id="13f3c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="13f3c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update personinterest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
