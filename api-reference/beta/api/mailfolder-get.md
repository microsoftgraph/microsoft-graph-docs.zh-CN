---
title: 获取 mailFolder
description: 检索邮件文件夹对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: af2cc42c2ee72f1a57a1e0f9402209c107e259f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540898"
---
# <a name="get-mailfolder"></a><span data-ttu-id="7611e-103">获取 mailFolder</span><span class="sxs-lookup"><span data-stu-id="7611e-103">Get mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7611e-104">检索邮件文件夹对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7611e-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="7611e-105">在以下两种情况下, 应用可以获取其他用户的邮件文件夹:</span><span class="sxs-lookup"><span data-stu-id="7611e-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="7611e-106">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="7611e-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="7611e-107">如果应用具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了邮件文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="7611e-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="7611e-108">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="7611e-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="7611e-109">权限</span><span class="sxs-lookup"><span data-stu-id="7611e-109">Permissions</span></span>

<span data-ttu-id="7611e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7611e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7611e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7611e-112">Permission type</span></span>      | <span data-ttu-id="7611e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7611e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7611e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7611e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7611e-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7611e-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7611e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7611e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7611e-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7611e-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7611e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7611e-118">Application</span></span> | <span data-ttu-id="7611e-119">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7611e-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7611e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7611e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7611e-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7611e-121">Optional query parameters</span></span>

<span data-ttu-id="7611e-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7611e-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7611e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="7611e-123">Request headers</span></span>

| <span data-ttu-id="7611e-124">名称</span><span class="sxs-lookup"><span data-stu-id="7611e-124">Name</span></span>          | <span data-ttu-id="7611e-125">类型</span><span class="sxs-lookup"><span data-stu-id="7611e-125">Type</span></span>   | <span data-ttu-id="7611e-126">说明</span><span class="sxs-lookup"><span data-stu-id="7611e-126">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="7611e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7611e-127">Authorization</span></span> | <span data-ttu-id="7611e-128">string</span><span class="sxs-lookup"><span data-stu-id="7611e-128">string</span></span> | <span data-ttu-id="7611e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7611e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7611e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="7611e-131">Request body</span></span>

<span data-ttu-id="7611e-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7611e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7611e-133">响应</span><span class="sxs-lookup"><span data-stu-id="7611e-133">Response</span></span>

<span data-ttu-id="7611e-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7611e-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7611e-135">示例</span><span class="sxs-lookup"><span data-stu-id="7611e-135">Examples</span></span>

### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="7611e-136">示例 1: 获取邮件文件夹</span><span class="sxs-lookup"><span data-stu-id="7611e-136">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="7611e-137">请求</span><span class="sxs-lookup"><span data-stu-id="7611e-137">Request</span></span>

<span data-ttu-id="7611e-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7611e-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="7611e-139">响应</span><span class="sxs-lookup"><span data-stu-id="7611e-139">Response</span></span>

<span data-ttu-id="7611e-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7611e-140">The following is an example of the response.</span></span>

> <span data-ttu-id="7611e-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7611e-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7611e-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7611e-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkAGVmMDEzM",
  "displayName": "Inbox",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 2,
  "unreadItemCount": 59,
  "totalItemCount": 60,
  "wellKnownName": "inbox"
}
```

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="7611e-143">示例 2: 获取邮件搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="7611e-143">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="7611e-144">请求</span><span class="sxs-lookup"><span data-stu-id="7611e-144">Request</span></span>

<span data-ttu-id="7611e-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7611e-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailSearchfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzN
```

#### <a name="response"></a><span data-ttu-id="7611e-146">响应</span><span class="sxs-lookup"><span data-stu-id="7611e-146">Response</span></span>

<span data-ttu-id="7611e-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7611e-147">The following is an example of the response.</span></span>

> <span data-ttu-id="7611e-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7611e-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7611e-149">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7611e-149">All the properties will be returned from an actual call.</span></span>

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
  "id": "AAMkAGVmMDEzN",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 0,
  "unreadItemCount": 6,
  "totalItemCount": 6,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
    "AAMkAGVmMDEzM"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
