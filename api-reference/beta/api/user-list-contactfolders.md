---
title: List contactFolders
description: 获取登录用户的邮箱中的所有联系人文件夹。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 591a0be85113aeb57b536aa0986544cef1eb5b85
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334777"
---
# <a name="list-contactfolders"></a><span data-ttu-id="0bbfd-103">List contactFolders</span><span class="sxs-lookup"><span data-stu-id="0bbfd-103">List contactFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bbfd-104">获取登录用户的邮箱中的所有联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-104">Get all the contact folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bbfd-105">权限</span><span class="sxs-lookup"><span data-stu-id="0bbfd-105">Permissions</span></span>
<span data-ttu-id="0bbfd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bbfd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0bbfd-108">Permission type</span></span>      | <span data-ttu-id="0bbfd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0bbfd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bbfd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0bbfd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0bbfd-111">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0bbfd-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0bbfd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0bbfd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bbfd-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0bbfd-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0bbfd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0bbfd-114">Application</span></span> | <span data-ttu-id="0bbfd-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0bbfd-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bbfd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0bbfd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0bbfd-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0bbfd-117">Optional query parameters</span></span>
<span data-ttu-id="0bbfd-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0bbfd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0bbfd-119">Request headers</span></span>
| <span data-ttu-id="0bbfd-120">标头</span><span class="sxs-lookup"><span data-stu-id="0bbfd-120">Header</span></span>       | <span data-ttu-id="0bbfd-121">值</span><span class="sxs-lookup"><span data-stu-id="0bbfd-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0bbfd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bbfd-122">Authorization</span></span>  | <span data-ttu-id="0bbfd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0bbfd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0bbfd-125">Content-Type</span></span>   | <span data-ttu-id="0bbfd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bbfd-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0bbfd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0bbfd-127">Request body</span></span>
<span data-ttu-id="0bbfd-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bbfd-129">响应</span><span class="sxs-lookup"><span data-stu-id="0bbfd-129">Response</span></span>

<span data-ttu-id="0bbfd-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ContactFolder](../resources/contactfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0bbfd-131">示例</span><span class="sxs-lookup"><span data-stu-id="0bbfd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0bbfd-132">请求</span><span class="sxs-lookup"><span data-stu-id="0bbfd-132">Request</span></span>
<span data-ttu-id="0bbfd-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders
```
##### <a name="response"></a><span data-ttu-id="0bbfd-134">响应</span><span class="sxs-lookup"><span data-stu-id="0bbfd-134">Response</span></span>
<span data-ttu-id="0bbfd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0bbfd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "wellKnownName": "wellKnownName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
