---
title: 更新 webAccount
description: 更新 webAccount 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: bf31a230d9e77a64905bf04b2ee26215bb47375f
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229057"
---
# <a name="update-webaccount"></a><span data-ttu-id="05358-103">更新 webAccount</span><span class="sxs-lookup"><span data-stu-id="05358-103">Update webAccount</span></span>

<span data-ttu-id="05358-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05358-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05358-105">更新用户的[配置文件](../resources/profile.md)中的[webAccount](../resources/webaccount.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="05358-105">Update the properties of a [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="05358-106">权限</span><span class="sxs-lookup"><span data-stu-id="05358-106">Permissions</span></span>

<span data-ttu-id="05358-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05358-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05358-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="05358-109">Permission type</span></span>                        | <span data-ttu-id="05358-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05358-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="05358-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05358-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="05358-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="05358-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="05358-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05358-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05358-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="05358-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="05358-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="05358-115">Application</span></span>                            | <span data-ttu-id="05358-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05358-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="05358-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05358-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="05358-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="05358-118">Request headers</span></span>

| <span data-ttu-id="05358-119">名称</span><span class="sxs-lookup"><span data-stu-id="05358-119">Name</span></span>           |<span data-ttu-id="05358-120">说明</span><span class="sxs-lookup"><span data-stu-id="05358-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="05358-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="05358-121">Authorization</span></span>  | <span data-ttu-id="05358-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05358-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="05358-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05358-124">Content-Type</span></span>   | <span data-ttu-id="05358-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="05358-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="05358-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="05358-127">Request body</span></span>

<span data-ttu-id="05358-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="05358-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="05358-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="05358-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="05358-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="05358-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="05358-131">属性</span><span class="sxs-lookup"><span data-stu-id="05358-131">Property</span></span>     | <span data-ttu-id="05358-132">类型</span><span class="sxs-lookup"><span data-stu-id="05358-132">Type</span></span>                                                    | <span data-ttu-id="05358-133">说明</span><span class="sxs-lookup"><span data-stu-id="05358-133">Description</span></span>                                                                                     |
|:-------------|:--------------------------------------------------------|:------------------------------------------------------------------------------------------------|
|<span data-ttu-id="05358-134">说明</span><span class="sxs-lookup"><span data-stu-id="05358-134">description</span></span>   |<span data-ttu-id="05358-135">字符串</span><span class="sxs-lookup"><span data-stu-id="05358-135">String</span></span>                                                   | <span data-ttu-id="05358-136">包含用户为所引用服务上的帐户提供的说明。</span><span class="sxs-lookup"><span data-stu-id="05358-136">Contains the description the user has provided for the account on the service being referenced.</span></span> |
|<span data-ttu-id="05358-137">service</span><span class="sxs-lookup"><span data-stu-id="05358-137">service</span></span>       |[<span data-ttu-id="05358-138">serviceInformation</span><span class="sxs-lookup"><span data-stu-id="05358-138">serviceInformation</span></span>](../resources/serviceinformation.md) | <span data-ttu-id="05358-139">表示有关用户提供的云服务的基本描述性数据。</span><span class="sxs-lookup"><span data-stu-id="05358-139">Represents the basic descriptive data about cloud service provided by a user.</span></span>                   |
|<span data-ttu-id="05358-140">statusMessage</span><span class="sxs-lookup"><span data-stu-id="05358-140">statusMessage</span></span> |<span data-ttu-id="05358-141">String</span><span class="sxs-lookup"><span data-stu-id="05358-141">String</span></span>                                                   | <span data-ttu-id="05358-142">包含来自云服务的状态邮件（如果提供或已同步）。</span><span class="sxs-lookup"><span data-stu-id="05358-142">Contains a status message from the cloud service if provided or synchronized.</span></span>                   |
|<span data-ttu-id="05358-143">userId</span><span class="sxs-lookup"><span data-stu-id="05358-143">userId</span></span>        |<span data-ttu-id="05358-144">String</span><span class="sxs-lookup"><span data-stu-id="05358-144">String</span></span>                                                   | <span data-ttu-id="05358-145">为 webaccount 显示的用户名（例如，@kevinb）。</span><span class="sxs-lookup"><span data-stu-id="05358-145">The user name  displayed for the webaccount (for example, @kevinb).</span></span>                             |
|<span data-ttu-id="05358-146">WebUrl</span><span class="sxs-lookup"><span data-stu-id="05358-146">webUrl</span></span>        |<span data-ttu-id="05358-147">String</span><span class="sxs-lookup"><span data-stu-id="05358-147">String</span></span>                                                   | <span data-ttu-id="05358-148">包含一个指向云服务上的用户配置文件的链接（如果存在）。</span><span class="sxs-lookup"><span data-stu-id="05358-148">Contains a link to the users profile on the cloud service if one exists.</span></span>                        |

## <a name="response"></a><span data-ttu-id="05358-149">响应</span><span class="sxs-lookup"><span data-stu-id="05358-149">Response</span></span>

<span data-ttu-id="05358-150">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[webAccount](../resources/webaccount.md)对象。</span><span class="sxs-lookup"><span data-stu-id="05358-150">If successful, this method returns a `200 OK` response code and an updated [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05358-151">示例</span><span class="sxs-lookup"><span data-stu-id="05358-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="05358-152">请求</span><span class="sxs-lookup"><span data-stu-id="05358-152">Request</span></span>

<span data-ttu-id="05358-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="05358-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="05358-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="05358-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="05358-155">C#</span><span class="sxs-lookup"><span data-stu-id="05358-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05358-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05358-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05358-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05358-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="05358-158">响应</span><span class="sxs-lookup"><span data-stu-id="05358-158">Response</span></span>

<span data-ttu-id="05358-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="05358-159">The following is an example of the response.</span></span>

> <span data-ttu-id="05358-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="05358-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
