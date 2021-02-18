---
title: 创建 openShiftChangeRequest
description: 创建 openShiftChangeRequest 对象的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e861dc2e5da1c175f419fdf47c76a4fac3b877bd
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292180"
---
# <a name="create-openshiftchangerequest"></a><span data-ttu-id="044c7-103">创建 openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="044c7-103">Create openShiftChangeRequest</span></span>

<span data-ttu-id="044c7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="044c7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="044c7-105">创建 [openShiftChangeRequest 对象](../resources/openshiftchangerequest.md) 的实例。</span><span class="sxs-lookup"><span data-stu-id="044c7-105">Create instance of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="044c7-106">权限</span><span class="sxs-lookup"><span data-stu-id="044c7-106">Permissions</span></span>

<span data-ttu-id="044c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="044c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="044c7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="044c7-109">Permission type</span></span>                        | <span data-ttu-id="044c7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="044c7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="044c7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="044c7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="044c7-112">Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="044c7-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="044c7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="044c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="044c7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="044c7-114">Not supported.</span></span> |
| <span data-ttu-id="044c7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="044c7-115">Application</span></span>                            | <span data-ttu-id="044c7-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="044c7-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="044c7-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="044c7-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="044c7-118">全局管理员可以访问不是其成员组的组。</span><span class="sxs-lookup"><span data-stu-id="044c7-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="044c7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="044c7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="044c7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="044c7-120">Request headers</span></span>

| <span data-ttu-id="044c7-121">名称</span><span class="sxs-lookup"><span data-stu-id="044c7-121">Name</span></span>      |<span data-ttu-id="044c7-122">说明</span><span class="sxs-lookup"><span data-stu-id="044c7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="044c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="044c7-123">Authorization</span></span> | <span data-ttu-id="044c7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="044c7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="044c7-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="044c7-126">Content-type</span></span> | <span data-ttu-id="044c7-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="044c7-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="044c7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="044c7-129">Request body</span></span>
<span data-ttu-id="044c7-130">在请求正文中，提供新 [openShiftChangeRequest](../resources/openshiftchangerequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="044c7-130">In the request body, provide a JSON representation of a new [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="044c7-131">响应</span><span class="sxs-lookup"><span data-stu-id="044c7-131">Response</span></span>

<span data-ttu-id="044c7-132">如果成功，此方法在响应正文中返回响应代码和创建的 `200 OK` [openShiftChangeRequest](../resources/openshiftchangerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="044c7-132">If successful, this method returns a `200 OK` response code and the created [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="044c7-133">示例</span><span class="sxs-lookup"><span data-stu-id="044c7-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="044c7-134">请求</span><span class="sxs-lookup"><span data-stu-id="044c7-134">Request</span></span>

<span data-ttu-id="044c7-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="044c7-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/openShiftChangeRequests
Authorization: Bearer {token}
Content-type: application/json
Content-length: 244

{
  "senderMessage": "Can I take this shift?",
  "openShiftId": "577b75d2-a927-48c0-a5d1-dc984894e7b8"
}
```

### <a name="response"></a><span data-ttu-id="044c7-136">响应</span><span class="sxs-lookup"><span data-stu-id="044c7-136">Response</span></span>

<span data-ttu-id="044c7-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="044c7-137">The following is an example of the response.</span></span>

> <span data-ttu-id="044c7-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="044c7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

