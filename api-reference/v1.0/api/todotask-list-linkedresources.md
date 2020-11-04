---
title: 列出 linkedResources
description: 从 linkedResources 导航属性中获取 linkedResources。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: aa016742bad1535332ee9e5d78585467fc7a6af0
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904355"
---
# <a name="list-linkedresources"></a><span data-ttu-id="c3b36-103">列出 linkedResources</span><span class="sxs-lookup"><span data-stu-id="c3b36-103">List linkedResources</span></span>
<span data-ttu-id="c3b36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3b36-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c3b36-105">获取合作伙伴应用程序中的一个或多个项目的信息，基于创建的指定 [任务](../resources/todotask.md) 。</span><span class="sxs-lookup"><span data-stu-id="c3b36-105">Get information of one or more items in a partner application, based on which a specified [task](../resources/todotask.md) was created.</span></span> <span data-ttu-id="c3b36-106">信息在每个项目的 [linkedResource](../resources/linkedresource.md) 对象中表示。</span><span class="sxs-lookup"><span data-stu-id="c3b36-106">The information is represented in a [linkedResource](../resources/linkedresource.md) object for each item.</span></span> <span data-ttu-id="c3b36-107">它包括合作伙伴应用程序中的项目的外部 ID，如果适用，还包括指向应用程序中该项目的深层链接。</span><span class="sxs-lookup"><span data-stu-id="c3b36-107">It includes an external ID for the item in the partner application, and if applicable, a deep link to that item in the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3b36-108">权限</span><span class="sxs-lookup"><span data-stu-id="c3b36-108">Permissions</span></span>
<span data-ttu-id="c3b36-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3b36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3b36-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3b36-111">Permission type</span></span>|<span data-ttu-id="c3b36-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c3b36-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3b36-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3b36-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3b36-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3b36-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="c3b36-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3b36-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3b36-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3b36-116">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="c3b36-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3b36-117">Application</span></span>|<span data-ttu-id="c3b36-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3b36-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3b36-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3b36-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3b36-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c3b36-120">Optional query parameters</span></span>
<span data-ttu-id="c3b36-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c3b36-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c3b36-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c3b36-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3b36-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3b36-123">Request headers</span></span>
|<span data-ttu-id="c3b36-124">名称</span><span class="sxs-lookup"><span data-stu-id="c3b36-124">Name</span></span>|<span data-ttu-id="c3b36-125">说明</span><span class="sxs-lookup"><span data-stu-id="c3b36-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c3b36-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3b36-126">Authorization</span></span>|<span data-ttu-id="c3b36-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c3b36-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3b36-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3b36-129">Request body</span></span>
<span data-ttu-id="c3b36-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c3b36-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3b36-131">响应</span><span class="sxs-lookup"><span data-stu-id="c3b36-131">Response</span></span>

<span data-ttu-id="c3b36-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [linkedResource](../resources/linkedresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c3b36-132">If successful, this method returns a `200 OK` response code and a collection of [linkedResource](../resources/linkedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3b36-133">示例</span><span class="sxs-lookup"><span data-stu-id="c3b36-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c3b36-134">请求</span><span class="sxs-lookup"><span data-stu-id="c3b36-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c3b36-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3b36-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
```
# <a name="c"></a>[<span data-ttu-id="c3b36-136">C#</span><span class="sxs-lookup"><span data-stu-id="c3b36-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3b36-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3b36-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3b36-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3b36-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3b36-139">Java</span><span class="sxs-lookup"><span data-stu-id="c3b36-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-linkedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c3b36-140">响应</span><span class="sxs-lookup"><span data-stu-id="c3b36-140">Response</span></span>
<span data-ttu-id="c3b36-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c3b36-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.linkedResource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.linkedResource",
      "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
      "webUrl": "http:://microsoft.com",
      "applicationName": "Microsoft",
      "displayName": "Microsoft",
      "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
    }
  ]
}
```



