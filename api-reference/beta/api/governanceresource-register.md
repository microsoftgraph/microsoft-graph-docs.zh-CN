---
title: 注册 governanceResource
description: 在 PIM 中注册一个非托管的 governanceResource 对象。
ms.openlocfilehash: 53452202b58c2d2187b6876eabfaae1ae646710d
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2018
ms.locfileid: "27195289"
---
# <a name="register-governanceresource"></a><span data-ttu-id="59418-103">注册 governanceResource</span><span class="sxs-lookup"><span data-stu-id="59418-103">Register governanceResource</span></span>

> <span data-ttu-id="59418-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="59418-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59418-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="59418-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59418-106">在特权身份管理中注册一个非托管的[governanceResource](../resources/governanceresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="59418-106">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="59418-107">权限</span><span class="sxs-lookup"><span data-stu-id="59418-107">Permissions</span></span>
<span data-ttu-id="59418-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59418-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="59418-110">**注意：** 此 API 还需要请求者对资源具有至少一个活动角色分配。</span><span class="sxs-lookup"><span data-stu-id="59418-110">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="59418-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="59418-111">Permission type</span></span>      | <span data-ttu-id="59418-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="59418-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59418-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59418-113">Delegated (work or school account)</span></span> | <span data-ttu-id="59418-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="59418-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="59418-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59418-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59418-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="59418-116">Not supported.</span></span>    |
|<span data-ttu-id="59418-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="59418-117">Application</span></span> | <span data-ttu-id="59418-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="59418-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="59418-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59418-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="59418-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="59418-120">Optional query parameters</span></span>
<span data-ttu-id="59418-121">此方法**仅**支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="59418-121">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="59418-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="59418-122">Request headers</span></span>
| <span data-ttu-id="59418-123">名称</span><span class="sxs-lookup"><span data-stu-id="59418-123">Name</span></span>      |<span data-ttu-id="59418-124">说明</span><span class="sxs-lookup"><span data-stu-id="59418-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="59418-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="59418-125">Authorization</span></span>  | <span data-ttu-id="59418-126">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="59418-126">Bearer {code}</span></span>|
| <span data-ttu-id="59418-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="59418-127">Content-type</span></span>  | <span data-ttu-id="59418-128">application/json</span><span class="sxs-lookup"><span data-stu-id="59418-128">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="59418-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="59418-129">Request body</span></span>

|<span data-ttu-id="59418-130">参数</span><span class="sxs-lookup"><span data-stu-id="59418-130">Parameters</span></span>      |<span data-ttu-id="59418-131">类型</span><span class="sxs-lookup"><span data-stu-id="59418-131">Type</span></span>                 |<span data-ttu-id="59418-132">必需</span><span class="sxs-lookup"><span data-stu-id="59418-132">Required</span></span> |<span data-ttu-id="59418-133">说明</span><span class="sxs-lookup"><span data-stu-id="59418-133">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="59418-134">externalId</span><span class="sxs-lookup"><span data-stu-id="59418-134">externalId</span></span>    |<span data-ttu-id="59418-135">String</span><span class="sxs-lookup"><span data-stu-id="59418-135">String</span></span>                 |<span data-ttu-id="59418-136">✓</span><span class="sxs-lookup"><span data-stu-id="59418-136">✓</span></span>        |<span data-ttu-id="59418-137">要在 PIM 中注册的资源 externalId。</span><span class="sxs-lookup"><span data-stu-id="59418-137">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="59418-138">响应</span><span class="sxs-lookup"><span data-stu-id="59418-138">Response</span></span>
<span data-ttu-id="59418-139">如果成功，此方法返回`200 OK`响应。</span><span class="sxs-lookup"><span data-stu-id="59418-139">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="59418-140">示例</span><span class="sxs-lookup"><span data-stu-id="59418-140">Example</span></span>
<span data-ttu-id="59418-141">本示例演示如何注册的 Azure 订阅 Wingtip Toys-prod 移。</span><span class="sxs-lookup"><span data-stu-id="59418-141">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="59418-142">请求</span><span class="sxs-lookup"><span data-stu-id="59418-142">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="59418-143">响应</span><span class="sxs-lookup"><span data-stu-id="59418-143">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
