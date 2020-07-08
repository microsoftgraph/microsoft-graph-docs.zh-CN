---
title: 删除 profileCardProperty
description: 删除 profileCardProperty 对象并删除配置文件卡片中的所有自定义项。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2dffcc667281d26fb64e44dd7cd45e8e0f1c313f
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080688"
---
# <a name="delete-profilecardproperty"></a><span data-ttu-id="6233c-103">删除 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="6233c-103">Delete profileCardProperty</span></span>

<span data-ttu-id="6233c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6233c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6233c-105">从组织的配置文件卡片中删除由其指定的[profileCardProperty](../resources/profilecardproperty.md)对象 `directoryPropertyName` ，并删除该属性的所有本地化的自定义项。</span><span class="sxs-lookup"><span data-stu-id="6233c-105">Delete the [profileCardProperty](../resources/profilecardproperty.md) object specified by its `directoryPropertyName` from the organization's profile card, and remove any localized customizations for that property.</span></span>

## <a name="permissions"></a><span data-ttu-id="6233c-106">权限</span><span class="sxs-lookup"><span data-stu-id="6233c-106">Permissions</span></span>

<span data-ttu-id="6233c-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6233c-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6233c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6233c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6233c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6233c-109">Permission type</span></span>                        | <span data-ttu-id="6233c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6233c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6233c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6233c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6233c-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="6233c-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6233c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6233c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6233c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6233c-114">Not supported.</span></span>                              |
| <span data-ttu-id="6233c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6233c-115">Application</span></span>                            | <span data-ttu-id="6233c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6233c-116">Not supported.</span></span>                              |

><span data-ttu-id="6233c-117">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="6233c-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="6233c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6233c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/organization/settings/profileCardProperties/{directoryPropertyName-Value}
```

## <a name="request-headers"></a><span data-ttu-id="6233c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6233c-119">Request headers</span></span>

| <span data-ttu-id="6233c-120">名称</span><span class="sxs-lookup"><span data-stu-id="6233c-120">Name</span></span>          | <span data-ttu-id="6233c-121">说明</span><span class="sxs-lookup"><span data-stu-id="6233c-121">Description</span></span>    |
|:--------------|:---------------|
| <span data-ttu-id="6233c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6233c-122">Authorization</span></span> | <span data-ttu-id="6233c-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="6233c-123">Bearer {token}.</span></span> <span data-ttu-id="6233c-124">Required.</span><span class="sxs-lookup"><span data-stu-id="6233c-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6233c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6233c-125">Request body</span></span>

<span data-ttu-id="6233c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6233c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6233c-127">响应</span><span class="sxs-lookup"><span data-stu-id="6233c-127">Response</span></span>

<span data-ttu-id="6233c-128">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="6233c-128">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="6233c-129">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="6233c-129">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6233c-130">示例</span><span class="sxs-lookup"><span data-stu-id="6233c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6233c-131">请求</span><span class="sxs-lookup"><span data-stu-id="6233c-131">Request</span></span>

<span data-ttu-id="6233c-132">下面的示例演示如何从组织的配置文件卡片中删除名为 "Fax" 的属性。</span><span class="sxs-lookup"><span data-stu-id="6233c-132">The following example shows how to delete the attribute named "Fax" from the profile card for the organization.</span></span>

# <a name="http"></a>[<span data-ttu-id="6233c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6233c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_profilecardproperty"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/settings/profileCardProperties/fax
```
# <a name="c"></a>[<span data-ttu-id="6233c-134">C#</span><span class="sxs-lookup"><span data-stu-id="6233c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-profilecardproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6233c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6233c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6233c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6233c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-profilecardproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6233c-137">响应</span><span class="sxs-lookup"><span data-stu-id="6233c-137">Response</span></span>

<span data-ttu-id="6233c-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6233c-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
