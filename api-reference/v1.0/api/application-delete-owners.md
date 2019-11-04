---
title: 删除所有者
description: 从应用程序中删除所有者。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c9a2ad6319b7478051b3e5b4e6ed3e46432f6ff4
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939738"
---
# <a name="remove-owner"></a><span data-ttu-id="205d7-103">删除所有者</span><span class="sxs-lookup"><span data-stu-id="205d7-103">Remove owner</span></span>

<span data-ttu-id="205d7-104">从[应用程序](../resources/application.md)中删除所有者。</span><span class="sxs-lookup"><span data-stu-id="205d7-104">Remove an owner from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="205d7-105">权限</span><span class="sxs-lookup"><span data-stu-id="205d7-105">Permissions</span></span>
<span data-ttu-id="205d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="205d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="205d7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="205d7-108">Permission type</span></span>      | <span data-ttu-id="205d7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="205d7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="205d7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="205d7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="205d7-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="205d7-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="205d7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="205d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="205d7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="205d7-113">Not supported.</span></span>    |
|<span data-ttu-id="205d7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="205d7-114">Application</span></span> | <span data-ttu-id="205d7-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="205d7-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="205d7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="205d7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/{id}/$ref

```
## <a name="request-headers"></a><span data-ttu-id="205d7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="205d7-117">Request headers</span></span>
| <span data-ttu-id="205d7-118">名称</span><span class="sxs-lookup"><span data-stu-id="205d7-118">Name</span></span> | <span data-ttu-id="205d7-119">说明</span><span class="sxs-lookup"><span data-stu-id="205d7-119">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="205d7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="205d7-120">Authorization</span></span> | <span data-ttu-id="205d7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="205d7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="205d7-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="205d7-123">Request body</span></span>
<span data-ttu-id="205d7-124">在请求正文中，提供要作为所有者分配的目录对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="205d7-124">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="205d7-125">响应</span><span class="sxs-lookup"><span data-stu-id="205d7-125">Response</span></span>

<span data-ttu-id="205d7-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="205d7-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="205d7-127">示例</span><span class="sxs-lookup"><span data-stu-id="205d7-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="205d7-128">请求</span><span class="sxs-lookup"><span data-stu-id="205d7-128">Request</span></span>

<span data-ttu-id="205d7-129">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="205d7-129">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "application_delete_owners"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/owners/{id}/$ref
Content-type: application/json
Content-length: 30

{
"@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

```

### <a name="response"></a><span data-ttu-id="205d7-130">响应</span><span class="sxs-lookup"><span data-stu-id="205d7-130">Response</span></span>

<span data-ttu-id="205d7-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="205d7-131">The following is an example of the response.</span></span>

><span data-ttu-id="205d7-132">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="205d7-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="205d7-133">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="205d7-133">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
