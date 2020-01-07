---
title: 创建 openShiftChangeRequest
description: 创建 openShiftChangeRequest 对象的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fb37f5c65ba04547aebd273df8ada78271a68108
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952207"
---
# <a name="create-openshiftchangerequest"></a><span data-ttu-id="f23c3-103">创建 openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="f23c3-103">Create openShiftChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f23c3-104">创建[openShiftChangeRequest](../resources/openshiftchangerequest.md)对象的实例。</span><span class="sxs-lookup"><span data-stu-id="f23c3-104">Create instance of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f23c3-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="f23c3-105">Permissions</span></span>

<span data-ttu-id="f23c3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f23c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f23c3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f23c3-108">Permission type</span></span>                        | <span data-ttu-id="f23c3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f23c3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f23c3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f23c3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f23c3-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f23c3-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="f23c3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f23c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f23c3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f23c3-113">Not supported.</span></span> |
| <span data-ttu-id="f23c3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f23c3-114">Application</span></span>                            | <span data-ttu-id="f23c3-115">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="f23c3-115">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="f23c3-116">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="f23c3-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="f23c3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f23c3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f23c3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f23c3-118">Optional query parameters</span></span>

<span data-ttu-id="f23c3-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f23c3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f23c3-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f23c3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f23c3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f23c3-121">Request headers</span></span>

| <span data-ttu-id="f23c3-122">名称</span><span class="sxs-lookup"><span data-stu-id="f23c3-122">Name</span></span>      |<span data-ttu-id="f23c3-123">说明</span><span class="sxs-lookup"><span data-stu-id="f23c3-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f23c3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f23c3-124">Authorization</span></span> | <span data-ttu-id="f23c3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f23c3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f23c3-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="f23c3-127">Content-type</span></span> | <span data-ttu-id="f23c3-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f23c3-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f23c3-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f23c3-130">Request body</span></span>
<span data-ttu-id="f23c3-131">在请求正文中，提供新的[openShiftChangeRequest](../resources/openshiftchangerequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f23c3-131">In the request body, provide a JSON representation of a new [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f23c3-132">响应</span><span class="sxs-lookup"><span data-stu-id="f23c3-132">Response</span></span>

<span data-ttu-id="f23c3-133">如果成功，此方法在响应`200 OK`正文中返回响应代码和创建的[openShiftChangeRequest](../resources/openshiftchangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f23c3-133">If successful, this method returns a `200 OK` response code and the created [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f23c3-134">示例</span><span class="sxs-lookup"><span data-stu-id="f23c3-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f23c3-135">请求</span><span class="sxs-lookup"><span data-stu-id="f23c3-135">Request</span></span>

<span data-ttu-id="f23c3-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f23c3-136">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f23c3-137">响应</span><span class="sxs-lookup"><span data-stu-id="f23c3-137">Response</span></span>

<span data-ttu-id="f23c3-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f23c3-138">The following is an example of the response.</span></span>

> <span data-ttu-id="f23c3-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f23c3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
