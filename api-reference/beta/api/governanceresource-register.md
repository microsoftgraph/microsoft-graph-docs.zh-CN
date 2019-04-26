---
title: 注册 governanceResource
description: 在 PIM 中注册非托管的 governanceResource 对象。
localization_priority: Normal
ms.openlocfilehash: a6ad89f799ee171971f7301ed039cf1b6d9111ea
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329745"
---
# <a name="register-governanceresource"></a><span data-ttu-id="8300b-103">注册 governanceResource</span><span class="sxs-lookup"><span data-stu-id="8300b-103">Register governanceResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8300b-104">在特权标识管理中注册非托管的[governanceResource](../resources/governanceresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8300b-104">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="8300b-105">权限</span><span class="sxs-lookup"><span data-stu-id="8300b-105">Permissions</span></span>
<span data-ttu-id="8300b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8300b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="8300b-108">**注意:** 此 API 还要求请求者在资源上至少有一个活动角色分配。</span><span class="sxs-lookup"><span data-stu-id="8300b-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="8300b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8300b-109">Permission type</span></span>      | <span data-ttu-id="8300b-110">权限</span><span class="sxs-lookup"><span data-stu-id="8300b-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8300b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8300b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8300b-112">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="8300b-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="8300b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8300b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8300b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8300b-114">Not supported.</span></span>    |
|<span data-ttu-id="8300b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8300b-115">Application</span></span> | <span data-ttu-id="8300b-116">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="8300b-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="8300b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8300b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="8300b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8300b-118">Optional query parameters</span></span>
<span data-ttu-id="8300b-119">此方法**仅**支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8300b-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="8300b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8300b-120">Request headers</span></span>
| <span data-ttu-id="8300b-121">名称</span><span class="sxs-lookup"><span data-stu-id="8300b-121">Name</span></span>      |<span data-ttu-id="8300b-122">说明</span><span class="sxs-lookup"><span data-stu-id="8300b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8300b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8300b-123">Authorization</span></span>  | <span data-ttu-id="8300b-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8300b-124">Bearer {code}</span></span>|
| <span data-ttu-id="8300b-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="8300b-125">Content-type</span></span>  | <span data-ttu-id="8300b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8300b-126">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="8300b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8300b-127">Request body</span></span>

|<span data-ttu-id="8300b-128">参数</span><span class="sxs-lookup"><span data-stu-id="8300b-128">Parameters</span></span>      |<span data-ttu-id="8300b-129">类型</span><span class="sxs-lookup"><span data-stu-id="8300b-129">Type</span></span>                 |<span data-ttu-id="8300b-130">必需</span><span class="sxs-lookup"><span data-stu-id="8300b-130">Required</span></span> |<span data-ttu-id="8300b-131">说明</span><span class="sxs-lookup"><span data-stu-id="8300b-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="8300b-132">externalId</span><span class="sxs-lookup"><span data-stu-id="8300b-132">externalId</span></span>    |<span data-ttu-id="8300b-133">String</span><span class="sxs-lookup"><span data-stu-id="8300b-133">String</span></span>                 |<span data-ttu-id="8300b-134">✓</span><span class="sxs-lookup"><span data-stu-id="8300b-134">✓</span></span>        |<span data-ttu-id="8300b-135">要在 PIM 中注册的资源的 externalId。</span><span class="sxs-lookup"><span data-stu-id="8300b-135">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="8300b-136">响应</span><span class="sxs-lookup"><span data-stu-id="8300b-136">Response</span></span>
<span data-ttu-id="8300b-137">如果成功, 此方法将`200 OK`返回响应。</span><span class="sxs-lookup"><span data-stu-id="8300b-137">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="8300b-138">示例</span><span class="sxs-lookup"><span data-stu-id="8300b-138">Example</span></span>
<span data-ttu-id="8300b-139">本示例演示如何注册 Azure 订阅 Wingtip 玩具-生产。</span><span class="sxs-lookup"><span data-stu-id="8300b-139">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="8300b-140">请求</span><span class="sxs-lookup"><span data-stu-id="8300b-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="8300b-141">响应</span><span class="sxs-lookup"><span data-stu-id="8300b-141">Response</span></span>
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
  "suppressions": []
}
-->
