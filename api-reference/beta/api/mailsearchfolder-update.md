---
title: 更新 mailSearchFolder
description: 更新 mailSearchFolder 对象的可写属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 08a4ad5a7a846689e70f2da4bdd50f8d16218f85
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456990"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="c038a-103">更新 mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="c038a-103">Update mailSearchFolder</span></span>

<span data-ttu-id="c038a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c038a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c038a-105">更新[mailSearchFolder](../resources/mailsearchfolder.md)对象的可写属性。</span><span class="sxs-lookup"><span data-stu-id="c038a-105">Update the writable properties of a [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c038a-106">权限</span><span class="sxs-lookup"><span data-stu-id="c038a-106">Permissions</span></span>
<span data-ttu-id="c038a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c038a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c038a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c038a-109">Permission type</span></span>      | <span data-ttu-id="c038a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c038a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c038a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c038a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c038a-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c038a-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c038a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c038a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c038a-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c038a-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c038a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c038a-115">Application</span></span> | <span data-ttu-id="c038a-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c038a-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c038a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c038a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c038a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c038a-118">Request headers</span></span>
| <span data-ttu-id="c038a-119">标头</span><span class="sxs-lookup"><span data-stu-id="c038a-119">Header</span></span>       | <span data-ttu-id="c038a-120">值</span><span class="sxs-lookup"><span data-stu-id="c038a-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c038a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c038a-121">Authorization</span></span>  | <span data-ttu-id="c038a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c038a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c038a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c038a-124">Content-Type</span></span>  | <span data-ttu-id="c038a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c038a-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c038a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c038a-127">Request body</span></span>
<span data-ttu-id="c038a-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="c038a-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c038a-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="c038a-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c038a-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c038a-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c038a-131">属性</span><span class="sxs-lookup"><span data-stu-id="c038a-131">Property</span></span>     | <span data-ttu-id="c038a-132">类型</span><span class="sxs-lookup"><span data-stu-id="c038a-132">Type</span></span>   |<span data-ttu-id="c038a-133">说明</span><span class="sxs-lookup"><span data-stu-id="c038a-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c038a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c038a-134">displayName</span></span> | <span data-ttu-id="c038a-135">String</span><span class="sxs-lookup"><span data-stu-id="c038a-135">String</span></span> | <span data-ttu-id="c038a-136">[MailFolder](../resources/mailfolder.md)的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c038a-136">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="c038a-137">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="c038a-137">includeNestedFolders</span></span> | <span data-ttu-id="c038a-138">布尔</span><span class="sxs-lookup"><span data-stu-id="c038a-138">Boolean</span></span> | <span data-ttu-id="c038a-139">应如何遍历邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="c038a-139">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="c038a-140">`true`表示应执行深入搜索，而不是`false`指应改为进行浅表搜索。</span><span class="sxs-lookup"><span data-stu-id="c038a-140">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="c038a-141">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="c038a-141">sourceFolderIds</span></span> | <span data-ttu-id="c038a-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="c038a-142">String collection</span></span> | <span data-ttu-id="c038a-143">应挖掘的邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="c038a-143">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="c038a-144">filterQuery</span><span class="sxs-lookup"><span data-stu-id="c038a-144">filterQuery</span></span> | <span data-ttu-id="c038a-145">String</span><span class="sxs-lookup"><span data-stu-id="c038a-145">String</span></span> | <span data-ttu-id="c038a-146">用于筛选邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="c038a-146">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="c038a-147">响应</span><span class="sxs-lookup"><span data-stu-id="c038a-147">Response</span></span>
<span data-ttu-id="c038a-148">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[mailFolder](../resources/mailfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c038a-148">If successful, this method returns a `200 OK` response code and an updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c038a-149">示例</span><span class="sxs-lookup"><span data-stu-id="c038a-149">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c038a-150">请求</span><span class="sxs-lookup"><span data-stu-id="c038a-150">Request</span></span>
<span data-ttu-id="c038a-151">下面是一个更新搜索文件夹的**filterQuery**属性的示例请求。</span><span class="sxs-lookup"><span data-stu-id="c038a-151">The following is an example request that updates the **filterQuery** property of the search folder.</span></span>

# <a name="http"></a>[<span data-ttu-id="c038a-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="c038a-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')"
}
```
# <a name="c"></a>[<span data-ttu-id="c038a-153">C#</span><span class="sxs-lookup"><span data-stu-id="c038a-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c038a-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c038a-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c038a-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c038a-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c038a-156">响应</span><span class="sxs-lookup"><span data-stu-id="c038a-156">Response</span></span>
<span data-ttu-id="c038a-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c038a-157">The following is an example of the response.</span></span>
><span data-ttu-id="c038a-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c038a-158">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c038a-159">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c038a-159">All the properties will be returned from an actual call.</span></span>
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
