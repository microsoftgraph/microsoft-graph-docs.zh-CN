---
title: 更新 mailSearchFolder
description: 更新 mailSearchFolder 对象的可写属性。
ms.openlocfilehash: abe32817c45ee1e05fbb251bd46a31941eb4218b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049511"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="b9f06-103">更新 mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="b9f06-103">Update mailSearchFolder</span></span>

> <span data-ttu-id="b9f06-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b9f06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9f06-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b9f06-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9f06-106">更新[mailSearchFolder](../resources/mailsearchfolder.md)对象的可写属性。</span><span class="sxs-lookup"><span data-stu-id="b9f06-106">Update the writable properties of [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9f06-107">权限</span><span class="sxs-lookup"><span data-stu-id="b9f06-107">Permissions</span></span>
<span data-ttu-id="b9f06-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9f06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9f06-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9f06-110">Permission type</span></span>      | <span data-ttu-id="b9f06-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9f06-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9f06-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9f06-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b9f06-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9f06-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b9f06-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9f06-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9f06-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9f06-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b9f06-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9f06-116">Application</span></span> | <span data-ttu-id="b9f06-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9f06-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9f06-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9f06-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b9f06-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9f06-119">Request headers</span></span>
| <span data-ttu-id="b9f06-120">标头</span><span class="sxs-lookup"><span data-stu-id="b9f06-120">Header</span></span>       | <span data-ttu-id="b9f06-121">值</span><span class="sxs-lookup"><span data-stu-id="b9f06-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b9f06-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9f06-122">Authorization</span></span>  | <span data-ttu-id="b9f06-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9f06-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b9f06-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9f06-125">Content-Type</span></span>  | <span data-ttu-id="b9f06-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b9f06-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9f06-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9f06-128">Request body</span></span>
<span data-ttu-id="b9f06-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b9f06-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b9f06-132">属性</span><span class="sxs-lookup"><span data-stu-id="b9f06-132">Property</span></span>     | <span data-ttu-id="b9f06-133">类型</span><span class="sxs-lookup"><span data-stu-id="b9f06-133">Type</span></span>   |<span data-ttu-id="b9f06-134">说明</span><span class="sxs-lookup"><span data-stu-id="b9f06-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b9f06-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b9f06-135">displayName</span></span> | <span data-ttu-id="b9f06-136">字符串</span><span class="sxs-lookup"><span data-stu-id="b9f06-136">String</span></span> | <span data-ttu-id="b9f06-137">[MailFolder](../resources/mailfolder.md)显示名称。</span><span class="sxs-lookup"><span data-stu-id="b9f06-137">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="b9f06-138">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="b9f06-138">includeNestedFolders</span></span> | <span data-ttu-id="b9f06-139">布尔</span><span class="sxs-lookup"><span data-stu-id="b9f06-139">Boolean</span></span> | <span data-ttu-id="b9f06-140">如何应遍历的邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="b9f06-140">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="b9f06-141">`true`意味着应为深入搜索完成时`false`意味着浅表搜索应改为完成。</span><span class="sxs-lookup"><span data-stu-id="b9f06-141">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="b9f06-142">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="b9f06-142">sourceFolderIDs</span></span> | <span data-ttu-id="b9f06-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="b9f06-143">String collection</span></span> | <span data-ttu-id="b9f06-144">应 mined 邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="b9f06-144">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="b9f06-145">filterQuery</span><span class="sxs-lookup"><span data-stu-id="b9f06-145">filterQuery</span></span> | <span data-ttu-id="b9f06-146">字符串</span><span class="sxs-lookup"><span data-stu-id="b9f06-146">String</span></span> | <span data-ttu-id="b9f06-147">要筛选的邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="b9f06-147">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="b9f06-148">响应</span><span class="sxs-lookup"><span data-stu-id="b9f06-148">Response</span></span>
<span data-ttu-id="b9f06-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [mailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9f06-149">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9f06-150">示例</span><span class="sxs-lookup"><span data-stu-id="b9f06-150">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b9f06-151">请求</span><span class="sxs-lookup"><span data-stu-id="b9f06-151">Request</span></span>
<span data-ttu-id="b9f06-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b9f06-152">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="b9f06-153">响应</span><span class="sxs-lookup"><span data-stu-id="b9f06-153">Response</span></span>
<span data-ttu-id="b9f06-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b9f06-154">The following is an example of the response.</span></span>
><span data-ttu-id="b9f06-155">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b9f06-155">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b9f06-156">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b9f06-156">All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
