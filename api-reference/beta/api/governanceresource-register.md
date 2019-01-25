---
title: 注册 governanceResource
description: 在 PIM 中注册一个非托管的 governanceResource 对象。
localization_priority: Normal
ms.openlocfilehash: f65c8b5884f08377967d3418bade0d5fc70c2063
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519043"
---
# <a name="register-governanceresource"></a><span data-ttu-id="6d93e-103">注册 governanceResource</span><span class="sxs-lookup"><span data-stu-id="6d93e-103">Register governanceResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d93e-104">在特权身份管理中注册一个非托管的[governanceResource](../resources/governanceresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6d93e-104">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d93e-105">权限</span><span class="sxs-lookup"><span data-stu-id="6d93e-105">Permissions</span></span>
<span data-ttu-id="6d93e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d93e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="6d93e-108">**注意：** 此 API 还需要请求者对资源具有至少一个活动角色分配。</span><span class="sxs-lookup"><span data-stu-id="6d93e-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="6d93e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d93e-109">Permission type</span></span>      | <span data-ttu-id="6d93e-110">权限</span><span class="sxs-lookup"><span data-stu-id="6d93e-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d93e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d93e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6d93e-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6d93e-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="6d93e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d93e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d93e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d93e-114">Not supported.</span></span>    |
|<span data-ttu-id="6d93e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d93e-115">Application</span></span> | <span data-ttu-id="6d93e-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6d93e-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d93e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d93e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="6d93e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6d93e-118">Optional query parameters</span></span>
<span data-ttu-id="6d93e-119">此方法**仅**支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="6d93e-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="6d93e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d93e-120">Request headers</span></span>
| <span data-ttu-id="6d93e-121">名称</span><span class="sxs-lookup"><span data-stu-id="6d93e-121">Name</span></span>      |<span data-ttu-id="6d93e-122">说明</span><span class="sxs-lookup"><span data-stu-id="6d93e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6d93e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d93e-123">Authorization</span></span>  | <span data-ttu-id="6d93e-124">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="6d93e-124">Bearer {code}</span></span>|
| <span data-ttu-id="6d93e-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="6d93e-125">Content-type</span></span>  | <span data-ttu-id="6d93e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d93e-126">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="6d93e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d93e-127">Request body</span></span>

|<span data-ttu-id="6d93e-128">参数</span><span class="sxs-lookup"><span data-stu-id="6d93e-128">Parameters</span></span>      |<span data-ttu-id="6d93e-129">类型</span><span class="sxs-lookup"><span data-stu-id="6d93e-129">Type</span></span>                 |<span data-ttu-id="6d93e-130">必需</span><span class="sxs-lookup"><span data-stu-id="6d93e-130">Required</span></span> |<span data-ttu-id="6d93e-131">说明</span><span class="sxs-lookup"><span data-stu-id="6d93e-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="6d93e-132">externalId</span><span class="sxs-lookup"><span data-stu-id="6d93e-132">externalId</span></span>    |<span data-ttu-id="6d93e-133">String</span><span class="sxs-lookup"><span data-stu-id="6d93e-133">String</span></span>                 |<span data-ttu-id="6d93e-134">✓</span><span class="sxs-lookup"><span data-stu-id="6d93e-134">✓</span></span>        |<span data-ttu-id="6d93e-135">要在 PIM 中注册的资源 externalId。</span><span class="sxs-lookup"><span data-stu-id="6d93e-135">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="6d93e-136">响应</span><span class="sxs-lookup"><span data-stu-id="6d93e-136">Response</span></span>
<span data-ttu-id="6d93e-137">如果成功，此方法返回`200 OK`响应。</span><span class="sxs-lookup"><span data-stu-id="6d93e-137">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="6d93e-138">示例</span><span class="sxs-lookup"><span data-stu-id="6d93e-138">Example</span></span>
<span data-ttu-id="6d93e-139">本示例演示如何注册的 Azure 订阅 Wingtip Toys-prod 移。</span><span class="sxs-lookup"><span data-stu-id="6d93e-139">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="6d93e-140">请求</span><span class="sxs-lookup"><span data-stu-id="6d93e-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="6d93e-141">响应</span><span class="sxs-lookup"><span data-stu-id="6d93e-141">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceresource-register.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
