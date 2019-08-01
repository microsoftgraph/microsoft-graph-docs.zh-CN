---
title: 更新 mailSearchFolder
description: 更新 mailSearchFolder 对象的可写属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5760946ba7bffaf71e95e0c5481ded19d2f155b3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025462"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="04f47-103">更新 mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="04f47-103">Update mailSearchFolder</span></span>

<span data-ttu-id="04f47-104">更新[mailSearchFolder](../resources/mailsearchfolder.md)对象的可写属性。</span><span class="sxs-lookup"><span data-stu-id="04f47-104">Update the writable properties of a [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="04f47-105">权限</span><span class="sxs-lookup"><span data-stu-id="04f47-105">Permissions</span></span>
<span data-ttu-id="04f47-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04f47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04f47-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="04f47-108">Permission type</span></span>      | <span data-ttu-id="04f47-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04f47-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04f47-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04f47-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04f47-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04f47-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="04f47-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04f47-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04f47-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04f47-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="04f47-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="04f47-114">Application</span></span> | <span data-ttu-id="04f47-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04f47-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="04f47-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04f47-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="04f47-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="04f47-117">Request headers</span></span>
| <span data-ttu-id="04f47-118">标头</span><span class="sxs-lookup"><span data-stu-id="04f47-118">Header</span></span>       | <span data-ttu-id="04f47-119">值</span><span class="sxs-lookup"><span data-stu-id="04f47-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="04f47-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="04f47-120">Authorization</span></span>  | <span data-ttu-id="04f47-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="04f47-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="04f47-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04f47-123">Content-Type</span></span>  | <span data-ttu-id="04f47-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="04f47-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="04f47-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="04f47-126">Request body</span></span>
<span data-ttu-id="04f47-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="04f47-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="04f47-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="04f47-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="04f47-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="04f47-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="04f47-130">属性</span><span class="sxs-lookup"><span data-stu-id="04f47-130">Property</span></span>     | <span data-ttu-id="04f47-131">类型</span><span class="sxs-lookup"><span data-stu-id="04f47-131">Type</span></span>   |<span data-ttu-id="04f47-132">说明</span><span class="sxs-lookup"><span data-stu-id="04f47-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="04f47-133">displayName</span><span class="sxs-lookup"><span data-stu-id="04f47-133">displayName</span></span> | <span data-ttu-id="04f47-134">String</span><span class="sxs-lookup"><span data-stu-id="04f47-134">String</span></span> | <span data-ttu-id="04f47-135">[MailFolder](../resources/mailfolder.md)的显示名称。</span><span class="sxs-lookup"><span data-stu-id="04f47-135">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="04f47-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="04f47-136">includeNestedFolders</span></span> | <span data-ttu-id="04f47-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="04f47-137">Boolean</span></span> | <span data-ttu-id="04f47-138">应如何遍历邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="04f47-138">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="04f47-139">`true`表示应执行深入搜索, 而不是`false`指应改为进行浅表搜索。</span><span class="sxs-lookup"><span data-stu-id="04f47-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="04f47-140">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="04f47-140">sourceFolderIds</span></span> | <span data-ttu-id="04f47-141">String collection</span><span class="sxs-lookup"><span data-stu-id="04f47-141">String collection</span></span> | <span data-ttu-id="04f47-142">应挖掘的邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="04f47-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="04f47-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="04f47-143">filterQuery</span></span> | <span data-ttu-id="04f47-144">String</span><span class="sxs-lookup"><span data-stu-id="04f47-144">String</span></span> | <span data-ttu-id="04f47-145">用于筛选邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="04f47-145">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="04f47-146">响应</span><span class="sxs-lookup"><span data-stu-id="04f47-146">Response</span></span>
<span data-ttu-id="04f47-147">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[mailFolder](../resources/mailfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="04f47-147">If successful, this method returns a `200 OK` response code and an updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04f47-148">示例</span><span class="sxs-lookup"><span data-stu-id="04f47-148">Example</span></span>
#### <a name="request"></a><span data-ttu-id="04f47-149">请求</span><span class="sxs-lookup"><span data-stu-id="04f47-149">Request</span></span>
<span data-ttu-id="04f47-150">下面是一个更新搜索文件夹的**filterQuery**属性的示例请求。</span><span class="sxs-lookup"><span data-stu-id="04f47-150">The following is an example request that updates the **filterQuery** property of the search folder.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="04f47-151">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="04f47-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="04f47-152">C#</span><span class="sxs-lookup"><span data-stu-id="04f47-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04f47-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="04f47-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="04f47-154">目标-C</span><span class="sxs-lookup"><span data-stu-id="04f47-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="04f47-155">Java</span><span class="sxs-lookup"><span data-stu-id="04f47-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailsearchfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="04f47-156">响应</span><span class="sxs-lookup"><span data-stu-id="04f47-156">Response</span></span>
<span data-ttu-id="04f47-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="04f47-157">The following is an example of the response.</span></span>
><span data-ttu-id="04f47-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="04f47-158">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="04f47-159">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="04f47-159">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 0,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": [
      "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'Analytics')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    
  ]
}
-->
