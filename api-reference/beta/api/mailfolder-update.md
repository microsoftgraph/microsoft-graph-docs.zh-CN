---
title: 更新 mailFolder
description: 更新 mailFolder 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6517386c4c21df35ae8df843de5734142a249f68
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347085"
---
# <a name="update-mailfolder"></a><span data-ttu-id="18b23-103">更新 mailFolder</span><span class="sxs-lookup"><span data-stu-id="18b23-103">Update mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18b23-104">更新[mailFolder](../resources/mailfolder.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="18b23-104">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="18b23-105">权限</span><span class="sxs-lookup"><span data-stu-id="18b23-105">Permissions</span></span>
<span data-ttu-id="18b23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18b23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18b23-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="18b23-108">Permission type</span></span>      | <span data-ttu-id="18b23-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18b23-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18b23-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18b23-110">Delegated (work or school account)</span></span> | <span data-ttu-id="18b23-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18b23-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="18b23-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18b23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18b23-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18b23-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="18b23-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="18b23-114">Application</span></span> | <span data-ttu-id="18b23-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18b23-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="18b23-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18b23-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="18b23-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="18b23-117">Request headers</span></span>
| <span data-ttu-id="18b23-118">标头</span><span class="sxs-lookup"><span data-stu-id="18b23-118">Header</span></span>       | <span data-ttu-id="18b23-119">值</span><span class="sxs-lookup"><span data-stu-id="18b23-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18b23-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="18b23-120">Authorization</span></span>  | <span data-ttu-id="18b23-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18b23-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="18b23-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18b23-123">Content-Type</span></span>  | <span data-ttu-id="18b23-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="18b23-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18b23-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="18b23-126">Request body</span></span>
<span data-ttu-id="18b23-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="18b23-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="18b23-130">属性</span><span class="sxs-lookup"><span data-stu-id="18b23-130">Property</span></span>     | <span data-ttu-id="18b23-131">类型</span><span class="sxs-lookup"><span data-stu-id="18b23-131">Type</span></span>   |<span data-ttu-id="18b23-132">说明</span><span class="sxs-lookup"><span data-stu-id="18b23-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18b23-133">displayName</span><span class="sxs-lookup"><span data-stu-id="18b23-133">displayName</span></span>|<span data-ttu-id="18b23-134">String</span><span class="sxs-lookup"><span data-stu-id="18b23-134">String</span></span>|<span data-ttu-id="18b23-135">mailFolder 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="18b23-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="18b23-136">响应</span><span class="sxs-lookup"><span data-stu-id="18b23-136">Response</span></span>
<span data-ttu-id="18b23-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [mailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18b23-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18b23-138">示例</span><span class="sxs-lookup"><span data-stu-id="18b23-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="18b23-139">请求</span><span class="sxs-lookup"><span data-stu-id="18b23-139">Request</span></span>
<span data-ttu-id="18b23-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="18b23-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="18b23-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="18b23-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="18b23-142">C#</span><span class="sxs-lookup"><span data-stu-id="18b23-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18b23-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18b23-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="18b23-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="18b23-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="18b23-145">Java</span><span class="sxs-lookup"><span data-stu-id="18b23-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="18b23-146">响应</span><span class="sxs-lookup"><span data-stu-id="18b23-146">Response</span></span>
<span data-ttu-id="18b23-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="18b23-147">The following is an example of the response.</span></span>
><span data-ttu-id="18b23-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="18b23-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="18b23-149">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="18b23-149">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "displayName-value",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
