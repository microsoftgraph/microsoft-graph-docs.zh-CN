---
title: 更新 mailSearchFolder
description: 更新 mailSearchFolder 对象的可写属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: dac2bbb95da7d287ce00503ac4b79cdf52a85968
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536020"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="edf36-103">更新 mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="edf36-103">Update mailSearchFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edf36-104">更新[mailSearchFolder](../resources/mailsearchfolder.md)对象的可写属性。</span><span class="sxs-lookup"><span data-stu-id="edf36-104">Update the writable properties of [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="edf36-105">权限</span><span class="sxs-lookup"><span data-stu-id="edf36-105">Permissions</span></span>
<span data-ttu-id="edf36-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="edf36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edf36-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="edf36-108">Permission type</span></span>      | <span data-ttu-id="edf36-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="edf36-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edf36-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="edf36-110">Delegated (work or school account)</span></span> | <span data-ttu-id="edf36-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="edf36-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="edf36-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="edf36-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edf36-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="edf36-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="edf36-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="edf36-114">Application</span></span> | <span data-ttu-id="edf36-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="edf36-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="edf36-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edf36-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="edf36-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="edf36-117">Request headers</span></span>
| <span data-ttu-id="edf36-118">标头</span><span class="sxs-lookup"><span data-stu-id="edf36-118">Header</span></span>       | <span data-ttu-id="edf36-119">值</span><span class="sxs-lookup"><span data-stu-id="edf36-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="edf36-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="edf36-120">Authorization</span></span>  | <span data-ttu-id="edf36-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="edf36-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="edf36-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="edf36-123">Content-Type</span></span>  | <span data-ttu-id="edf36-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="edf36-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="edf36-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="edf36-126">Request body</span></span>
<span data-ttu-id="edf36-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="edf36-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="edf36-130">属性</span><span class="sxs-lookup"><span data-stu-id="edf36-130">Property</span></span>     | <span data-ttu-id="edf36-131">类型</span><span class="sxs-lookup"><span data-stu-id="edf36-131">Type</span></span>   |<span data-ttu-id="edf36-132">说明</span><span class="sxs-lookup"><span data-stu-id="edf36-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="edf36-133">displayName</span><span class="sxs-lookup"><span data-stu-id="edf36-133">displayName</span></span> | <span data-ttu-id="edf36-134">String</span><span class="sxs-lookup"><span data-stu-id="edf36-134">String</span></span> | <span data-ttu-id="edf36-135">[MailFolder](../resources/mailfolder.md)的显示名称。</span><span class="sxs-lookup"><span data-stu-id="edf36-135">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="edf36-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="edf36-136">includeNestedFolders</span></span> | <span data-ttu-id="edf36-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="edf36-137">Boolean</span></span> | <span data-ttu-id="edf36-138">应如何遍历邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="edf36-138">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="edf36-139">`true`表示应执行深入搜索, 而不是`false`指应改为进行浅表搜索。</span><span class="sxs-lookup"><span data-stu-id="edf36-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="edf36-140">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="edf36-140">sourceFolderIDs</span></span> | <span data-ttu-id="edf36-141">String collection</span><span class="sxs-lookup"><span data-stu-id="edf36-141">String collection</span></span> | <span data-ttu-id="edf36-142">应挖掘的邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="edf36-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="edf36-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="edf36-143">filterQuery</span></span> | <span data-ttu-id="edf36-144">String</span><span class="sxs-lookup"><span data-stu-id="edf36-144">String</span></span> | <span data-ttu-id="edf36-145">用于筛选邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="edf36-145">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="edf36-146">响应</span><span class="sxs-lookup"><span data-stu-id="edf36-146">Response</span></span>
<span data-ttu-id="edf36-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [mailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="edf36-147">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edf36-148">示例</span><span class="sxs-lookup"><span data-stu-id="edf36-148">Example</span></span>
#### <a name="request"></a><span data-ttu-id="edf36-149">请求</span><span class="sxs-lookup"><span data-stu-id="edf36-149">Request</span></span>
<span data-ttu-id="edf36-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="edf36-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')))"
}
```

#### <a name="response"></a><span data-ttu-id="edf36-151">响应</span><span class="sxs-lookup"><span data-stu-id="edf36-151">Response</span></span>
<span data-ttu-id="edf36-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="edf36-152">The following is an example of the response.</span></span>
><span data-ttu-id="edf36-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="edf36-153">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="edf36-154">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="edf36-154">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

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
  "sourceFolderIDs": [
      "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'Analytics')"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="edf36-155">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="edf36-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="edf36-156">C#</span><span class="sxs-lookup"><span data-stu-id="edf36-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_mailsearchfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="edf36-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="edf36-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_mailsearchfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/mailsearchfolder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailsearchfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
