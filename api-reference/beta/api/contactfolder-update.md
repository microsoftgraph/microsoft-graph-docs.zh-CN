---
title: 更新 contactfolder
description: 更新 contactfolder 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 58dfbe102e153930c603d092a74c2bc7d0a99d3c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863217"
---
# <a name="update-contactfolder"></a><span data-ttu-id="e3b83-103">更新 contactfolder</span><span class="sxs-lookup"><span data-stu-id="e3b83-103">Update contactfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3b83-104">更新 contactfolder 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e3b83-104">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e3b83-105">权限</span><span class="sxs-lookup"><span data-stu-id="e3b83-105">Permissions</span></span>
<span data-ttu-id="e3b83-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3b83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3b83-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3b83-108">Permission type</span></span>      | <span data-ttu-id="e3b83-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3b83-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3b83-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3b83-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e3b83-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3b83-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e3b83-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3b83-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3b83-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3b83-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e3b83-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3b83-114">Application</span></span> | <span data-ttu-id="e3b83-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3b83-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3b83-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3b83-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e3b83-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3b83-117">Request headers</span></span>
| <span data-ttu-id="e3b83-118">标头</span><span class="sxs-lookup"><span data-stu-id="e3b83-118">Header</span></span>       | <span data-ttu-id="e3b83-119">值</span><span class="sxs-lookup"><span data-stu-id="e3b83-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e3b83-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3b83-120">Authorization</span></span>  | <span data-ttu-id="e3b83-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3b83-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e3b83-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3b83-123">Content-Type</span></span>  | <span data-ttu-id="e3b83-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e3b83-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e3b83-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3b83-126">Request body</span></span>
<span data-ttu-id="e3b83-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e3b83-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e3b83-130">属性</span><span class="sxs-lookup"><span data-stu-id="e3b83-130">Property</span></span>     | <span data-ttu-id="e3b83-131">类型</span><span class="sxs-lookup"><span data-stu-id="e3b83-131">Type</span></span>   |<span data-ttu-id="e3b83-132">说明</span><span class="sxs-lookup"><span data-stu-id="e3b83-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3b83-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e3b83-133">displayName</span></span>|<span data-ttu-id="e3b83-134">String</span><span class="sxs-lookup"><span data-stu-id="e3b83-134">String</span></span>|<span data-ttu-id="e3b83-135">文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e3b83-135">The folder's display name.</span></span>|
|<span data-ttu-id="e3b83-136">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="e3b83-136">parentFolderId</span></span>|<span data-ttu-id="e3b83-137">String</span><span class="sxs-lookup"><span data-stu-id="e3b83-137">String</span></span>|<span data-ttu-id="e3b83-138">文件夹的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="e3b83-138">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="e3b83-139">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="e3b83-139">wellKnownName</span></span>|<span data-ttu-id="e3b83-140">string</span><span class="sxs-lookup"><span data-stu-id="e3b83-140">string</span></span>|<span data-ttu-id="e3b83-141">文件夹的名称 (如果文件夹是可识别的文件夹)。</span><span class="sxs-lookup"><span data-stu-id="e3b83-141">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="e3b83-142">当前`contacts`是唯一可识别的 "联系人" 文件夹。</span><span class="sxs-lookup"><span data-stu-id="e3b83-142">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="response"></a><span data-ttu-id="e3b83-143">响应</span><span class="sxs-lookup"><span data-stu-id="e3b83-143">Response</span></span>

<span data-ttu-id="e3b83-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [contactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e3b83-144">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3b83-145">示例</span><span class="sxs-lookup"><span data-stu-id="e3b83-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3b83-146">请求</span><span class="sxs-lookup"><span data-stu-id="e3b83-146">Request</span></span>
<span data-ttu-id="e3b83-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e3b83-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e3b83-148">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e3b83-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e3b83-149">C#</span><span class="sxs-lookup"><span data-stu-id="e3b83-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3b83-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="e3b83-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e3b83-151">目标-C</span><span class="sxs-lookup"><span data-stu-id="e3b83-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e3b83-152">Java</span><span class="sxs-lookup"><span data-stu-id="e3b83-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e3b83-153">响应</span><span class="sxs-lookup"><span data-stu-id="e3b83-153">Response</span></span>
<span data-ttu-id="e3b83-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e3b83-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "wellKnownName": "wellKnownName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
