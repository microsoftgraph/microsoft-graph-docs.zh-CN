---
title: 删除 directoryObject
description: 删除 directoryObject。
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 74e1420bacd7a8c1437301dc1c01511acf46c9a9
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180963"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="06143-103">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="06143-103">Delete directoryObject</span></span>

<span data-ttu-id="06143-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06143-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06143-105">删除 directoryObject。</span><span class="sxs-lookup"><span data-stu-id="06143-105">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="06143-106">权限</span><span class="sxs-lookup"><span data-stu-id="06143-106">Permissions</span></span>
<span data-ttu-id="06143-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06143-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="06143-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="06143-109">Permission type</span></span>      | <span data-ttu-id="06143-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06143-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06143-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06143-111">Delegated (work or school account)</span></span> | <span data-ttu-id="06143-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06143-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06143-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06143-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06143-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="06143-114">Not supported.</span></span>    |
|<span data-ttu-id="06143-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="06143-115">Application</span></span> | <span data-ttu-id="06143-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="06143-116">Not supported.</span></span> |

<span data-ttu-id="06143-117">**注意：** 用户、组和联系人是 directory 对象的类型。</span><span class="sxs-lookup"><span data-stu-id="06143-117">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="06143-118">因此，如果需要删除用户，可以且应使用以下权限： User. ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="06143-118">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="06143-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06143-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="06143-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="06143-120">Request headers</span></span>
| <span data-ttu-id="06143-121">名称</span><span class="sxs-lookup"><span data-stu-id="06143-121">Name</span></span>       | <span data-ttu-id="06143-122">类型</span><span class="sxs-lookup"><span data-stu-id="06143-122">Type</span></span> | <span data-ttu-id="06143-123">说明</span><span class="sxs-lookup"><span data-stu-id="06143-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="06143-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="06143-124">Authorization</span></span>  | <span data-ttu-id="06143-125">string</span><span class="sxs-lookup"><span data-stu-id="06143-125">string</span></span>  | <span data-ttu-id="06143-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="06143-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06143-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="06143-128">Request body</span></span>
<span data-ttu-id="06143-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="06143-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06143-130">响应</span><span class="sxs-lookup"><span data-stu-id="06143-130">Response</span></span>

<span data-ttu-id="06143-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="06143-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06143-133">示例</span><span class="sxs-lookup"><span data-stu-id="06143-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06143-134">请求</span><span class="sxs-lookup"><span data-stu-id="06143-134">Request</span></span>
<span data-ttu-id="06143-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06143-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/ffab4dce-9b82-49a6-b7c7-1a143106598c
```
##### <a name="response"></a><span data-ttu-id="06143-136">响应</span><span class="sxs-lookup"><span data-stu-id="06143-136">Response</span></span>
<span data-ttu-id="06143-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="06143-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
