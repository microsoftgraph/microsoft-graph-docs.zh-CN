---
title: 获取 contactFolder
description: 通过使用联系人文件夹 ID 获取联系人文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 86f2adf867737e31d96a75d40f50442b10a468b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985114"
---
# <a name="get-contactfolder"></a><span data-ttu-id="10e69-103">获取 contactFolder</span><span class="sxs-lookup"><span data-stu-id="10e69-103">Get contactFolder</span></span>

> <span data-ttu-id="10e69-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="10e69-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10e69-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="10e69-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="10e69-106">通过使用联系人文件夹 ID 获取联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="10e69-106">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="10e69-107">有两种方案相关应用程序可以在哪里找到另一个用户的联系人文件夹：</span><span class="sxs-lookup"><span data-stu-id="10e69-107">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="10e69-108">如果应用程序具有应用程序权限，或，</span><span class="sxs-lookup"><span data-stu-id="10e69-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="10e69-109">如果应用程序具有相应从一个用户委派[权限](#permissions)，并另一个用户具有与该用户，共享联系人文件夹，或具有委派的访问赋予该用户。</span><span class="sxs-lookup"><span data-stu-id="10e69-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="10e69-110">请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。</span><span class="sxs-lookup"><span data-stu-id="10e69-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="10e69-111">权限</span><span class="sxs-lookup"><span data-stu-id="10e69-111">Permissions</span></span>
<span data-ttu-id="10e69-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10e69-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10e69-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="10e69-114">Permission type</span></span>      | <span data-ttu-id="10e69-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10e69-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10e69-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10e69-116">Delegated (work or school account)</span></span> | <span data-ttu-id="10e69-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10e69-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="10e69-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10e69-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10e69-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10e69-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="10e69-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="10e69-120">Application</span></span> | <span data-ttu-id="10e69-121">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10e69-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="10e69-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10e69-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="10e69-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="10e69-123">Optional query parameters</span></span>
<span data-ttu-id="10e69-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="10e69-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="10e69-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="10e69-125">Request headers</span></span>
| <span data-ttu-id="10e69-126">名称</span><span class="sxs-lookup"><span data-stu-id="10e69-126">Name</span></span>       | <span data-ttu-id="10e69-127">类型</span><span class="sxs-lookup"><span data-stu-id="10e69-127">Type</span></span> | <span data-ttu-id="10e69-128">说明</span><span class="sxs-lookup"><span data-stu-id="10e69-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="10e69-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="10e69-129">Authorization</span></span>  | <span data-ttu-id="10e69-130">string</span><span class="sxs-lookup"><span data-stu-id="10e69-130">string</span></span>  | <span data-ttu-id="10e69-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="10e69-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10e69-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="10e69-133">Request body</span></span>
<span data-ttu-id="10e69-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="10e69-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10e69-135">响应</span><span class="sxs-lookup"><span data-stu-id="10e69-135">Response</span></span>

<span data-ttu-id="10e69-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="10e69-136">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10e69-137">示例</span><span class="sxs-lookup"><span data-stu-id="10e69-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10e69-138">请求</span><span class="sxs-lookup"><span data-stu-id="10e69-138">Request</span></span>
<span data-ttu-id="10e69-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10e69-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="10e69-140">响应</span><span class="sxs-lookup"><span data-stu-id="10e69-140">Response</span></span>
<span data-ttu-id="10e69-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="10e69-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "wellKnownName": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
