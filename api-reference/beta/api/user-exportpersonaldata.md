---
title: 用户： exportPersonalData
description: 提交数据策略操作发出的请求，公司管理员通过导出组织用户的数据。
ms.openlocfilehash: ffde9af132fbb15706fe54af8a6b3aaeba07d12b
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748267"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="44670-103">用户： exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="44670-103">user: exportPersonalData</span></span>

<span data-ttu-id="44670-104">提交数据策略操作发出的请求，由公司管理员导出组织用户的数据。</span><span class="sxs-lookup"><span data-stu-id="44670-104">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="44670-105">权限</span><span class="sxs-lookup"><span data-stu-id="44670-105">Permissions</span></span>
<span data-ttu-id="44670-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44670-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="44670-108">Permission type</span></span>      | <span data-ttu-id="44670-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44670-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44670-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44670-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="44670-111">User.Export.All 和 User.Read.All</span><span class="sxs-lookup"><span data-stu-id="44670-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="44670-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44670-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="44670-113">不适用</span><span class="sxs-lookup"><span data-stu-id="44670-113">Not applicable</span></span>  |
|<span data-ttu-id="44670-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="44670-114">Application</span></span> | <span data-ttu-id="44670-115">User.Export.All 和 User.Read.All</span><span class="sxs-lookup"><span data-stu-id="44670-115">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="44670-116">**注意：** 使用委派的权限时，仅可由公司管理员执行导出。</span><span class="sxs-lookup"><span data-stu-id="44670-116">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="44670-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44670-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="44670-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="44670-118">Request headers</span></span>
| <span data-ttu-id="44670-119">名称</span><span class="sxs-lookup"><span data-stu-id="44670-119">Name</span></span>       | <span data-ttu-id="44670-120">说明</span><span class="sxs-lookup"><span data-stu-id="44670-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="44670-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="44670-121">Authorization</span></span>  | <span data-ttu-id="44670-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="44670-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="44670-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="44670-123">Request body</span></span>
<span data-ttu-id="44670-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="44670-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="44670-125">参数</span><span class="sxs-lookup"><span data-stu-id="44670-125">Parameter</span></span>    | <span data-ttu-id="44670-126">类型</span><span class="sxs-lookup"><span data-stu-id="44670-126">Type</span></span>   |<span data-ttu-id="44670-127">说明</span><span class="sxs-lookup"><span data-stu-id="44670-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="44670-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="44670-128">storageLocation</span></span>|<span data-ttu-id="44670-129">字符串</span><span class="sxs-lookup"><span data-stu-id="44670-129">String</span></span>|<span data-ttu-id="44670-130">这是指向 Azure 存储帐户，其中应导出数据的共享的访问签名 (SA) URL。</span><span class="sxs-lookup"><span data-stu-id="44670-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="44670-131">响应</span><span class="sxs-lookup"><span data-stu-id="44670-131">Response</span></span>
<span data-ttu-id="44670-132">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="44670-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="44670-133">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="44670-133">It does not return anything in the response body.</span></span> <span data-ttu-id="44670-134">则响应中包含以下标头。</span><span class="sxs-lookup"><span data-stu-id="44670-134">The response contains the following headers.</span></span>

| <span data-ttu-id="44670-135">名称</span><span class="sxs-lookup"><span data-stu-id="44670-135">Name</span></span>       | <span data-ttu-id="44670-136">说明</span><span class="sxs-lookup"><span data-stu-id="44670-136">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="44670-137">Location</span><span class="sxs-lookup"><span data-stu-id="44670-137">Location</span></span>  | <span data-ttu-id="44670-138">若要检查请求的状态的 URL。</span><span class="sxs-lookup"><span data-stu-id="44670-138">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="44670-139">重试间隔后</span><span class="sxs-lookup"><span data-stu-id="44670-139">Retry-After</span></span>  | <span data-ttu-id="44670-140">以秒为单位的时间段。</span><span class="sxs-lookup"><span data-stu-id="44670-140">Time period in seconds.</span></span> <span data-ttu-id="44670-141">请求 maker 应等待这长之后提交请求以检查的状态。</span><span class="sxs-lookup"><span data-stu-id="44670-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="44670-142">示例</span><span class="sxs-lookup"><span data-stu-id="44670-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44670-143">请求</span><span class="sxs-lookup"><span data-stu-id="44670-143">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="44670-144">响应</span><span class="sxs-lookup"><span data-stu-id="44670-144">Response</span></span>

```
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
  "tocPath": ""
}-->
