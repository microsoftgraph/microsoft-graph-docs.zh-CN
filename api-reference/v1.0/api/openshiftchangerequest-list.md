---
title: 列出 openShiftChangeRequests
description: 检索团队中的 openShiftChangeRequest 对象的列表。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4c203f9fab489844452eeb6cc341b18af7898eac
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44153779"
---
# <a name="list-openshiftchangerequests"></a><span data-ttu-id="099fd-103">列出 openShiftChangeRequests</span><span class="sxs-lookup"><span data-stu-id="099fd-103">List openShiftChangeRequests</span></span>

<span data-ttu-id="099fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="099fd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="099fd-105">检索团队中的[openShiftChangeRequest](../resources/openshiftchangerequest.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="099fd-105">Retrieve a list of [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="099fd-106">权限</span><span class="sxs-lookup"><span data-stu-id="099fd-106">Permissions</span></span>

<span data-ttu-id="099fd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="099fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="099fd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="099fd-109">Permission type</span></span>                        | <span data-ttu-id="099fd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="099fd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="099fd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="099fd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="099fd-112">请参阅 all、Group、Group. all、Schedule、Group、Group。所有</span><span class="sxs-lookup"><span data-stu-id="099fd-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="099fd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="099fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="099fd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="099fd-114">Not supported.</span></span> |
| <span data-ttu-id="099fd-115">Application</span><span class="sxs-lookup"><span data-stu-id="099fd-115">Application</span></span>                            | <span data-ttu-id="099fd-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="099fd-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="099fd-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="099fd-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="099fd-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="099fd-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="099fd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="099fd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="099fd-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="099fd-120">Optional query parameters</span></span>

<span data-ttu-id="099fd-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="099fd-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="099fd-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="099fd-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="099fd-123">请求头</span><span class="sxs-lookup"><span data-stu-id="099fd-123">Request headers</span></span>

| <span data-ttu-id="099fd-124">名称</span><span class="sxs-lookup"><span data-stu-id="099fd-124">Name</span></span>      |<span data-ttu-id="099fd-125">说明</span><span class="sxs-lookup"><span data-stu-id="099fd-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="099fd-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="099fd-126">Authorization</span></span> | <span data-ttu-id="099fd-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="099fd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="099fd-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="099fd-129">Request body</span></span>

<span data-ttu-id="099fd-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="099fd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="099fd-131">响应</span><span class="sxs-lookup"><span data-stu-id="099fd-131">Response</span></span>

<span data-ttu-id="099fd-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[openShiftChangeRequest](../resources/openshiftchangerequest.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="099fd-132">If successful, this method returns a `200 OK` response code and the list of [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="099fd-133">示例</span><span class="sxs-lookup"><span data-stu-id="099fd-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="099fd-134">请求</span><span class="sxs-lookup"><span data-stu-id="099fd-134">Request</span></span>

<span data-ttu-id="099fd-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="099fd-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftsChangeRequests
```

### <a name="response"></a><span data-ttu-id="099fd-136">响应</span><span class="sxs-lookup"><span data-stu-id="099fd-136">Response</span></span>

<span data-ttu-id="099fd-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="099fd-137">The following is an example of the response.</span></span>

> <span data-ttu-id="099fd-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="099fd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [{
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
    }]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List openShiftChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
