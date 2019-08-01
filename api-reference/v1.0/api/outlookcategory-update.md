---
title: 更新 Outlook 类别
description: '更新指定 outlookCategory 对象的可写属性 **color**。 不能修改**displayName**属性 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2525e7465d5b1a40ede09ef1d02c6b5045799a59
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976318"
---
# <a name="update-outlook-category"></a><span data-ttu-id="18c4f-104">更新 Outlook 类别</span><span class="sxs-lookup"><span data-stu-id="18c4f-104">Update Outlook category</span></span>


<span data-ttu-id="18c4f-105">更新指定 [outlookCategory](../resources/outlookcategory.md) 对象的可写属性 **color**。</span><span class="sxs-lookup"><span data-stu-id="18c4f-105">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="18c4f-106">创建类别后，不能修改 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="18c4f-106">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="18c4f-107">权限</span><span class="sxs-lookup"><span data-stu-id="18c4f-107">Permissions</span></span>
<span data-ttu-id="18c4f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18c4f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18c4f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="18c4f-110">Permission type</span></span>      | <span data-ttu-id="18c4f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18c4f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18c4f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18c4f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18c4f-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18c4f-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="18c4f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18c4f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18c4f-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18c4f-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="18c4f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="18c4f-116">Application</span></span> | <span data-ttu-id="18c4f-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18c4f-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="18c4f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18c4f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="18c4f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="18c4f-119">Request headers</span></span>
| <span data-ttu-id="18c4f-120">名称</span><span class="sxs-lookup"><span data-stu-id="18c4f-120">Name</span></span>      |<span data-ttu-id="18c4f-121">说明</span><span class="sxs-lookup"><span data-stu-id="18c4f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="18c4f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18c4f-122">Authorization</span></span>  | <span data-ttu-id="18c4f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18c4f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18c4f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="18c4f-125">Request body</span></span>
<span data-ttu-id="18c4f-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="18c4f-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="18c4f-129">属性</span><span class="sxs-lookup"><span data-stu-id="18c4f-129">Property</span></span>     | <span data-ttu-id="18c4f-130">类型</span><span class="sxs-lookup"><span data-stu-id="18c4f-130">Type</span></span>   |<span data-ttu-id="18c4f-131">说明</span><span class="sxs-lookup"><span data-stu-id="18c4f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18c4f-132">color</span><span class="sxs-lookup"><span data-stu-id="18c4f-132">color</span></span>|<span data-ttu-id="18c4f-133">String</span><span class="sxs-lookup"><span data-stu-id="18c4f-133">String</span></span>|<span data-ttu-id="18c4f-134">预先设定的颜色常数，它表示类别的特征，并映射到 25 种预定义颜色中的一种。</span><span class="sxs-lookup"><span data-stu-id="18c4f-134">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="18c4f-135">响应</span><span class="sxs-lookup"><span data-stu-id="18c4f-135">Response</span></span>

<span data-ttu-id="18c4f-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18c4f-136">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18c4f-137">示例</span><span class="sxs-lookup"><span data-stu-id="18c4f-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18c4f-138">请求</span><span class="sxs-lookup"><span data-stu-id="18c4f-138">Request</span></span>
<span data-ttu-id="18c4f-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18c4f-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="18c4f-140">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="18c4f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["bac262b7-485d-4739-b436-e31467d64fac"],
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="18c4f-141">C#</span><span class="sxs-lookup"><span data-stu-id="18c4f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18c4f-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="18c4f-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="18c4f-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="18c4f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="18c4f-144">Java</span><span class="sxs-lookup"><span data-stu-id="18c4f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="18c4f-145">响应</span><span class="sxs-lookup"><span data-stu-id="18c4f-145">Response</span></span>
<span data-ttu-id="18c4f-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18c4f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset15"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
