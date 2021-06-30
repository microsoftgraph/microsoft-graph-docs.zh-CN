---
title: 删除团队合作标记
description: 删除团队合作标记对象。
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 169879fbc3bcd121f5edf270d90f4666a15a93ef
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210215"
---
# <a name="delete-teamworktag"></a><span data-ttu-id="14a63-103">删除团队合作标记</span><span class="sxs-lookup"><span data-stu-id="14a63-103">Delete teamworkTag</span></span>
<span data-ttu-id="14a63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14a63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14a63-105">删除 [tag](../resources/teamworktag.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14a63-105">Delete a [tag](../resources/teamworktag.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="14a63-106">权限</span><span class="sxs-lookup"><span data-stu-id="14a63-106">Permissions</span></span>
<span data-ttu-id="14a63-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14a63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14a63-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="14a63-109">Permission type</span></span>|<span data-ttu-id="14a63-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="14a63-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14a63-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14a63-111">Delegated (work or school account)</span></span>|<span data-ttu-id="14a63-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="14a63-112">Not supported.</span></span>|
|<span data-ttu-id="14a63-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14a63-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14a63-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="14a63-114">Not supported.</span></span>|
|<span data-ttu-id="14a63-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="14a63-115">Application</span></span>|<span data-ttu-id="14a63-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a63-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14a63-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14a63-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="request-headers"></a><span data-ttu-id="14a63-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="14a63-118">Request headers</span></span>
|<span data-ttu-id="14a63-119">名称</span><span class="sxs-lookup"><span data-stu-id="14a63-119">Name</span></span>|<span data-ttu-id="14a63-120">说明</span><span class="sxs-lookup"><span data-stu-id="14a63-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="14a63-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="14a63-121">Authorization</span></span>|<span data-ttu-id="14a63-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14a63-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="14a63-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="14a63-124">Request body</span></span>
<span data-ttu-id="14a63-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="14a63-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14a63-126">响应</span><span class="sxs-lookup"><span data-stu-id="14a63-126">Response</span></span>

<span data-ttu-id="14a63-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="14a63-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="14a63-128">示例</span><span class="sxs-lookup"><span data-stu-id="14a63-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14a63-129">请求</span><span class="sxs-lookup"><span data-stu-id="14a63-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="14a63-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="14a63-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamworktag"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==
```
# <a name="c"></a>[<span data-ttu-id="14a63-131">C#</span><span class="sxs-lookup"><span data-stu-id="14a63-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamworktag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14a63-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14a63-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamworktag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14a63-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14a63-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamworktag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14a63-134">Java</span><span class="sxs-lookup"><span data-stu-id="14a63-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamworktag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="14a63-135">响应</span><span class="sxs-lookup"><span data-stu-id="14a63-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

