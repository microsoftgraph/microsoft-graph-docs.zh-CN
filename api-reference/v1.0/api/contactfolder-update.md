---
title: 更新 contactfolder
description: 更新 contactfolder 对象的属性。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 851d28549c90a79c74f806b8ec882d7d0d6611c6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010099"
---
# <a name="update-contactfolder"></a><span data-ttu-id="b84f0-103">更新 contactfolder</span><span class="sxs-lookup"><span data-stu-id="b84f0-103">Update contactfolder</span></span>

<span data-ttu-id="b84f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b84f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b84f0-105">更新 contactfolder 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b84f0-105">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b84f0-106">权限</span><span class="sxs-lookup"><span data-stu-id="b84f0-106">Permissions</span></span>
<span data-ttu-id="b84f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b84f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b84f0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b84f0-109">Permission type</span></span>      | <span data-ttu-id="b84f0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b84f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b84f0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b84f0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b84f0-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b84f0-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b84f0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b84f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b84f0-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b84f0-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b84f0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b84f0-115">Application</span></span> | <span data-ttu-id="b84f0-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b84f0-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b84f0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b84f0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b84f0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b84f0-118">Request headers</span></span>
| <span data-ttu-id="b84f0-119">标头</span><span class="sxs-lookup"><span data-stu-id="b84f0-119">Header</span></span>       | <span data-ttu-id="b84f0-120">值</span><span class="sxs-lookup"><span data-stu-id="b84f0-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b84f0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b84f0-121">Authorization</span></span>  | <span data-ttu-id="b84f0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b84f0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b84f0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b84f0-124">Content-Type</span></span>  | <span data-ttu-id="b84f0-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b84f0-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b84f0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b84f0-127">Request body</span></span>
<span data-ttu-id="b84f0-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b84f0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b84f0-131">属性</span><span class="sxs-lookup"><span data-stu-id="b84f0-131">Property</span></span>     | <span data-ttu-id="b84f0-132">类型</span><span class="sxs-lookup"><span data-stu-id="b84f0-132">Type</span></span>   |<span data-ttu-id="b84f0-133">说明</span><span class="sxs-lookup"><span data-stu-id="b84f0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b84f0-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b84f0-134">displayName</span></span>|<span data-ttu-id="b84f0-135">String</span><span class="sxs-lookup"><span data-stu-id="b84f0-135">String</span></span>|<span data-ttu-id="b84f0-136">文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b84f0-136">The folder's display name.</span></span>|
|<span data-ttu-id="b84f0-137">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="b84f0-137">parentFolderId</span></span>|<span data-ttu-id="b84f0-138">String</span><span class="sxs-lookup"><span data-stu-id="b84f0-138">String</span></span>|<span data-ttu-id="b84f0-139">文件夹的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="b84f0-139">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="b84f0-140">响应</span><span class="sxs-lookup"><span data-stu-id="b84f0-140">Response</span></span>

<span data-ttu-id="b84f0-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [contactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b84f0-141">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b84f0-142">示例</span><span class="sxs-lookup"><span data-stu-id="b84f0-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b84f0-143">请求</span><span class="sxs-lookup"><span data-stu-id="b84f0-143">Request</span></span>
<span data-ttu-id="b84f0-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b84f0-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b84f0-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="b84f0-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="b84f0-146">C#</span><span class="sxs-lookup"><span data-stu-id="b84f0-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b84f0-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b84f0-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b84f0-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b84f0-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b84f0-149">Java</span><span class="sxs-lookup"><span data-stu-id="b84f0-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b84f0-150">响应</span><span class="sxs-lookup"><span data-stu-id="b84f0-150">Response</span></span>
<span data-ttu-id="b84f0-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b84f0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

