---
title: 更新 webAccount
description: 更新 webAccount 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f13a7a350bb3fa2214061c3f8bc1c08a64267223
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996133"
---
# <a name="update-webaccount"></a><span data-ttu-id="bacf7-103">更新 webAccount</span><span class="sxs-lookup"><span data-stu-id="bacf7-103">Update webAccount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bacf7-104">更新用户的[配置文件](../resources/profile.md)中的[webAccount](../resources/webaccount.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bacf7-104">Update the properties of a [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bacf7-105">权限</span><span class="sxs-lookup"><span data-stu-id="bacf7-105">Permissions</span></span>

<span data-ttu-id="bacf7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bacf7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bacf7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bacf7-108">Permission type</span></span>                        | <span data-ttu-id="bacf7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bacf7-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bacf7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bacf7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bacf7-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="bacf7-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="bacf7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bacf7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bacf7-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="bacf7-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="bacf7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bacf7-114">Application</span></span>                            | <span data-ttu-id="bacf7-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bacf7-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="bacf7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bacf7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bacf7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bacf7-117">Request headers</span></span>

| <span data-ttu-id="bacf7-118">名称</span><span class="sxs-lookup"><span data-stu-id="bacf7-118">Name</span></span>           |<span data-ttu-id="bacf7-119">说明</span><span class="sxs-lookup"><span data-stu-id="bacf7-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="bacf7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bacf7-120">Authorization</span></span>  | <span data-ttu-id="bacf7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bacf7-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="bacf7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bacf7-123">Content-Type</span></span>   | <span data-ttu-id="bacf7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bacf7-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="bacf7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bacf7-126">Request body</span></span>

<span data-ttu-id="bacf7-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="bacf7-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bacf7-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="bacf7-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bacf7-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="bacf7-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bacf7-130">属性</span><span class="sxs-lookup"><span data-stu-id="bacf7-130">Property</span></span>     | <span data-ttu-id="bacf7-131">类型</span><span class="sxs-lookup"><span data-stu-id="bacf7-131">Type</span></span>                                                    | <span data-ttu-id="bacf7-132">说明</span><span class="sxs-lookup"><span data-stu-id="bacf7-132">Description</span></span>                                                                                     |
|:-------------|:--------------------------------------------------------|:------------------------------------------------------------------------------------------------|
|<span data-ttu-id="bacf7-133">说明</span><span class="sxs-lookup"><span data-stu-id="bacf7-133">description</span></span>   |<span data-ttu-id="bacf7-134">字符串</span><span class="sxs-lookup"><span data-stu-id="bacf7-134">String</span></span>                                                   | <span data-ttu-id="bacf7-135">包含用户为所引用服务上的帐户提供的说明。</span><span class="sxs-lookup"><span data-stu-id="bacf7-135">Contains the description the user has provided for the account on the service being referenced.</span></span> |
|<span data-ttu-id="bacf7-136">service</span><span class="sxs-lookup"><span data-stu-id="bacf7-136">service</span></span>       |[<span data-ttu-id="bacf7-137">serviceInformation</span><span class="sxs-lookup"><span data-stu-id="bacf7-137">serviceInformation</span></span>](../resources/serviceinformation.md) | <span data-ttu-id="bacf7-138">表示有关用户提供的云服务的基本描述性数据。</span><span class="sxs-lookup"><span data-stu-id="bacf7-138">Represents the basic descriptive data about cloud service provided by a user.</span></span>                   |
|<span data-ttu-id="bacf7-139">statusMessage</span><span class="sxs-lookup"><span data-stu-id="bacf7-139">statusMessage</span></span> |<span data-ttu-id="bacf7-140">String</span><span class="sxs-lookup"><span data-stu-id="bacf7-140">String</span></span>                                                   | <span data-ttu-id="bacf7-141">包含来自云服务的状态邮件（如果提供或已同步）。</span><span class="sxs-lookup"><span data-stu-id="bacf7-141">Contains a status message from the cloud service if provided or synchronized.</span></span>                   |
|<span data-ttu-id="bacf7-142">userId</span><span class="sxs-lookup"><span data-stu-id="bacf7-142">userId</span></span>        |<span data-ttu-id="bacf7-143">String</span><span class="sxs-lookup"><span data-stu-id="bacf7-143">String</span></span>                                                   | <span data-ttu-id="bacf7-144">为 webaccount 显示的用户名（例如，@kevinb）。</span><span class="sxs-lookup"><span data-stu-id="bacf7-144">The user name  displayed for the webaccount (for example, @kevinb).</span></span>                                       |
|<span data-ttu-id="bacf7-145">webUrl</span><span class="sxs-lookup"><span data-stu-id="bacf7-145">webUrl</span></span>        |<span data-ttu-id="bacf7-146">String</span><span class="sxs-lookup"><span data-stu-id="bacf7-146">String</span></span>                                                   | <span data-ttu-id="bacf7-147">包含一个指向云服务上的用户配置文件的链接（如果存在）。</span><span class="sxs-lookup"><span data-stu-id="bacf7-147">Contains a link to the users profile on the cloud service if one exists.</span></span>                        |

## <a name="response"></a><span data-ttu-id="bacf7-148">响应</span><span class="sxs-lookup"><span data-stu-id="bacf7-148">Response</span></span>

<span data-ttu-id="bacf7-149">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[webAccount](../resources/webaccount.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bacf7-149">If successful, this method returns a `200 OK` response code and an updated [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bacf7-150">示例</span><span class="sxs-lookup"><span data-stu-id="bacf7-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bacf7-151">请求</span><span class="sxs-lookup"><span data-stu-id="bacf7-151">Request</span></span>

<span data-ttu-id="bacf7-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bacf7-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bacf7-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="bacf7-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_webaccount"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/webAccounts/{id}
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bacf7-154">C#</span><span class="sxs-lookup"><span data-stu-id="bacf7-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bacf7-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bacf7-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bacf7-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bacf7-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bacf7-157">响应</span><span class="sxs-lookup"><span data-stu-id="bacf7-157">Response</span></span>

<span data-ttu-id="bacf7-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bacf7-158">The following is an example of the response.</span></span>

> <span data-ttu-id="bacf7-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bacf7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update webaccount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
