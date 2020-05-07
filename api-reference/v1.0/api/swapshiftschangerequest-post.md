---
title: 创建 swapshiftRequest
description: 创建 swapShiftsChangeRequest 的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fae65ef9812b68bea46960966af7caf694cb3b37
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155017"
---
# <a name="create-swapshiftschangerequest"></a><span data-ttu-id="88be0-103">创建 swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="88be0-103">Create swapShiftsChangeRequest</span></span>

<span data-ttu-id="88be0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88be0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="88be0-105">创建[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象的实例。</span><span class="sxs-lookup"><span data-stu-id="88be0-105">Create an instance of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="88be0-106">权限</span><span class="sxs-lookup"><span data-stu-id="88be0-106">Permissions</span></span>

<span data-ttu-id="88be0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88be0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="88be0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="88be0-109">Permission type</span></span>                        | <span data-ttu-id="88be0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88be0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="88be0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88be0-111">Delegated (work or school account)</span></span> |<span data-ttu-id="88be0-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="88be0-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="88be0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88be0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88be0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="88be0-114">Not supported.</span></span>    |
|<span data-ttu-id="88be0-115">Application</span><span class="sxs-lookup"><span data-stu-id="88be0-115">Application</span></span> | <span data-ttu-id="88be0-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88be0-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="88be0-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="88be0-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="88be0-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="88be0-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="88be0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88be0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88be0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="88be0-120">Optional query parameters</span></span>

<span data-ttu-id="88be0-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="88be0-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="88be0-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="88be0-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="88be0-123">请求头</span><span class="sxs-lookup"><span data-stu-id="88be0-123">Request headers</span></span>

| <span data-ttu-id="88be0-124">名称</span><span class="sxs-lookup"><span data-stu-id="88be0-124">Name</span></span>      |<span data-ttu-id="88be0-125">说明</span><span class="sxs-lookup"><span data-stu-id="88be0-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="88be0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="88be0-126">Authorization</span></span> | <span data-ttu-id="88be0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88be0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="88be0-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="88be0-129">Content-type</span></span> | <span data-ttu-id="88be0-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="88be0-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88be0-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="88be0-132">Request body</span></span>
<span data-ttu-id="88be0-133">在请求正文中，提供新的[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88be0-133">In the request body, provide a JSON representation of a new [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="88be0-134">响应</span><span class="sxs-lookup"><span data-stu-id="88be0-134">Response</span></span>

<span data-ttu-id="88be0-135">如果成功，此方法在响应`200 OK`正文中返回响应代码和创建的[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="88be0-135">If successful, this method returns a `200 OK` response code and the created [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="88be0-136">示例</span><span class="sxs-lookup"><span data-stu-id="88be0-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="88be0-137">请求</span><span class="sxs-lookup"><span data-stu-id="88be0-137">Request</span></span>

<span data-ttu-id="88be0-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="88be0-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/swapShiftsChangeRequests
Authorization: Bearer {token}
Content-type: application/json

{
  "senderShiftId": "5ad10161-6524-4c7c-9beb-4e8677ba2f6d",
  "senderMessage": "I can't make my shift, any chance we can swap?",
  "recipientUserId": "567c8ea5-9e32-422a-a663-8270201699cd",
  "recipientShiftId": "e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c"
}
```

### <a name="response"></a><span data-ttu-id="88be0-139">响应</span><span class="sxs-lookup"><span data-stu-id="88be0-139">Response</span></span>

<span data-ttu-id="88be0-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="88be0-140">The following is an example of the response.</span></span>

> <span data-ttu-id="88be0-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="88be0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
"id": "0b87dd20-d5ed-4764-9c3e-cfc8516def09",
"senderShiftId": "5ad10161-6524-4c7c-9beb-4e8677ba2f6d",
"recipientShiftId": "e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c",
"assignedTo": "recipient",
"state": "pending",
"senderUserId": "3fe0bc21-1398-4fd9-9713-52511b434c1e",
"senderDateTime": "2019-05-01T10:00:00Z",
"senderMessage": "I can't make my shift, any chance we can swap?",
"recipientUserId": "567c8ea5-9e32-422a-a663-8270201699cd",
"recipientActionDateTime": null,
"recipientActionMessage": null,
"managerUserId": null,
"managerActionDateTime": null,
"managerActionMessage": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create swapShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
