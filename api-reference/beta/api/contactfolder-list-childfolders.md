---
title: 列出 childFolder
description: 获取指定联系人文件夹下的子文件夹的集合。
ms.openlocfilehash: 7d379e81229ee8efd4c12718147a99ed13ebdb93
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044562"
---
# <a name="list-childfolders"></a><span data-ttu-id="dca2f-103">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="dca2f-103">List childFolders</span></span>

> <span data-ttu-id="dca2f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dca2f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dca2f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dca2f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dca2f-106">获取指定联系人文件夹下的子文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="dca2f-106">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="dca2f-107">权限</span><span class="sxs-lookup"><span data-stu-id="dca2f-107">Permissions</span></span>
<span data-ttu-id="dca2f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dca2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dca2f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dca2f-110">Permission type</span></span>      | <span data-ttu-id="dca2f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dca2f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dca2f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dca2f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dca2f-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dca2f-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="dca2f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dca2f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dca2f-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dca2f-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="dca2f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dca2f-116">Application</span></span> | <span data-ttu-id="dca2f-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dca2f-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dca2f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dca2f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dca2f-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dca2f-119">Optional query parameters</span></span>
<span data-ttu-id="dca2f-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dca2f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dca2f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="dca2f-121">Request headers</span></span>
| <span data-ttu-id="dca2f-122">名称</span><span class="sxs-lookup"><span data-stu-id="dca2f-122">Name</span></span>       | <span data-ttu-id="dca2f-123">类型</span><span class="sxs-lookup"><span data-stu-id="dca2f-123">Type</span></span> | <span data-ttu-id="dca2f-124">说明</span><span class="sxs-lookup"><span data-stu-id="dca2f-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dca2f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dca2f-125">Authorization</span></span>  | <span data-ttu-id="dca2f-126">string</span><span class="sxs-lookup"><span data-stu-id="dca2f-126">string</span></span>  | <span data-ttu-id="dca2f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dca2f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dca2f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="dca2f-129">Request body</span></span>
<span data-ttu-id="dca2f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dca2f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dca2f-131">响应</span><span class="sxs-lookup"><span data-stu-id="dca2f-131">Response</span></span>

<span data-ttu-id="dca2f-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ContactFolder](../resources/contactfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dca2f-132">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dca2f-133">示例</span><span class="sxs-lookup"><span data-stu-id="dca2f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dca2f-134">请求</span><span class="sxs-lookup"><span data-stu-id="dca2f-134">Request</span></span>
<span data-ttu-id="dca2f-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dca2f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="dca2f-136">响应</span><span class="sxs-lookup"><span data-stu-id="dca2f-136">Response</span></span>
<span data-ttu-id="dca2f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dca2f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
