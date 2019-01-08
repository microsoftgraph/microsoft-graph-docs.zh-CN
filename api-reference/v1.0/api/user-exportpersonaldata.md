---
title: 用户： exportPersonalData
description: 提交数据策略操作发出的请求，公司管理员通过导出组织用户的数据。
ms.openlocfilehash: 9308e955e83ccad5779d8261537306a5220d8086
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748211"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="92505-103">用户： exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="92505-103">user: exportPersonalData</span></span>

<span data-ttu-id="92505-104">提交数据策略操作请求从公司管理员或要导出的组织的用户数据的应用程序。</span><span class="sxs-lookup"><span data-stu-id="92505-104">Submit a data policy operation request from a company administrator or an application to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="92505-105">权限</span><span class="sxs-lookup"><span data-stu-id="92505-105">Permissions</span></span>
<span data-ttu-id="92505-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92505-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="92505-108">Permission type</span></span>      | <span data-ttu-id="92505-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92505-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92505-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92505-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="92505-111">User.Export.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="92505-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="92505-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92505-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="92505-113">不适用</span><span class="sxs-lookup"><span data-stu-id="92505-113">Not applicable</span></span>  |
|<span data-ttu-id="92505-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="92505-114">Application</span></span> | <span data-ttu-id="92505-115">User.Export.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="92505-115">User.Export.All, User.Read.All</span></span> |

><span data-ttu-id="92505-116">**注意：** 由公司管理员可以仅执行导出时所使用的委派的权限。</span><span class="sxs-lookup"><span data-stu-id="92505-116">**Note:** The export can only be performed by a company administrator when delegated permissions are used.</span></span>

## <a name="http-request"></a><span data-ttu-id="92505-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92505-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="92505-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="92505-118">Request headers</span></span>
| <span data-ttu-id="92505-119">名称</span><span class="sxs-lookup"><span data-stu-id="92505-119">Name</span></span>       | <span data-ttu-id="92505-120">说明</span><span class="sxs-lookup"><span data-stu-id="92505-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="92505-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="92505-121">Authorization</span></span>  | <span data-ttu-id="92505-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="92505-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="92505-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="92505-123">Request body</span></span>
<span data-ttu-id="92505-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="92505-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="92505-125">参数</span><span class="sxs-lookup"><span data-stu-id="92505-125">Parameter</span></span>    | <span data-ttu-id="92505-126">类型</span><span class="sxs-lookup"><span data-stu-id="92505-126">Type</span></span>   |<span data-ttu-id="92505-127">说明</span><span class="sxs-lookup"><span data-stu-id="92505-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92505-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="92505-128">storageLocation</span></span>|<span data-ttu-id="92505-129">字符串</span><span class="sxs-lookup"><span data-stu-id="92505-129">String</span></span>|<span data-ttu-id="92505-130">这是指向 Azure 存储帐户，其中应导出数据的共享的访问签名 (SA) URL。</span><span class="sxs-lookup"><span data-stu-id="92505-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="92505-131">响应</span><span class="sxs-lookup"><span data-stu-id="92505-131">Response</span></span>
<span data-ttu-id="92505-132">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="92505-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="92505-133">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="92505-133">It does not return anything in the response body.</span></span> <span data-ttu-id="92505-134">则响应中包含以下响应标头。</span><span class="sxs-lookup"><span data-stu-id="92505-134">The response contains the following response headers.</span></span>

| <span data-ttu-id="92505-135">名称</span><span class="sxs-lookup"><span data-stu-id="92505-135">Name</span></span>       | <span data-ttu-id="92505-136">说明</span><span class="sxs-lookup"><span data-stu-id="92505-136">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="92505-137">Location</span><span class="sxs-lookup"><span data-stu-id="92505-137">Location</span></span>  | <span data-ttu-id="92505-138">若要检查请求的状态的 URL。</span><span class="sxs-lookup"><span data-stu-id="92505-138">URL to check on the status of the request.</span></span> |
| <span data-ttu-id="92505-139">重试间隔后</span><span class="sxs-lookup"><span data-stu-id="92505-139">Retry-After</span></span>  | <span data-ttu-id="92505-140">以秒为单位的时间段。</span><span class="sxs-lookup"><span data-stu-id="92505-140">Time period in seconds.</span></span> <span data-ttu-id="92505-141">请求 maker 应等待这长之后提交请求以检查的状态。</span><span class="sxs-lookup"><span data-stu-id="92505-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |

## <a name="example"></a><span data-ttu-id="92505-142">示例</span><span class="sxs-lookup"><span data-stu-id="92505-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92505-143">请求</span><span class="sxs-lookup"><span data-stu-id="92505-143">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="92505-144">响应</span><span class="sxs-lookup"><span data-stu-id="92505-144">Response</span></span>

```
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
  "tocPath": ""
}-->
