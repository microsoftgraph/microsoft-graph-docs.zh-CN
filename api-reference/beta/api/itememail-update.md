---
title: 更新 itememail
description: 更新用户的配置文件中的 itememail 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 62d7198eabebda2b7ed612c57754007130195a90
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200320"
---
# <a name="update-itememail"></a><span data-ttu-id="28be7-103">更新 itememail</span><span class="sxs-lookup"><span data-stu-id="28be7-103">Update itememail</span></span>

<span data-ttu-id="28be7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28be7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28be7-105">更新用户的[配置文件](../resources/profile.md)中的[itemEmail](../resources/itememail.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="28be7-105">Update the properties of an [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="28be7-106">权限</span><span class="sxs-lookup"><span data-stu-id="28be7-106">Permissions</span></span>

<span data-ttu-id="28be7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28be7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="28be7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="28be7-109">Permission type</span></span>                        | <span data-ttu-id="28be7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28be7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="28be7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28be7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="28be7-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="28be7-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="28be7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28be7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28be7-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="28be7-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="28be7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="28be7-115">Application</span></span>                            | <span data-ttu-id="28be7-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28be7-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="28be7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28be7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/emails/{id}
```

## <a name="request-headers"></a><span data-ttu-id="28be7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="28be7-118">Request headers</span></span>

| <span data-ttu-id="28be7-119">名称</span><span class="sxs-lookup"><span data-stu-id="28be7-119">Name</span></span>           |<span data-ttu-id="28be7-120">说明</span><span class="sxs-lookup"><span data-stu-id="28be7-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="28be7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="28be7-121">Authorization</span></span>  | <span data-ttu-id="28be7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="28be7-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="28be7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28be7-124">Content-Type</span></span>   | <span data-ttu-id="28be7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="28be7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28be7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="28be7-127">Request body</span></span>

<span data-ttu-id="28be7-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="28be7-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="28be7-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="28be7-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="28be7-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="28be7-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="28be7-131">属性</span><span class="sxs-lookup"><span data-stu-id="28be7-131">Property</span></span>     | <span data-ttu-id="28be7-132">类型</span><span class="sxs-lookup"><span data-stu-id="28be7-132">Type</span></span>        | <span data-ttu-id="28be7-133">说明</span><span class="sxs-lookup"><span data-stu-id="28be7-133">Description</span></span>                                                              |
|:-------------|:------------|:-------------------------------------------------------------------------|
|<span data-ttu-id="28be7-134">address</span><span class="sxs-lookup"><span data-stu-id="28be7-134">address</span></span>       |<span data-ttu-id="28be7-135">String</span><span class="sxs-lookup"><span data-stu-id="28be7-135">String</span></span>       | <span data-ttu-id="28be7-136">电子邮件地址本身。</span><span class="sxs-lookup"><span data-stu-id="28be7-136">The email address itself.</span></span>                                                |
|<span data-ttu-id="28be7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="28be7-137">displayName</span></span>   |<span data-ttu-id="28be7-138">字符串</span><span class="sxs-lookup"><span data-stu-id="28be7-138">String</span></span>       | <span data-ttu-id="28be7-139">用户与特定电子邮件地址相关联的名称或标签。</span><span class="sxs-lookup"><span data-stu-id="28be7-139">The name or label a user has associated with a particular email address.</span></span> |
|<span data-ttu-id="28be7-140">类型</span><span class="sxs-lookup"><span data-stu-id="28be7-140">type</span></span>          |<span data-ttu-id="28be7-141">字符串</span><span class="sxs-lookup"><span data-stu-id="28be7-141">string</span></span>       | <span data-ttu-id="28be7-142">可取值为：`unknown`、`work`、`personal`、`main`、`other`。</span><span class="sxs-lookup"><span data-stu-id="28be7-142">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>     |

## <a name="response"></a><span data-ttu-id="28be7-143">响应</span><span class="sxs-lookup"><span data-stu-id="28be7-143">Response</span></span>

<span data-ttu-id="28be7-144">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[itemEmail](../resources/itememail.md)对象。</span><span class="sxs-lookup"><span data-stu-id="28be7-144">If successful, this method returns a `200 OK` response code and an updated [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="28be7-145">示例</span><span class="sxs-lookup"><span data-stu-id="28be7-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="28be7-146">请求</span><span class="sxs-lookup"><span data-stu-id="28be7-146">Request</span></span>

<span data-ttu-id="28be7-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="28be7-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28be7-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="28be7-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itememail"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/emails/{id}
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```

# <a name="c"></a>[<span data-ttu-id="28be7-149">C#</span><span class="sxs-lookup"><span data-stu-id="28be7-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-itememail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28be7-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28be7-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-itememail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28be7-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28be7-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-itememail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="28be7-152">响应</span><span class="sxs-lookup"><span data-stu-id="28be7-152">Response</span></span>

<span data-ttu-id="28be7-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="28be7-153">The following is an example of the response.</span></span>

> <span data-ttu-id="28be7-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="28be7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update itememail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
