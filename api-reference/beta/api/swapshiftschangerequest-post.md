---
title: 创建 swapshiftRequest
description: 创建 swapShiftsChangeRequest 的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1b1f873194d18f3ec34681f90942d5de2cbb089b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054831"
---
# <a name="create-swapshiftschangerequest"></a><span data-ttu-id="1d3a4-103">创建 swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="1d3a4-103">Create swapShiftsChangeRequest</span></span>

<span data-ttu-id="1d3a4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d3a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d3a4-105">创建 [swapShiftsChangeRequest 对象](../resources/swapshiftschangerequest.md) 的实例。</span><span class="sxs-lookup"><span data-stu-id="1d3a4-105">Create an instance of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d3a4-106">权限</span><span class="sxs-lookup"><span data-stu-id="1d3a4-106">Permissions</span></span>

<span data-ttu-id="1d3a4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d3a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1d3a4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d3a4-109">Permission type</span></span>                        | <span data-ttu-id="1d3a4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1d3a4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1d3a4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d3a4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1d3a4-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d3a4-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1d3a4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d3a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d3a4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d3a4-114">Not supported.</span></span> |
| <span data-ttu-id="1d3a4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d3a4-115">Application</span></span>                            | <span data-ttu-id="1d3a4-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="1d3a4-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="1d3a4-117">\***重要提示：** 应用程序权限目前仅为个人预览版，不可公开使用。</span><span class="sxs-lookup"><span data-stu-id="1d3a4-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="1d3a4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d3a4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d3a4-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1d3a4-119">Optional query parameters</span></span>

<span data-ttu-id="1d3a4-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1d3a4-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1d3a4-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1d3a4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d3a4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d3a4-122">Request headers</span></span>

| <span data-ttu-id="1d3a4-123">名称</span><span class="sxs-lookup"><span data-stu-id="1d3a4-123">Name</span></span>      |<span data-ttu-id="1d3a4-124">说明</span><span class="sxs-lookup"><span data-stu-id="1d3a4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1d3a4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d3a4-125">Authorization</span></span> | <span data-ttu-id="1d3a4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1d3a4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1d3a4-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="1d3a4-128">Content-type</span></span> | <span data-ttu-id="1d3a4-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1d3a4-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d3a4-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d3a4-131">Request body</span></span>
<span data-ttu-id="1d3a4-132">在请求正文中，提供新的 [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d3a4-132">In the request body, provide a JSON representation of a new [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1d3a4-133">响应</span><span class="sxs-lookup"><span data-stu-id="1d3a4-133">Response</span></span>

<span data-ttu-id="1d3a4-134">如果成功，此方法在响应正文中返回 响应代码和创建的 `200 OK` [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1d3a4-134">If successful, this method returns a `200 OK` response code and the created [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1d3a4-135">示例</span><span class="sxs-lookup"><span data-stu-id="1d3a4-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1d3a4-136">请求</span><span class="sxs-lookup"><span data-stu-id="1d3a4-136">Request</span></span>

<span data-ttu-id="1d3a4-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1d3a4-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/swapShiftsChangeRequests
Authorization: Bearer {token}
Content-type: application/json

{
  "senderShiftId": "5ad10161-6524-4c7c-9beb-4e8677ba2f6d",
  "senderMessage": "I can't make my shift, any chance we can swap?",
  "recipientUserId": "567c8ea5-9e32-422a-a663-8270201699cd",
  "recipientShiftId": "e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c"
}
```

### <a name="response"></a><span data-ttu-id="1d3a4-138">响应</span><span class="sxs-lookup"><span data-stu-id="1d3a4-138">Response</span></span>

<span data-ttu-id="1d3a4-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1d3a4-139">The following is an example of the response.</span></span>

> <span data-ttu-id="1d3a4-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1d3a4-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


