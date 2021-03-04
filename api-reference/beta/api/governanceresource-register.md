---
title: governanceResource：register
description: 在 PIM 中注册 governanceResource 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: fed82587a1132b6c39e6e27e09546906792486b0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435941"
---
# <a name="governanceresource-register"></a><span data-ttu-id="c5fab-103">governanceResource：register</span><span class="sxs-lookup"><span data-stu-id="c5fab-103">governanceResource: register</span></span>

<span data-ttu-id="c5fab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5fab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5fab-105">在 Privileged Identity Management 中注册 [governanceResource](../resources/governanceresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c5fab-105">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5fab-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c5fab-106">Permissions</span></span>

<span data-ttu-id="c5fab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="c5fab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="c5fab-109">**注意：** 此 API 还要求请求者至少对资源角色分配一个活动应用程序。</span><span class="sxs-lookup"><span data-stu-id="c5fab-109">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

### <a name="azure-resources"></a><span data-ttu-id="c5fab-110">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="c5fab-110">Azure resources</span></span>

| <span data-ttu-id="c5fab-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5fab-111">Permission type</span></span> | <span data-ttu-id="c5fab-112">权限</span><span class="sxs-lookup"><span data-stu-id="c5fab-112">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="c5fab-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5fab-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c5fab-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c5fab-114">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="c5fab-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5fab-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5fab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5fab-116">Not supported.</span></span> |
| <span data-ttu-id="c5fab-117">Application</span><span class="sxs-lookup"><span data-stu-id="c5fab-117">Application</span></span> | <span data-ttu-id="c5fab-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5fab-118">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="c5fab-119">Azure AD</span><span class="sxs-lookup"><span data-stu-id="c5fab-119">Azure AD</span></span>

| <span data-ttu-id="c5fab-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5fab-120">Permission type</span></span> | <span data-ttu-id="c5fab-121">权限</span><span class="sxs-lookup"><span data-stu-id="c5fab-121">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="c5fab-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5fab-122">Delegated (work or school account)</span></span> | <span data-ttu-id="c5fab-123">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="c5fab-123">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="c5fab-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5fab-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5fab-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5fab-125">Not supported.</span></span> |
| <span data-ttu-id="c5fab-126">Application</span><span class="sxs-lookup"><span data-stu-id="c5fab-126">Application</span></span> | <span data-ttu-id="c5fab-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5fab-127">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="c5fab-128">组</span><span class="sxs-lookup"><span data-stu-id="c5fab-128">Groups</span></span>

|<span data-ttu-id="c5fab-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5fab-129">Permission type</span></span> | <span data-ttu-id="c5fab-130">权限</span><span class="sxs-lookup"><span data-stu-id="c5fab-130">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="c5fab-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5fab-131">Delegated (work or school account)</span></span> | <span data-ttu-id="c5fab-132">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="c5fab-132">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="c5fab-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5fab-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5fab-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5fab-134">Not supported.</span></span> |
| <span data-ttu-id="c5fab-135">Application</span><span class="sxs-lookup"><span data-stu-id="c5fab-135">Application</span></span> | <span data-ttu-id="c5fab-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5fab-136">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5fab-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5fab-137">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5fab-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c5fab-138">Optional query parameters</span></span>

<span data-ttu-id="c5fab-139">此方法 **仅** 支持和 `$select` `$expand` [OData](/graph/query-parameters) 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c5fab-139">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5fab-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5fab-140">Request headers</span></span>

| <span data-ttu-id="c5fab-141">名称</span><span class="sxs-lookup"><span data-stu-id="c5fab-141">Name</span></span> | <span data-ttu-id="c5fab-142">说明</span><span class="sxs-lookup"><span data-stu-id="c5fab-142">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="c5fab-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5fab-143">Authorization</span></span> | <span data-ttu-id="c5fab-144">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="c5fab-144">Bearer {token}</span></span> |
| <span data-ttu-id="c5fab-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="c5fab-145">Content-type</span></span> | <span data-ttu-id="c5fab-146">application/json</span><span class="sxs-lookup"><span data-stu-id="c5fab-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5fab-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5fab-147">Request body</span></span>

| <span data-ttu-id="c5fab-148">属性</span><span class="sxs-lookup"><span data-stu-id="c5fab-148">Properties</span></span> | <span data-ttu-id="c5fab-149">类型</span><span class="sxs-lookup"><span data-stu-id="c5fab-149">Type</span></span> | <span data-ttu-id="c5fab-150">说明</span><span class="sxs-lookup"><span data-stu-id="c5fab-150">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="c5fab-151">externalId</span><span class="sxs-lookup"><span data-stu-id="c5fab-151">externalId</span></span> | <span data-ttu-id="c5fab-152">String</span><span class="sxs-lookup"><span data-stu-id="c5fab-152">String</span></span> | <span data-ttu-id="c5fab-153">在 PIM 中注册的资源的外部标识符。</span><span class="sxs-lookup"><span data-stu-id="c5fab-153">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="c5fab-154">如果注册订阅，标识符是预先预置的订阅标识符 `/subscriptions/` 。</span><span class="sxs-lookup"><span data-stu-id="c5fab-154">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="c5fab-155">例如，`/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`。</span><span class="sxs-lookup"><span data-stu-id="c5fab-155">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="c5fab-156">响应</span><span class="sxs-lookup"><span data-stu-id="c5fab-156">Response</span></span>

<span data-ttu-id="c5fab-157">如果成功，此方法将返回 `200 OK` 响应。</span><span class="sxs-lookup"><span data-stu-id="c5fab-157">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="c5fab-158">示例</span><span class="sxs-lookup"><span data-stu-id="c5fab-158">Example</span></span>

<span data-ttu-id="c5fab-159">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="c5fab-159">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="c5fab-160">请求</span><span class="sxs-lookup"><span data-stu-id="c5fab-160">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="c5fab-161">响应</span><span class="sxs-lookup"><span data-stu-id="c5fab-161">Response</span></span>
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


