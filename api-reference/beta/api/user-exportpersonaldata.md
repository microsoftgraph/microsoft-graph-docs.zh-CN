---
title: 用户： exportPersonalData
description: 提交数据策略操作请求，由公司管理员进行导出以导出组织用户的数据。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 24262a733a4a8dcdc8724950b0c65bf31fdbc9a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067529"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="44a23-103">用户： exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="44a23-103">user: exportPersonalData</span></span>

<span data-ttu-id="44a23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44a23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44a23-105">提交公司管理员发出的数据策略操作请求，以导出组织用户的数据。</span><span class="sxs-lookup"><span data-stu-id="44a23-105">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="44a23-106">权限</span><span class="sxs-lookup"><span data-stu-id="44a23-106">Permissions</span></span>
<span data-ttu-id="44a23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44a23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44a23-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="44a23-109">Permission type</span></span>      | <span data-ttu-id="44a23-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44a23-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44a23-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44a23-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="44a23-112">Export. All 和 User. All</span><span class="sxs-lookup"><span data-stu-id="44a23-112">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="44a23-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44a23-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="44a23-114">不适用</span><span class="sxs-lookup"><span data-stu-id="44a23-114">Not applicable</span></span>  |
|<span data-ttu-id="44a23-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="44a23-115">Application</span></span> | <span data-ttu-id="44a23-116">Export. All 和 User. All</span><span class="sxs-lookup"><span data-stu-id="44a23-116">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="44a23-117">**注意：** 仅当使用委派的权限时，公司管理员才能执行导出。</span><span class="sxs-lookup"><span data-stu-id="44a23-117">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="44a23-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44a23-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="44a23-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="44a23-119">Request headers</span></span>
| <span data-ttu-id="44a23-120">名称</span><span class="sxs-lookup"><span data-stu-id="44a23-120">Name</span></span>       | <span data-ttu-id="44a23-121">说明</span><span class="sxs-lookup"><span data-stu-id="44a23-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="44a23-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="44a23-122">Authorization</span></span>  | <span data-ttu-id="44a23-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="44a23-123">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="44a23-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="44a23-124">Request body</span></span>
<span data-ttu-id="44a23-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="44a23-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="44a23-126">参数</span><span class="sxs-lookup"><span data-stu-id="44a23-126">Parameter</span></span>    | <span data-ttu-id="44a23-127">类型</span><span class="sxs-lookup"><span data-stu-id="44a23-127">Type</span></span>   |<span data-ttu-id="44a23-128">说明</span><span class="sxs-lookup"><span data-stu-id="44a23-128">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="44a23-129">storageLocation</span><span class="sxs-lookup"><span data-stu-id="44a23-129">storageLocation</span></span>|<span data-ttu-id="44a23-130">String</span><span class="sxs-lookup"><span data-stu-id="44a23-130">String</span></span>|<span data-ttu-id="44a23-131">这是 Azure 存储帐户 (SAS) URL 的共享访问签名，可将数据导出到其中。</span><span class="sxs-lookup"><span data-stu-id="44a23-131">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="44a23-132">响应</span><span class="sxs-lookup"><span data-stu-id="44a23-132">Response</span></span>
<span data-ttu-id="44a23-133">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="44a23-133">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="44a23-134">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="44a23-134">It does not return anything in the response body.</span></span> <span data-ttu-id="44a23-135">响应包含以下标头。</span><span class="sxs-lookup"><span data-stu-id="44a23-135">The response contains the following headers.</span></span>

| <span data-ttu-id="44a23-136">名称</span><span class="sxs-lookup"><span data-stu-id="44a23-136">Name</span></span>       | <span data-ttu-id="44a23-137">说明</span><span class="sxs-lookup"><span data-stu-id="44a23-137">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="44a23-138">Location</span><span class="sxs-lookup"><span data-stu-id="44a23-138">Location</span></span>  | <span data-ttu-id="44a23-139">用于检查请求状态的 URL。</span><span class="sxs-lookup"><span data-stu-id="44a23-139">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="44a23-140">重试-After</span><span class="sxs-lookup"><span data-stu-id="44a23-140">Retry-After</span></span>  | <span data-ttu-id="44a23-141">以秒为单位的时间段。</span><span class="sxs-lookup"><span data-stu-id="44a23-141">Time period in seconds.</span></span> <span data-ttu-id="44a23-142">在提交请求以检查状态后，请求生成器应等待这长时间。</span><span class="sxs-lookup"><span data-stu-id="44a23-142">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="44a23-143">示例</span><span class="sxs-lookup"><span data-stu-id="44a23-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44a23-144">请求</span><span class="sxs-lookup"><span data-stu-id="44a23-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="44a23-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="44a23-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="44a23-146">C#</span><span class="sxs-lookup"><span data-stu-id="44a23-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-exportpersonaldata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44a23-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44a23-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-exportpersonaldata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44a23-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44a23-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-exportpersonaldata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="44a23-149">响应</span><span class="sxs-lookup"><span data-stu-id="44a23-149">Response</span></span>

```http
{
  Location: https://graph.microsoft.com/beta/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
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


