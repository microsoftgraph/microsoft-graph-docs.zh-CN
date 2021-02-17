---
title: 创建 plannerRoster
description: 创建新的 plannerRoster 对象。
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 153a88951943ce1a66d73ee26be289eaae7631f0
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272004"
---
# <a name="create-plannerroster"></a><span data-ttu-id="59055-103">创建 plannerRoster</span><span class="sxs-lookup"><span data-stu-id="59055-103">Create plannerRoster</span></span>
<span data-ttu-id="59055-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59055-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59055-105">创建新的 [plannerRoster](../resources/plannerroster.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59055-105">Create a new [plannerRoster](../resources/plannerroster.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="59055-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="59055-106">Permissions</span></span>
<span data-ttu-id="59055-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59055-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59055-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="59055-109">Permission type</span></span>|<span data-ttu-id="59055-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59055-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59055-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59055-111">Delegated (work or school account)</span></span>|<span data-ttu-id="59055-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59055-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="59055-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59055-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59055-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="59055-114">Not supported.</span></span>|
|<span data-ttu-id="59055-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="59055-115">Application</span></span>|<span data-ttu-id="59055-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="59055-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59055-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59055-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /planner/rosters
```

## <a name="request-headers"></a><span data-ttu-id="59055-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="59055-118">Request headers</span></span>
|<span data-ttu-id="59055-119">名称</span><span class="sxs-lookup"><span data-stu-id="59055-119">Name</span></span>|<span data-ttu-id="59055-120">说明</span><span class="sxs-lookup"><span data-stu-id="59055-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="59055-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="59055-121">Authorization</span></span>|<span data-ttu-id="59055-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59055-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="59055-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59055-124">Content-Type</span></span>|<span data-ttu-id="59055-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="59055-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59055-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="59055-127">Request body</span></span>
<span data-ttu-id="59055-128">在请求正文中，提供 [plannerRoster](../resources/plannerroster.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59055-128">In the request body, supply a JSON representation of the [plannerRoster](../resources/plannerroster.md) object.</span></span>

<span data-ttu-id="59055-129">plannerRoster 上没有可 [写属性](../resources/plannerroster.md)。</span><span class="sxs-lookup"><span data-stu-id="59055-129">There are no writable properties on [plannerRoster](../resources/plannerroster.md).</span></span>

## <a name="response"></a><span data-ttu-id="59055-130">响应</span><span class="sxs-lookup"><span data-stu-id="59055-130">Response</span></span>

<span data-ttu-id="59055-131">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [plannerRoster](../resources/plannerroster.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59055-131">If successful, this method returns a `201 Created` response code and a [plannerRoster](../resources/plannerroster.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="59055-132">示例</span><span class="sxs-lookup"><span data-stu-id="59055-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="59055-133">请求</span><span class="sxs-lookup"><span data-stu-id="59055-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="59055-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="59055-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerroster_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/planner/rosters
Content-Type: application/json
Content-length: 55

{
  "@odata.type": "#microsoft.graph.plannerRoster"
}
```
# <a name="c"></a>[<span data-ttu-id="59055-135">C#</span><span class="sxs-lookup"><span data-stu-id="59055-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerroster-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59055-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59055-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerroster-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59055-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59055-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerroster-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59055-138">Java</span><span class="sxs-lookup"><span data-stu-id="59055-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerroster-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="59055-139">响应</span><span class="sxs-lookup"><span data-stu-id="59055-139">Response</span></span>
<span data-ttu-id="59055-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="59055-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerRoster"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.plannerRoster",
  "id": "6519868f-868f-6519-8f86-19658f861965"
}
```

