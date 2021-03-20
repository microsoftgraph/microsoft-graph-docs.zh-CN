---
title: 列出用户使用情况Rights
description: 检索用户的 usageRights 对象列表。
author: jeeshnair
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 253dbe479c4bd0e60798da2d7e21b78965a1e356
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942017"
---
# <a name="list-user-usagerights"></a><span data-ttu-id="5bf37-103">列出用户使用情况Rights</span><span class="sxs-lookup"><span data-stu-id="5bf37-103">List user usageRights</span></span>
<span data-ttu-id="5bf37-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bf37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bf37-105">检索给定用户的 [usageRight](../resources/usageright.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="5bf37-105">Retrieve a list of [usageRight](../resources/usageright.md) objects for a given user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bf37-106">权限</span><span class="sxs-lookup"><span data-stu-id="5bf37-106">Permissions</span></span>
<span data-ttu-id="5bf37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5bf37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bf37-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5bf37-109">Permission type</span></span>|<span data-ttu-id="5bf37-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5bf37-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bf37-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5bf37-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5bf37-112">User.Read、User.ReadWrite、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bf37-112">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="5bf37-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5bf37-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bf37-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bf37-114">Not supported.</span></span>|
|<span data-ttu-id="5bf37-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5bf37-115">Application</span></span>|<span data-ttu-id="5bf37-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bf37-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bf37-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5bf37-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{userId}/usageRights
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5bf37-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5bf37-118">Optional query parameters</span></span>
<span data-ttu-id="5bf37-119">此 API 支持 $filter [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5bf37-119">This API supports the $filter [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="5bf37-120">支持以下$filter模式：</span><span class="sxs-lookup"><span data-stu-id="5bf37-120">The following patterns of $filter are supported:</span></span>

- <span data-ttu-id="5bf37-121">$filter = state eq 'value'</span><span class="sxs-lookup"><span data-stu-id="5bf37-121">$filter = state eq 'value'</span></span>
- <span data-ttu-id="5bf37-122">$filter = serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="5bf37-122">$filter = serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="5bf37-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="5bf37-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="5bf37-124">$filter = ( value1、value2") </span><span class="sxs-lookup"><span data-stu-id="5bf37-124">$filter = state in ('value1', 'value2')</span></span>
- <span data-ttu-id="5bf37-125">$filter =serviceIdentifier in ('value1'， 'value2') </span><span class="sxs-lookup"><span data-stu-id="5bf37-125">$filter = serviceIdentifier in ('value1', 'value2')</span></span>
- <span data-ttu-id="5bf37-126">$filter = ( value1、value2") 和 serviceIdentifier 中的 state ( value1"，"value2") </span><span class="sxs-lookup"><span data-stu-id="5bf37-126">$filter = state in ('value1', 'value2') and serviceIdentifier in ('value1', 'value2')</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bf37-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="5bf37-127">Request headers</span></span>
|<span data-ttu-id="5bf37-128">名称</span><span class="sxs-lookup"><span data-stu-id="5bf37-128">Name</span></span>|<span data-ttu-id="5bf37-129">说明</span><span class="sxs-lookup"><span data-stu-id="5bf37-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5bf37-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bf37-130">Authorization</span></span>|<span data-ttu-id="5bf37-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5bf37-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5bf37-133">odata.maxpagesize</span><span class="sxs-lookup"><span data-stu-id="5bf37-133">odata.maxpagesize</span></span>|<span data-ttu-id="5bf37-134">设置每个结果页的最大大小。</span><span class="sxs-lookup"><span data-stu-id="5bf37-134">Set the max result page size pereference.</span></span> <span data-ttu-id="5bf37-135">可选。</span><span class="sxs-lookup"><span data-stu-id="5bf37-135">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bf37-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="5bf37-136">Request body</span></span>
<span data-ttu-id="5bf37-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5bf37-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bf37-138">响应</span><span class="sxs-lookup"><span data-stu-id="5bf37-138">Response</span></span>
<span data-ttu-id="5bf37-139">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [usageRight](../resources/usageright.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5bf37-139">If successful, this method returns a `200 OK` response code and a collection of [usageRight](../resources/usageright.md) objects in the response body.</span></span>

<span data-ttu-id="5bf37-140">此外，如果响应中有更多的页面，@odata.nextLink。</span><span class="sxs-lookup"><span data-stu-id="5bf37-140">Additionally, if there are more pages in the response an @odata.nextLink is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="5bf37-141">示例</span><span class="sxs-lookup"><span data-stu-id="5bf37-141">Examples</span></span>

### <a name="example-1-get-all-usage-rights-for-a-user"></a><span data-ttu-id="5bf37-142">示例 1：获取用户的所有使用权限</span><span class="sxs-lookup"><span data-stu-id="5bf37-142">Example 1: Get all usage rights for a user</span></span>

#### <a name="request"></a><span data-ttu-id="5bf37-143">请求</span><span class="sxs-lookup"><span data-stu-id="5bf37-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5bf37-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bf37-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright_3"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{userId}/usageRights
```
# <a name="c"></a>[<span data-ttu-id="5bf37-145">C#</span><span class="sxs-lookup"><span data-stu-id="5bf37-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bf37-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bf37-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bf37-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bf37-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5bf37-148">Java</span><span class="sxs-lookup"><span data-stu-id="5bf37-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5bf37-149">响应</span><span class="sxs-lookup"><span data-stu-id="5bf37-149">Response</span></span>
><span data-ttu-id="5bf37-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5bf37-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.usageRight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64952b80-51fd-4378-9ba5-589a840afb80')/usageRights",
  "@odata.nextLink": "https://graph.microsoft.com/beta/users/64952b80-51fd-4378-9ba5-589a840afb80/usageRights?$skiptoken=W4diD29cGKX1bX",
  "value": [
    {
      "id": "c2e034cb-3cbc-41be-a496-bfcd031e4cfc",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "mscrm.f6d23ec7-255c-4bd8-8c99-dc041d5cb8b3.517f7ddd-df45-4f1c-83ec-a081a047f546",
      "state": "active"
    }
  ]
}
```

### <a name="example-2-get-usage-rights-for-a-user-with-specific-service-identifiers-and-states"></a><span data-ttu-id="5bf37-151">示例 2：获取具有特定服务标识符和状态的用户的使用权限</span><span class="sxs-lookup"><span data-stu-id="5bf37-151">Example 2: Get usage rights for a user with specific service identifiers and states</span></span>

#### <a name="request"></a><span data-ttu-id="5bf37-152">请求</span><span class="sxs-lookup"><span data-stu-id="5bf37-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5bf37-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bf37-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright_4"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{userId}/usageRights?$filter=state in ('active', 'suspended') and serviceIdentifier in ('ABCD')
```
# <a name="c"></a>[<span data-ttu-id="5bf37-154">C#</span><span class="sxs-lookup"><span data-stu-id="5bf37-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bf37-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bf37-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bf37-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bf37-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5bf37-157">Java</span><span class="sxs-lookup"><span data-stu-id="5bf37-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5bf37-158">响应</span><span class="sxs-lookup"><span data-stu-id="5bf37-158">Response</span></span>
><span data-ttu-id="5bf37-159">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5bf37-159">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.usageRight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64952b80-51fd-4378-9ba5-589a840afb80')/usageRights",
  "value": [
    {
      "id": "505261eb-b4ee-421c-8206-05529ae2c150",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "ABCD",
      "state": "active"
    }
  ]
}
```
