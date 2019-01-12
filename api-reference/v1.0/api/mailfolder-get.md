---
title: 获取 mailFolder
description: 检索邮件文件夹对象的属性和关系。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: d2f61152b8edd98aa11fc7c6b34d2c2b04b72f55
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990122"
---
# <a name="get-mailfolder"></a><span data-ttu-id="276e6-103">获取 mailFolder</span><span class="sxs-lookup"><span data-stu-id="276e6-103">Get mailFolder</span></span>

<span data-ttu-id="276e6-104">检索邮件文件夹对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="276e6-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="276e6-105">有两种方案相关应用程序可以在哪里找到另一个用户的邮件文件夹：</span><span class="sxs-lookup"><span data-stu-id="276e6-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="276e6-106">如果应用程序具有应用程序权限，或，</span><span class="sxs-lookup"><span data-stu-id="276e6-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="276e6-107">如果应用程序具有相应从一个用户委派[权限](#permissions)，并另一个用户具有与该用户，共享邮件文件夹，或具有委派的访问赋予该用户。</span><span class="sxs-lookup"><span data-stu-id="276e6-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="276e6-108">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="276e6-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="276e6-109">权限</span><span class="sxs-lookup"><span data-stu-id="276e6-109">Permissions</span></span>
<span data-ttu-id="276e6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="276e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="276e6-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="276e6-112">Permission type</span></span>      | <span data-ttu-id="276e6-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="276e6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="276e6-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="276e6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="276e6-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="276e6-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="276e6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="276e6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="276e6-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="276e6-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="276e6-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="276e6-118">Application</span></span> | <span data-ttu-id="276e6-119">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="276e6-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="276e6-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="276e6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="276e6-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="276e6-121">Optional query parameters</span></span>
<span data-ttu-id="276e6-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="276e6-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="276e6-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="276e6-123">Request headers</span></span>
| <span data-ttu-id="276e6-124">名称</span><span class="sxs-lookup"><span data-stu-id="276e6-124">Name</span></span>       | <span data-ttu-id="276e6-125">类型</span><span class="sxs-lookup"><span data-stu-id="276e6-125">Type</span></span> | <span data-ttu-id="276e6-126">说明</span><span class="sxs-lookup"><span data-stu-id="276e6-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="276e6-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="276e6-127">Authorization</span></span>  | <span data-ttu-id="276e6-128">string</span><span class="sxs-lookup"><span data-stu-id="276e6-128">string</span></span>  | <span data-ttu-id="276e6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="276e6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="276e6-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="276e6-131">Request body</span></span>
<span data-ttu-id="276e6-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="276e6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="276e6-133">响应</span><span class="sxs-lookup"><span data-stu-id="276e6-133">Response</span></span>

<span data-ttu-id="276e6-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="276e6-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="276e6-135">示例</span><span class="sxs-lookup"><span data-stu-id="276e6-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="276e6-136">请求</span><span class="sxs-lookup"><span data-stu-id="276e6-136">Request</span></span>
<span data-ttu-id="276e6-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="276e6-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="276e6-138">响应</span><span class="sxs-lookup"><span data-stu-id="276e6-138">Response</span></span>
<span data-ttu-id="276e6-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="276e6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
