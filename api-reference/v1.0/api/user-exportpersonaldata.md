---
title: '用户: exportPersonalData'
description: 提交数据策略操作请求, 由公司管理员进行导出以导出组织用户的数据。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a42a6f5ac10fdc84a3a66f6c5e0dd88228c20baf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373659"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="c9211-103">用户: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="c9211-103">user: exportPersonalData</span></span>

<span data-ttu-id="c9211-104">提交来自公司管理员或应用程序的数据策略操作请求, 以导出组织用户的数据。</span><span class="sxs-lookup"><span data-stu-id="c9211-104">Submit a data policy operation request from a company administrator or an application to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9211-105">权限</span><span class="sxs-lookup"><span data-stu-id="c9211-105">Permissions</span></span>
<span data-ttu-id="c9211-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9211-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9211-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9211-108">Permission type</span></span>      | <span data-ttu-id="c9211-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c9211-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9211-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9211-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c9211-111">将用户导出为 All、User、Read。 All</span><span class="sxs-lookup"><span data-stu-id="c9211-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="c9211-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9211-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c9211-113">不适用</span><span class="sxs-lookup"><span data-stu-id="c9211-113">Not applicable</span></span>  |
|<span data-ttu-id="c9211-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9211-114">Application</span></span> | <span data-ttu-id="c9211-115">将用户导出为 All、User、Read。 All</span><span class="sxs-lookup"><span data-stu-id="c9211-115">User.Export.All, User.Read.All</span></span> |

><span data-ttu-id="c9211-116">**注意:** 只有在使用委派权限时, 公司管理员才能执行导出。</span><span class="sxs-lookup"><span data-stu-id="c9211-116">**Note:** The export can only be performed by a company administrator when delegated permissions are used.</span></span>

## <a name="http-request"></a><span data-ttu-id="c9211-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9211-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="c9211-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9211-118">Request headers</span></span>
| <span data-ttu-id="c9211-119">名称</span><span class="sxs-lookup"><span data-stu-id="c9211-119">Name</span></span>       | <span data-ttu-id="c9211-120">说明</span><span class="sxs-lookup"><span data-stu-id="c9211-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c9211-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9211-121">Authorization</span></span>  | <span data-ttu-id="c9211-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="c9211-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9211-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9211-123">Request body</span></span>
<span data-ttu-id="c9211-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c9211-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c9211-125">参数</span><span class="sxs-lookup"><span data-stu-id="c9211-125">Parameter</span></span>    | <span data-ttu-id="c9211-126">类型</span><span class="sxs-lookup"><span data-stu-id="c9211-126">Type</span></span>   |<span data-ttu-id="c9211-127">说明</span><span class="sxs-lookup"><span data-stu-id="c9211-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9211-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="c9211-128">storageLocation</span></span>|<span data-ttu-id="c9211-129">String</span><span class="sxs-lookup"><span data-stu-id="c9211-129">String</span></span>|<span data-ttu-id="c9211-130">这是 Azure 存储帐户的共享访问签名 (SAS) URL, 应导出数据的位置。</span><span class="sxs-lookup"><span data-stu-id="c9211-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="c9211-131">响应</span><span class="sxs-lookup"><span data-stu-id="c9211-131">Response</span></span>
<span data-ttu-id="c9211-132">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c9211-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="c9211-133">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c9211-133">It does not return anything in the response body.</span></span> <span data-ttu-id="c9211-134">响应包含以下响应头。</span><span class="sxs-lookup"><span data-stu-id="c9211-134">The response contains the following response headers.</span></span>

| <span data-ttu-id="c9211-135">名称</span><span class="sxs-lookup"><span data-stu-id="c9211-135">Name</span></span>       | <span data-ttu-id="c9211-136">说明</span><span class="sxs-lookup"><span data-stu-id="c9211-136">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c9211-137">Location</span><span class="sxs-lookup"><span data-stu-id="c9211-137">Location</span></span>  | <span data-ttu-id="c9211-138">用于检查请求状态的 URL。</span><span class="sxs-lookup"><span data-stu-id="c9211-138">URL to check on the status of the request.</span></span> |
| <span data-ttu-id="c9211-139">重试-After</span><span class="sxs-lookup"><span data-stu-id="c9211-139">Retry-After</span></span>  | <span data-ttu-id="c9211-140">以秒为单位的时间段。</span><span class="sxs-lookup"><span data-stu-id="c9211-140">Time period in seconds.</span></span> <span data-ttu-id="c9211-141">在提交请求以检查状态后, 请求生成器应等待这长时间。</span><span class="sxs-lookup"><span data-stu-id="c9211-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |

## <a name="example"></a><span data-ttu-id="c9211-142">示例</span><span class="sxs-lookup"><span data-stu-id="c9211-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9211-143">请求</span><span class="sxs-lookup"><span data-stu-id="c9211-143">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c9211-144">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c9211-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9211-145">C#</span><span class="sxs-lookup"><span data-stu-id="c9211-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-exportpersonaldata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9211-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9211-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-exportpersonaldata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9211-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="c9211-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-exportpersonaldata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c9211-148">Java</span><span class="sxs-lookup"><span data-stu-id="c9211-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-exportpersonaldata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c9211-149">响应</span><span class="sxs-lookup"><span data-stu-id="c9211-149">Response</span></span>

```http
{
  Location: https://graph.microsoft.com/v1.0/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
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
