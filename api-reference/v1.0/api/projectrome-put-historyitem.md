---
title: 创建或替换 historyItem
description: 为现有用户活动创建新的或替换现有的历史记录项。
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: apiPageType
ms.openlocfilehash: 851862a49a3a6852d70e597d70f5622833c7c087
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025356"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="1dd36-103">创建或替换 historyItem</span><span class="sxs-lookup"><span data-stu-id="1dd36-103">Create or replace a historyItem</span></span>

<span data-ttu-id="1dd36-104">为现有用户活动创建新的或替换现有的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="1dd36-104">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="1dd36-105">权限</span><span class="sxs-lookup"><span data-stu-id="1dd36-105">Permissions</span></span>

<span data-ttu-id="1dd36-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1dd36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1dd36-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1dd36-108">Permission type</span></span>      | <span data-ttu-id="1dd36-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1dd36-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dd36-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1dd36-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1dd36-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1dd36-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1dd36-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1dd36-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dd36-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1dd36-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1dd36-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1dd36-114">Application</span></span> | <span data-ttu-id="1dd36-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1dd36-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dd36-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1dd36-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="1dd36-117">Id 必须是 GUID。</span><span class="sxs-lookup"><span data-stu-id="1dd36-117">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1dd36-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1dd36-118">Request headers</span></span>

|<span data-ttu-id="1dd36-119">名称</span><span class="sxs-lookup"><span data-stu-id="1dd36-119">Name</span></span> | <span data-ttu-id="1dd36-120">类型</span><span class="sxs-lookup"><span data-stu-id="1dd36-120">Type</span></span> | <span data-ttu-id="1dd36-121">说明</span><span class="sxs-lookup"><span data-stu-id="1dd36-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="1dd36-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dd36-122">Authorization</span></span> | <span data-ttu-id="1dd36-123">string</span><span class="sxs-lookup"><span data-stu-id="1dd36-123">string</span></span> | <span data-ttu-id="1dd36-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1dd36-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dd36-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1dd36-126">Request body</span></span>

<span data-ttu-id="1dd36-127">在请求正文中, 提供[historyItem](../resources/projectrome-historyitem.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1dd36-127">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1dd36-128">响应</span><span class="sxs-lookup"><span data-stu-id="1dd36-128">Response</span></span>

<span data-ttu-id="1dd36-129">如果成功, 此方法将在`201 Created`创建 historyItem 或`200 OK`替换 historyItem 时返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="1dd36-129">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="1dd36-130">示例</span><span class="sxs-lookup"><span data-stu-id="1dd36-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1dd36-131">请求</span><span class="sxs-lookup"><span data-stu-id="1dd36-131">Request</span></span>

<span data-ttu-id="1dd36-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1dd36-132">Here is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_historyItem"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
Content-type: application/json
Content-length: 364

{
    "startedDateTime": "2015-02-11T20:54:04.3457274+00:00",
    "userTimezone": "Africa/Casablanca",
    "lastActiveDateTime": "2015-02-11T20:54:04.3457274+00:00"
}
```

#### <a name="response"></a><span data-ttu-id="1dd36-133">响应</span><span class="sxs-lookup"><span data-stu-id="1dd36-133">Response</span></span>

<span data-ttu-id="1dd36-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1dd36-134">Here is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activityHistoryItem"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('user%40contoso.com')/activities('13881113971988980728')/historyItems/$entity",
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
