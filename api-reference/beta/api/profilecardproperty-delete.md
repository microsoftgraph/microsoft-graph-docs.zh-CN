---
title: 删除 profileCardProperty
description: 删除 profileCardProperty 对象并删除配置文件卡片中的所有自定义项。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 853f7abcb80d83c6aebbaf9dc773165a1263a331
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088069"
---
# <a name="delete-profilecardproperty"></a><span data-ttu-id="d5258-103">删除 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="d5258-103">Delete profileCardProperty</span></span>

<span data-ttu-id="d5258-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5258-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5258-105">从组织的配置文件卡片中删除由其指定的 [profileCardProperty](../resources/profilecardproperty.md) 对象 `directoryPropertyName` ，并删除该属性的所有本地化的自定义项。</span><span class="sxs-lookup"><span data-stu-id="d5258-105">Delete the [profileCardProperty](../resources/profilecardproperty.md) object specified by its `directoryPropertyName` from the organization's profile card, and remove any localized customizations for that property.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5258-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d5258-106">Permissions</span></span>

<span data-ttu-id="d5258-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5258-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5258-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5258-109">Permission type</span></span>                        | <span data-ttu-id="d5258-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5258-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d5258-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5258-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5258-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="d5258-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d5258-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5258-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5258-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5258-114">Not supported.</span></span>                              |
| <span data-ttu-id="d5258-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5258-115">Application</span></span>                            | <span data-ttu-id="d5258-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5258-116">Not supported.</span></span>                              |

><span data-ttu-id="d5258-117">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="d5258-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="d5258-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5258-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{directoryPropertyName-Value}
```

## <a name="request-headers"></a><span data-ttu-id="d5258-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5258-119">Request headers</span></span>

| <span data-ttu-id="d5258-120">名称</span><span class="sxs-lookup"><span data-stu-id="d5258-120">Name</span></span>          | <span data-ttu-id="d5258-121">说明</span><span class="sxs-lookup"><span data-stu-id="d5258-121">Description</span></span>    |
|:--------------|:---------------|
| <span data-ttu-id="d5258-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5258-122">Authorization</span></span> | <span data-ttu-id="d5258-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5258-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5258-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5258-125">Request body</span></span>

<span data-ttu-id="d5258-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5258-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5258-127">响应</span><span class="sxs-lookup"><span data-stu-id="d5258-127">Response</span></span>

<span data-ttu-id="d5258-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d5258-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d5258-130">示例</span><span class="sxs-lookup"><span data-stu-id="d5258-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5258-131">请求</span><span class="sxs-lookup"><span data-stu-id="d5258-131">Request</span></span>

<span data-ttu-id="d5258-132">下面的示例演示如何从组织的配置文件卡片中删除名为 "Fax" 的属性。</span><span class="sxs-lookup"><span data-stu-id="d5258-132">The following example shows how to delete the attribute named "Fax" from the profile card for the organization.</span></span>

# <a name="http"></a>[<span data-ttu-id="d5258-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5258-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_profilecardproperty"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/fax
```
# <a name="c"></a>[<span data-ttu-id="d5258-134">C#</span><span class="sxs-lookup"><span data-stu-id="d5258-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-profilecardproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5258-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5258-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5258-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5258-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-profilecardproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d5258-137">响应</span><span class="sxs-lookup"><span data-stu-id="d5258-137">Response</span></span>

<span data-ttu-id="d5258-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d5258-138">The following is an example of the response.</span></span>

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


