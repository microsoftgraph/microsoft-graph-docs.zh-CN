---
title: 列出 childFolder
description: 获取指定联系人文件夹下的子文件夹的集合。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3d0f6d14249e488333954b3a45c3bed0f6eaf93a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987795"
---
# <a name="list-childfolders"></a><span data-ttu-id="a8199-103">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="a8199-103">List childFolders</span></span>

<span data-ttu-id="a8199-104">获取指定联系人文件夹下的子文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="a8199-104">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="a8199-105">权限</span><span class="sxs-lookup"><span data-stu-id="a8199-105">Permissions</span></span>
<span data-ttu-id="a8199-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8199-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8199-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8199-108">Permission type</span></span>      | <span data-ttu-id="a8199-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8199-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8199-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8199-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a8199-111">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8199-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a8199-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8199-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8199-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8199-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a8199-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8199-114">Application</span></span> | <span data-ttu-id="a8199-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8199-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8199-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8199-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a8199-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a8199-117">Optional query parameters</span></span>
<span data-ttu-id="a8199-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a8199-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a8199-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8199-119">Request headers</span></span>
| <span data-ttu-id="a8199-120">名称</span><span class="sxs-lookup"><span data-stu-id="a8199-120">Name</span></span>       | <span data-ttu-id="a8199-121">类型</span><span class="sxs-lookup"><span data-stu-id="a8199-121">Type</span></span> | <span data-ttu-id="a8199-122">说明</span><span class="sxs-lookup"><span data-stu-id="a8199-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a8199-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8199-123">Authorization</span></span>  | <span data-ttu-id="a8199-124">string</span><span class="sxs-lookup"><span data-stu-id="a8199-124">string</span></span>  | <span data-ttu-id="a8199-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8199-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8199-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8199-127">Request body</span></span>
<span data-ttu-id="a8199-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a8199-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8199-129">响应</span><span class="sxs-lookup"><span data-stu-id="a8199-129">Response</span></span>

<span data-ttu-id="a8199-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ContactFolder](../resources/contactfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a8199-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a8199-131">示例</span><span class="sxs-lookup"><span data-stu-id="a8199-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8199-132">请求</span><span class="sxs-lookup"><span data-stu-id="a8199-132">Request</span></span>
<span data-ttu-id="a8199-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8199-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="a8199-134">响应</span><span class="sxs-lookup"><span data-stu-id="a8199-134">Response</span></span>
<span data-ttu-id="a8199-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a8199-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
