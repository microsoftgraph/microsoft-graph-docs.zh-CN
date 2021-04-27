---
title: 更新 Outlook 类别
description: '更新指定 outlookCategory 对象的可写属性 **color**。 不能修改 **displayName** 属性 '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f570c805f93ad7be8b05dd2dc6ccdefe654128fd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055496"
---
# <a name="update-outlook-category"></a><span data-ttu-id="17609-104">更新 Outlook 类别</span><span class="sxs-lookup"><span data-stu-id="17609-104">Update Outlook category</span></span>

<span data-ttu-id="17609-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17609-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17609-106">更新指定 [outlookCategory](../resources/outlookcategory.md) 对象的可写属性 **color**。</span><span class="sxs-lookup"><span data-stu-id="17609-106">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="17609-107">创建类别后，不能修改 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="17609-107">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="17609-108">权限</span><span class="sxs-lookup"><span data-stu-id="17609-108">Permissions</span></span>
<span data-ttu-id="17609-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17609-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17609-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="17609-111">Permission type</span></span>      | <span data-ttu-id="17609-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17609-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17609-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17609-113">Delegated (work or school account)</span></span> | <span data-ttu-id="17609-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17609-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="17609-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17609-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17609-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17609-116">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="17609-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="17609-117">Application</span></span> | <span data-ttu-id="17609-118">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17609-118">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="17609-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17609-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="17609-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="17609-120">Request headers</span></span>
| <span data-ttu-id="17609-121">名称</span><span class="sxs-lookup"><span data-stu-id="17609-121">Name</span></span>      |<span data-ttu-id="17609-122">说明</span><span class="sxs-lookup"><span data-stu-id="17609-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="17609-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="17609-123">Authorization</span></span>  | <span data-ttu-id="17609-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17609-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17609-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="17609-126">Request body</span></span>
<span data-ttu-id="17609-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="17609-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="17609-130">属性</span><span class="sxs-lookup"><span data-stu-id="17609-130">Property</span></span>     | <span data-ttu-id="17609-131">类型</span><span class="sxs-lookup"><span data-stu-id="17609-131">Type</span></span>   |<span data-ttu-id="17609-132">说明</span><span class="sxs-lookup"><span data-stu-id="17609-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17609-133">color</span><span class="sxs-lookup"><span data-stu-id="17609-133">color</span></span>|<span data-ttu-id="17609-134">String</span><span class="sxs-lookup"><span data-stu-id="17609-134">String</span></span>|<span data-ttu-id="17609-135">预先设定的颜色常数，它表示类别的特征，并映射到 25 种预定义颜色中的一种。</span><span class="sxs-lookup"><span data-stu-id="17609-135">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="17609-136">响应</span><span class="sxs-lookup"><span data-stu-id="17609-136">Response</span></span>

<span data-ttu-id="17609-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="17609-137">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="17609-138">示例</span><span class="sxs-lookup"><span data-stu-id="17609-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17609-139">请求</span><span class="sxs-lookup"><span data-stu-id="17609-139">Request</span></span>
<span data-ttu-id="17609-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17609-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="17609-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="17609-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
# <a name="c"></a>[<span data-ttu-id="17609-142">C#</span><span class="sxs-lookup"><span data-stu-id="17609-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17609-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17609-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17609-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17609-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17609-145">Java</span><span class="sxs-lookup"><span data-stu-id="17609-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="17609-146">响应</span><span class="sxs-lookup"><span data-stu-id="17609-146">Response</span></span>
<span data-ttu-id="17609-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="17609-147">Here is an example of the response.</span></span> <span data-ttu-id="17609-148">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="17609-148">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset15"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


