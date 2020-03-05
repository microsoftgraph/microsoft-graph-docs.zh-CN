---
title: 创建或替换 historyItem
description: 为现有用户活动创建新的或替换现有的历史记录项。
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ''
ms.openlocfilehash: 9d7f6d7888ba8a14f16e3756c4c01c3a16c3d73a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454872"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="09a3a-103">创建或替换 historyItem</span><span class="sxs-lookup"><span data-stu-id="09a3a-103">Create or replace a historyItem</span></span>

<span data-ttu-id="09a3a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="09a3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09a3a-105">为现有用户活动创建新的或替换现有的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="09a3a-105">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="09a3a-106">权限</span><span class="sxs-lookup"><span data-stu-id="09a3a-106">Permissions</span></span>

<span data-ttu-id="09a3a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09a3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="09a3a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="09a3a-109">Permission type</span></span>      | <span data-ttu-id="09a3a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09a3a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09a3a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09a3a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="09a3a-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="09a3a-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="09a3a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09a3a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09a3a-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="09a3a-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="09a3a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="09a3a-115">Application</span></span> | <span data-ttu-id="09a3a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="09a3a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="09a3a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09a3a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="09a3a-118">Id 必须是 GUID。</span><span class="sxs-lookup"><span data-stu-id="09a3a-118">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09a3a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="09a3a-119">Request headers</span></span>

|<span data-ttu-id="09a3a-120">名称</span><span class="sxs-lookup"><span data-stu-id="09a3a-120">Name</span></span> | <span data-ttu-id="09a3a-121">类型</span><span class="sxs-lookup"><span data-stu-id="09a3a-121">Type</span></span> | <span data-ttu-id="09a3a-122">说明</span><span class="sxs-lookup"><span data-stu-id="09a3a-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="09a3a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="09a3a-123">Authorization</span></span> | <span data-ttu-id="09a3a-124">string</span><span class="sxs-lookup"><span data-stu-id="09a3a-124">string</span></span> | <span data-ttu-id="09a3a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09a3a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="09a3a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="09a3a-127">Request body</span></span>

<span data-ttu-id="09a3a-128">在请求正文中，提供[historyItem](../resources/projectrome-historyitem.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09a3a-128">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="09a3a-129">响应</span><span class="sxs-lookup"><span data-stu-id="09a3a-129">Response</span></span>

<span data-ttu-id="09a3a-130">如果成功，此方法将在`201 Created`创建 historyItem 或`200 OK`替换 historyItem 时返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="09a3a-130">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="09a3a-131">示例</span><span class="sxs-lookup"><span data-stu-id="09a3a-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="09a3a-132">请求</span><span class="sxs-lookup"><span data-stu-id="09a3a-132">Request</span></span>

<span data-ttu-id="09a3a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="09a3a-133">Here is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="09a3a-134">响应</span><span class="sxs-lookup"><span data-stu-id="09a3a-134">Response</span></span>

<span data-ttu-id="09a3a-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="09a3a-135">Here is an example of the response.</span></span>

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
