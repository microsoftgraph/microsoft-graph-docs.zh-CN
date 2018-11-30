---
title: 创建或替换 historyItem
description: 创建一个新或替换现有的用户活动的现有历史记录项。
ms.openlocfilehash: 068e5cb4b98879c1dba5eeef56517b99c3fe47c8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049158"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="082bb-103">创建或替换 historyItem</span><span class="sxs-lookup"><span data-stu-id="082bb-103">Create or replace a historyItem</span></span>

> <span data-ttu-id="082bb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="082bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="082bb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="082bb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="082bb-106">创建一个新或替换现有的用户活动的现有历史记录项。</span><span class="sxs-lookup"><span data-stu-id="082bb-106">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="082bb-107">权限</span><span class="sxs-lookup"><span data-stu-id="082bb-107">Permissions</span></span>

<span data-ttu-id="082bb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="082bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="082bb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="082bb-110">Permission type</span></span>      | <span data-ttu-id="082bb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="082bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="082bb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="082bb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="082bb-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="082bb-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="082bb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="082bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="082bb-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="082bb-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="082bb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="082bb-116">Application</span></span> | <span data-ttu-id="082bb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="082bb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="082bb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="082bb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="082bb-119">Id 需要一个 GUID。</span><span class="sxs-lookup"><span data-stu-id="082bb-119">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="082bb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="082bb-120">Request headers</span></span>

|<span data-ttu-id="082bb-121">名称</span><span class="sxs-lookup"><span data-stu-id="082bb-121">Name</span></span> | <span data-ttu-id="082bb-122">类型</span><span class="sxs-lookup"><span data-stu-id="082bb-122">Type</span></span> | <span data-ttu-id="082bb-123">说明</span><span class="sxs-lookup"><span data-stu-id="082bb-123">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="082bb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="082bb-124">Authorization</span></span> | <span data-ttu-id="082bb-125">string</span><span class="sxs-lookup"><span data-stu-id="082bb-125">string</span></span> | <span data-ttu-id="082bb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="082bb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="082bb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="082bb-128">Request body</span></span>

<span data-ttu-id="082bb-129">在请求正文中，提供[historyItem](../resources/projectrome-historyitem.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="082bb-129">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="082bb-130">响应</span><span class="sxs-lookup"><span data-stu-id="082bb-130">Response</span></span>

<span data-ttu-id="082bb-131">如果成功，此方法返回`201 Created`如果 historyItem 已创建的响应代码或`200 OK`如果 historyItem 被替换。</span><span class="sxs-lookup"><span data-stu-id="082bb-131">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="082bb-132">示例</span><span class="sxs-lookup"><span data-stu-id="082bb-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="082bb-133">请求</span><span class="sxs-lookup"><span data-stu-id="082bb-133">Request</span></span>

<span data-ttu-id="082bb-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="082bb-134">Here is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_historyItem"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
Content-type: application/json
Content-length: 364

{
    "startedDateTime": "2015-02-11T20:54:04.3457274+00:00",
    "userTimezone": "Africa/Casablanca",
    "lastActiveDateTime": "2015-02-11T20:54:04.3457274+00:00"
}
```

#### <a name="response"></a><span data-ttu-id="082bb-135">响应</span><span class="sxs-lookup"><span data-stu-id="082bb-135">Response</span></span>

<span data-ttu-id="082bb-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="082bb-136">Here is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.historyItem"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('user%40contoso.com')/activities('13881113971988980728')/historyItems/$entity",
    "status": "updated",
    "userTimezone": "Africa/Casablanca",
    "createdDateTime": "2018-02-26T20:28:22.14Z",
    "lastModifiedDateTime": "2018-02-26T20:28:22.155Z",
    "id": "9d0b74e4-4b41-43ea-b34d-f9c1bf9f809c",
    "startedDateTime": "2018-02-26T20:54:04.345Z",
    "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
    "expirationDateTime": "2018-03-28T20:28:22.14Z",
    "activeDurationSeconds": 20
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->