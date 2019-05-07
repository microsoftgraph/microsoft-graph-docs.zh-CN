---
title: '用户: exportPersonalData'
description: 提交数据策略操作请求, 由公司管理员进行导出以导出组织用户的数据。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6feffbe56a6b4fe21c5a06eb89016f68d8f045ef
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602147"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="b0f34-103">用户: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="b0f34-103">user: exportPersonalData</span></span>

<span data-ttu-id="b0f34-104">提交来自公司管理员或应用程序的数据策略操作请求, 以导出组织用户的数据。</span><span class="sxs-lookup"><span data-stu-id="b0f34-104">Submit a data policy operation request from a company administrator or an application to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0f34-105">权限</span><span class="sxs-lookup"><span data-stu-id="b0f34-105">Permissions</span></span>
<span data-ttu-id="b0f34-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0f34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0f34-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0f34-108">Permission type</span></span>      | <span data-ttu-id="b0f34-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0f34-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0f34-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0f34-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b0f34-111">将用户导出为 All、User、Read。 All</span><span class="sxs-lookup"><span data-stu-id="b0f34-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="b0f34-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0f34-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b0f34-113">不适用</span><span class="sxs-lookup"><span data-stu-id="b0f34-113">Not applicable</span></span>  |
|<span data-ttu-id="b0f34-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0f34-114">Application</span></span> | <span data-ttu-id="b0f34-115">将用户导出为 All、User、Read。 All</span><span class="sxs-lookup"><span data-stu-id="b0f34-115">User.Export.All, User.Read.All</span></span> |

><span data-ttu-id="b0f34-116">**注意:** 只有在使用委派权限时, 公司管理员才能执行导出。</span><span class="sxs-lookup"><span data-stu-id="b0f34-116">**Note:** The export can only be performed by a company administrator when delegated permissions are used.</span></span>

## <a name="http-request"></a><span data-ttu-id="b0f34-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0f34-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="b0f34-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0f34-118">Request headers</span></span>
| <span data-ttu-id="b0f34-119">名称</span><span class="sxs-lookup"><span data-stu-id="b0f34-119">Name</span></span>       | <span data-ttu-id="b0f34-120">说明</span><span class="sxs-lookup"><span data-stu-id="b0f34-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b0f34-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0f34-121">Authorization</span></span>  | <span data-ttu-id="b0f34-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="b0f34-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0f34-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0f34-123">Request body</span></span>
<span data-ttu-id="b0f34-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b0f34-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b0f34-125">参数</span><span class="sxs-lookup"><span data-stu-id="b0f34-125">Parameter</span></span>    | <span data-ttu-id="b0f34-126">类型</span><span class="sxs-lookup"><span data-stu-id="b0f34-126">Type</span></span>   |<span data-ttu-id="b0f34-127">说明</span><span class="sxs-lookup"><span data-stu-id="b0f34-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0f34-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="b0f34-128">storageLocation</span></span>|<span data-ttu-id="b0f34-129">字符串</span><span class="sxs-lookup"><span data-stu-id="b0f34-129">String</span></span>|<span data-ttu-id="b0f34-130">这是 Azure 存储帐户的共享访问签名 (SAS) URL, 应导出数据的位置。</span><span class="sxs-lookup"><span data-stu-id="b0f34-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="b0f34-131">响应</span><span class="sxs-lookup"><span data-stu-id="b0f34-131">Response</span></span>
<span data-ttu-id="b0f34-132">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b0f34-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="b0f34-133">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b0f34-133">It does not return anything in the response body.</span></span> <span data-ttu-id="b0f34-134">响应包含以下响应头。</span><span class="sxs-lookup"><span data-stu-id="b0f34-134">The response contains the following response headers.</span></span>

| <span data-ttu-id="b0f34-135">名称</span><span class="sxs-lookup"><span data-stu-id="b0f34-135">Name</span></span>       | <span data-ttu-id="b0f34-136">说明</span><span class="sxs-lookup"><span data-stu-id="b0f34-136">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b0f34-137">Location</span><span class="sxs-lookup"><span data-stu-id="b0f34-137">Location</span></span>  | <span data-ttu-id="b0f34-138">用于检查请求状态的 URL。</span><span class="sxs-lookup"><span data-stu-id="b0f34-138">URL to check on the status of the request.</span></span> |
| <span data-ttu-id="b0f34-139">重试-After</span><span class="sxs-lookup"><span data-stu-id="b0f34-139">Retry-After</span></span>  | <span data-ttu-id="b0f34-140">以秒为单位的时间段。</span><span class="sxs-lookup"><span data-stu-id="b0f34-140">Time period in seconds.</span></span> <span data-ttu-id="b0f34-141">在提交请求以检查状态后, 请求生成器应等待这长时间。</span><span class="sxs-lookup"><span data-stu-id="b0f34-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |

## <a name="example"></a><span data-ttu-id="b0f34-142">示例</span><span class="sxs-lookup"><span data-stu-id="b0f34-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0f34-143">请求</span><span class="sxs-lookup"><span data-stu-id="b0f34-143">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="b0f34-144">响应</span><span class="sxs-lookup"><span data-stu-id="b0f34-144">Response</span></span>

```
#### SDK sample code
# [C#](#tab/cs)
[!INCLUDE [sample-code](../includes/user_exportpersonaldata-Cs-snippets.md)]

# [Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_exportpersonaldata-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
    "Error: /api-reference/v1.0/api/user-exportpersonaldata.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-exportpersonaldata.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
