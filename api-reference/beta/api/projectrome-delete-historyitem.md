---
title: 删除 historyItem
description: 删除现有用户活动的现有历史记录项。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: b3e9a505c47c4d43aff71d5b4e40f08e3fe29d2b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520422"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="1cc6a-103">删除 historyItem</span><span class="sxs-lookup"><span data-stu-id="1cc6a-103">Delete a historyItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cc6a-104">删除现有用户活动的现有历史记录项。</span><span class="sxs-lookup"><span data-stu-id="1cc6a-104">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cc6a-105">权限</span><span class="sxs-lookup"><span data-stu-id="1cc6a-105">Permissions</span></span>

<span data-ttu-id="1cc6a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1cc6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1cc6a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1cc6a-108">Permission type</span></span>      | <span data-ttu-id="1cc6a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1cc6a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cc6a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1cc6a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1cc6a-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1cc6a-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1cc6a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1cc6a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cc6a-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1cc6a-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1cc6a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1cc6a-114">Application</span></span> | <span data-ttu-id="1cc6a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1cc6a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cc6a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1cc6a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1cc6a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1cc6a-117">Request headers</span></span>

|<span data-ttu-id="1cc6a-118">名称</span><span class="sxs-lookup"><span data-stu-id="1cc6a-118">Name</span></span> | <span data-ttu-id="1cc6a-119">类型</span><span class="sxs-lookup"><span data-stu-id="1cc6a-119">Type</span></span> | <span data-ttu-id="1cc6a-120">说明</span><span class="sxs-lookup"><span data-stu-id="1cc6a-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="1cc6a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cc6a-121">Authorization</span></span> | <span data-ttu-id="1cc6a-122">string</span><span class="sxs-lookup"><span data-stu-id="1cc6a-122">string</span></span> | <span data-ttu-id="1cc6a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1cc6a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cc6a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1cc6a-125">Request body</span></span>

<span data-ttu-id="1cc6a-126">没有请求正文中。</span><span class="sxs-lookup"><span data-stu-id="1cc6a-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="1cc6a-127">响应</span><span class="sxs-lookup"><span data-stu-id="1cc6a-127">Response</span></span>

<span data-ttu-id="1cc6a-128">如果成功，此方法返回`204 No Content`如果历史记录项已删除的响应代码。</span><span class="sxs-lookup"><span data-stu-id="1cc6a-128">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="1cc6a-129">示例</span><span class="sxs-lookup"><span data-stu-id="1cc6a-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1cc6a-130">请求</span><span class="sxs-lookup"><span data-stu-id="1cc6a-130">Request</span></span>

<span data-ttu-id="1cc6a-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1cc6a-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```

##### <a name="response"></a><span data-ttu-id="1cc6a-132">响应</span><span class="sxs-lookup"><span data-stu-id="1cc6a-132">Response</span></span>

<span data-ttu-id="1cc6a-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1cc6a-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-delete-historyitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
