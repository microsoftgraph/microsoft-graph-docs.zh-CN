---
title: 创建 plannerPlan
description: 使用此 API 新建 **plannerPlan**。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 1bb26d2858cf3b37ca6d61095eedca5ec8a4294d
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473631"
---
# <a name="create-plannerplan"></a><span data-ttu-id="36df6-103">创建 plannerPlan</span><span class="sxs-lookup"><span data-stu-id="36df6-103">Create plannerPlan</span></span>

<span data-ttu-id="36df6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36df6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36df6-105">使用此 API 新建 **plannerPlan**。</span><span class="sxs-lookup"><span data-stu-id="36df6-105">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="36df6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="36df6-106">Permissions</span></span>

<span data-ttu-id="36df6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36df6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36df6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="36df6-109">Permission type</span></span>                        | <span data-ttu-id="36df6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36df6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="36df6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36df6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="36df6-112">Tasks.ReadWrite、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36df6-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="36df6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36df6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36df6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="36df6-114">Not supported.</span></span>                              |
| <span data-ttu-id="36df6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="36df6-115">Application</span></span>                            | <span data-ttu-id="36df6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="36df6-116">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="36df6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36df6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="36df6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="36df6-118">Request headers</span></span>

| <span data-ttu-id="36df6-119">名称</span><span class="sxs-lookup"><span data-stu-id="36df6-119">Name</span></span>          | <span data-ttu-id="36df6-120">说明</span><span class="sxs-lookup"><span data-stu-id="36df6-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="36df6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="36df6-121">Authorization</span></span> | <span data-ttu-id="36df6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36df6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36df6-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="36df6-124">Request body</span></span>

<span data-ttu-id="36df6-p103">在请求正文中，提供 [plannerPlan](../resources/plannerplan.md) 对象的 JSON 表示形式。**plannerPlan** 所有者属性必须设为 [组](../resources/group.md)对象的 id。</span><span class="sxs-lookup"><span data-stu-id="36df6-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="36df6-127">**注意：** 正在创建计划的用户必须是拥有该计划的组的成员。</span><span class="sxs-lookup"><span data-stu-id="36df6-127">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="36df6-128">使用“[创建组](../api/group-post-groups.md)”创建新组时，系统不会将你添加为组成员。</span><span class="sxs-lookup"><span data-stu-id="36df6-128">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="36df6-129">创建组后，使用“[组帖子成员](../api/group-post-members.md)”将自己添加为成员。</span><span class="sxs-lookup"><span data-stu-id="36df6-129">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>


## <a name="response"></a><span data-ttu-id="36df6-130">响应</span><span class="sxs-lookup"><span data-stu-id="36df6-130">Response</span></span>

<span data-ttu-id="36df6-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [plannerPlan](../resources/plannerplan.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36df6-131">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="36df6-p105">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法的处理最常见的错误为 400、403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="36df6-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="36df6-135">示例</span><span class="sxs-lookup"><span data-stu-id="36df6-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="36df6-136">请求</span><span class="sxs-lookup"><span data-stu-id="36df6-136">Request</span></span>

<span data-ttu-id="36df6-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36df6-137">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36df6-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="36df6-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
``` http
POST https://graph.microsoft.com/v1.0/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```
# <a name="c"></a>[<span data-ttu-id="36df6-139">C#</span><span class="sxs-lookup"><span data-stu-id="36df6-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerplan-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36df6-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36df6-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerplan-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36df6-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36df6-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerplan-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36df6-142">Java</span><span class="sxs-lookup"><span data-stu-id="36df6-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerplan-from-planner-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="36df6-143">在请求正文中，提供 [plannerPlan](../resources/plannerplan.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36df6-143">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="36df6-144">响应</span><span class="sxs-lookup"><span data-stu-id="36df6-144">Response</span></span>

<span data-ttu-id="36df6-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36df6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

