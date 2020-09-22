---
title: 创建 openShiftChangeRequest
description: 创建 openShiftChangeRequest 对象的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 04957803bd8c907bfad8fafb17d9c548e856e16c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071904"
---
# <a name="create-openshiftchangerequest"></a><span data-ttu-id="6e32f-103">创建 openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="6e32f-103">Create openShiftChangeRequest</span></span>

<span data-ttu-id="6e32f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e32f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e32f-105">创建 [openShiftChangeRequest](../resources/openshiftchangerequest.md) 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="6e32f-105">Create instance of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6e32f-106">权限</span><span class="sxs-lookup"><span data-stu-id="6e32f-106">Permissions</span></span>

<span data-ttu-id="6e32f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e32f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e32f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e32f-109">Permission type</span></span>                        | <span data-ttu-id="6e32f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e32f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6e32f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e32f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e32f-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e32f-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="6e32f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e32f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e32f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e32f-114">Not supported.</span></span> |
| <span data-ttu-id="6e32f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e32f-115">Application</span></span>                            | <span data-ttu-id="6e32f-116">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="6e32f-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="6e32f-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="6e32f-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="6e32f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e32f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e32f-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6e32f-119">Optional query parameters</span></span>

<span data-ttu-id="6e32f-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6e32f-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6e32f-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6e32f-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e32f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e32f-122">Request headers</span></span>

| <span data-ttu-id="6e32f-123">名称</span><span class="sxs-lookup"><span data-stu-id="6e32f-123">Name</span></span>      |<span data-ttu-id="6e32f-124">说明</span><span class="sxs-lookup"><span data-stu-id="6e32f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6e32f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e32f-125">Authorization</span></span> | <span data-ttu-id="6e32f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e32f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6e32f-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="6e32f-128">Content-type</span></span> | <span data-ttu-id="6e32f-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6e32f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e32f-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e32f-131">Request body</span></span>
<span data-ttu-id="6e32f-132">在请求正文中，提供新的 [openShiftChangeRequest](../resources/openshiftchangerequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e32f-132">In the request body, provide a JSON representation of a new [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6e32f-133">响应</span><span class="sxs-lookup"><span data-stu-id="6e32f-133">Response</span></span>

<span data-ttu-id="6e32f-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和创建的 [openShiftChangeRequest](../resources/openshiftchangerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6e32f-134">If successful, this method returns a `200 OK` response code and the created [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e32f-135">示例</span><span class="sxs-lookup"><span data-stu-id="6e32f-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e32f-136">请求</span><span class="sxs-lookup"><span data-stu-id="6e32f-136">Request</span></span>

<span data-ttu-id="6e32f-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e32f-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/openShiftsChangeRequests
Authorization: Bearer {token}
Content-type: application/json
Content-length: 244

{
  "senderMessage": "Can I take this shift?",
  "openShiftId": "577b75d2-a927-48c0-a5d1-dc984894e7b8"
}
```

### <a name="response"></a><span data-ttu-id="6e32f-138">响应</span><span class="sxs-lookup"><span data-stu-id="6e32f-138">Response</span></span>

<span data-ttu-id="6e32f-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6e32f-139">The following is an example of the response.</span></span>

> <span data-ttu-id="6e32f-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6e32f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09",
  "openShiftId": "577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "assignedTo": "manager",
  "state": "pending",
  "senderUserId": "3fe0bc21-1398-4fd9-9713-52511b434c1e",
  "senderDateTime": "2019-05-01T10:00:00Z",
  "senderMessage": "Can I take this shift?",
  "managerUserId": null,
  "managerActionDateTime": null,
  "managerActionMessage": null,
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create openShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


