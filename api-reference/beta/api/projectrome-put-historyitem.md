---
title: 创建或替换 historyItem
description: 为现有用户活动创建新的或替换现有的历史记录项。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 0a8d03029350ce96e7442473dffa0595278bc195
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337255"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="63767-103">创建或替换 historyItem</span><span class="sxs-lookup"><span data-stu-id="63767-103">Create or replace a historyItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63767-104">为现有用户活动创建新的或替换现有的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="63767-104">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="63767-105">权限</span><span class="sxs-lookup"><span data-stu-id="63767-105">Permissions</span></span>

<span data-ttu-id="63767-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63767-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="63767-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="63767-108">Permission type</span></span>      | <span data-ttu-id="63767-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63767-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63767-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63767-110">Delegated (work or school account)</span></span> | <span data-ttu-id="63767-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="63767-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="63767-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63767-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63767-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="63767-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="63767-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="63767-114">Application</span></span> | <span data-ttu-id="63767-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="63767-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63767-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63767-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="63767-117">Id 必须是 GUID。</span><span class="sxs-lookup"><span data-stu-id="63767-117">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63767-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="63767-118">Request headers</span></span>

|<span data-ttu-id="63767-119">名称</span><span class="sxs-lookup"><span data-stu-id="63767-119">Name</span></span> | <span data-ttu-id="63767-120">类型</span><span class="sxs-lookup"><span data-stu-id="63767-120">Type</span></span> | <span data-ttu-id="63767-121">说明</span><span class="sxs-lookup"><span data-stu-id="63767-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="63767-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="63767-122">Authorization</span></span> | <span data-ttu-id="63767-123">string</span><span class="sxs-lookup"><span data-stu-id="63767-123">string</span></span> | <span data-ttu-id="63767-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63767-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63767-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="63767-126">Request body</span></span>

<span data-ttu-id="63767-127">在请求正文中, 提供[historyItem](../resources/projectrome-historyitem.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63767-127">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="63767-128">响应</span><span class="sxs-lookup"><span data-stu-id="63767-128">Response</span></span>

<span data-ttu-id="63767-129">如果成功, 此方法将在`201 Created`创建 historyItem 或`200 OK`替换 historyItem 时返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="63767-129">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="63767-130">示例</span><span class="sxs-lookup"><span data-stu-id="63767-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="63767-131">请求</span><span class="sxs-lookup"><span data-stu-id="63767-131">Request</span></span>

<span data-ttu-id="63767-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63767-132">Here is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="63767-133">响应</span><span class="sxs-lookup"><span data-stu-id="63767-133">Response</span></span>

<span data-ttu-id="63767-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="63767-134">Here is an example of the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Upsert historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
