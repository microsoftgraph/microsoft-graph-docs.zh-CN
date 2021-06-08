---
title: user： exportPersonalData
description: 提交由公司管理员提出的数据策略操作请求，以导出组织用户的数据。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: c829ead807e87c3a11289beeb5edb122cce40ac2
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786094"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="870a3-103">user： exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="870a3-103">user: exportPersonalData</span></span>

<span data-ttu-id="870a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="870a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="870a3-105">提交公司管理员发出的数据策略操作请求，以导出组织用户的数据。</span><span class="sxs-lookup"><span data-stu-id="870a3-105">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="870a3-106">权限</span><span class="sxs-lookup"><span data-stu-id="870a3-106">Permissions</span></span>
<span data-ttu-id="870a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="870a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="870a3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="870a3-109">Permission type</span></span>      | <span data-ttu-id="870a3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="870a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="870a3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="870a3-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="870a3-112">User.Export.All 和 User.Read.All</span><span class="sxs-lookup"><span data-stu-id="870a3-112">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="870a3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="870a3-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="870a3-114">不适用</span><span class="sxs-lookup"><span data-stu-id="870a3-114">Not applicable</span></span>  |
|<span data-ttu-id="870a3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="870a3-115">Application</span></span> | <span data-ttu-id="870a3-116">User.Export.All 和 User.Read.All</span><span class="sxs-lookup"><span data-stu-id="870a3-116">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="870a3-117">**注意：** 使用委派权限时，只有公司管理员才能执行导出。</span><span class="sxs-lookup"><span data-stu-id="870a3-117">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="870a3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="870a3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="870a3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="870a3-119">Request headers</span></span>
| <span data-ttu-id="870a3-120">名称</span><span class="sxs-lookup"><span data-stu-id="870a3-120">Name</span></span>       | <span data-ttu-id="870a3-121">说明</span><span class="sxs-lookup"><span data-stu-id="870a3-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="870a3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="870a3-122">Authorization</span></span>  | <span data-ttu-id="870a3-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="870a3-123">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="870a3-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="870a3-124">Request body</span></span>
<span data-ttu-id="870a3-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="870a3-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="870a3-126">参数</span><span class="sxs-lookup"><span data-stu-id="870a3-126">Parameter</span></span>    | <span data-ttu-id="870a3-127">类型</span><span class="sxs-lookup"><span data-stu-id="870a3-127">Type</span></span>   |<span data-ttu-id="870a3-128">说明</span><span class="sxs-lookup"><span data-stu-id="870a3-128">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="870a3-129">storageLocation</span><span class="sxs-lookup"><span data-stu-id="870a3-129">storageLocation</span></span>|<span data-ttu-id="870a3-130">String</span><span class="sxs-lookup"><span data-stu-id="870a3-130">String</span></span>|<span data-ttu-id="870a3-131">这是一个共享访问签名 (SAS) URL Azure 存储帐户，将数据导出到其中。</span><span class="sxs-lookup"><span data-stu-id="870a3-131">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="870a3-132">响应</span><span class="sxs-lookup"><span data-stu-id="870a3-132">Response</span></span>
<span data-ttu-id="870a3-133">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="870a3-133">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="870a3-134">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="870a3-134">It does not return anything in the response body.</span></span> <span data-ttu-id="870a3-135">该响应包含以下标头。</span><span class="sxs-lookup"><span data-stu-id="870a3-135">The response contains the following headers.</span></span>

| <span data-ttu-id="870a3-136">名称</span><span class="sxs-lookup"><span data-stu-id="870a3-136">Name</span></span>       | <span data-ttu-id="870a3-137">说明</span><span class="sxs-lookup"><span data-stu-id="870a3-137">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="870a3-138">Location</span><span class="sxs-lookup"><span data-stu-id="870a3-138">Location</span></span>  | <span data-ttu-id="870a3-139">检查请求状态的 URL。</span><span class="sxs-lookup"><span data-stu-id="870a3-139">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="870a3-140">Retry-After</span><span class="sxs-lookup"><span data-stu-id="870a3-140">Retry-After</span></span>  | <span data-ttu-id="870a3-141">时间段（以秒表示）。</span><span class="sxs-lookup"><span data-stu-id="870a3-141">Time period in seconds.</span></span> <span data-ttu-id="870a3-142">请求建立者应在提交检查状态的请求后等待此时间。</span><span class="sxs-lookup"><span data-stu-id="870a3-142">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="870a3-143">示例</span><span class="sxs-lookup"><span data-stu-id="870a3-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="870a3-144">请求</span><span class="sxs-lookup"><span data-stu-id="870a3-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="870a3-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="870a3-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
# <a name="c"></a>[<span data-ttu-id="870a3-146">C#</span><span class="sxs-lookup"><span data-stu-id="870a3-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-exportpersonaldata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="870a3-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="870a3-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-exportpersonaldata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="870a3-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="870a3-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-exportpersonaldata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="870a3-149">Java</span><span class="sxs-lookup"><span data-stu-id="870a3-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-exportpersonaldata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="870a3-150">响应</span><span class="sxs-lookup"><span data-stu-id="870a3-150">Response</span></span>

```http
{
  Location: https://graph.microsoft.com/beta/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


