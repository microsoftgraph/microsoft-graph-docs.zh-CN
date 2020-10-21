---
title: governanceResource： register
description: 在 PIM 中注册 governanceResource 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: df5e9a2d63c6a49a8eb7b8ab9b5ed88b4f50c577
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635057"
---
# <a name="governanceresource-register"></a><span data-ttu-id="19d4e-103">governanceResource： register</span><span class="sxs-lookup"><span data-stu-id="19d4e-103">governanceResource: register</span></span>

<span data-ttu-id="19d4e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19d4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19d4e-105">在特权标识管理中注册 [governanceResource](../resources/governanceresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19d4e-105">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="19d4e-106">权限</span><span class="sxs-lookup"><span data-stu-id="19d4e-106">Permissions</span></span>

<span data-ttu-id="19d4e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="19d4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="19d4e-109">**注意：** 此 API 还要求请求者在资源上至少有一个活动角色分配。</span><span class="sxs-lookup"><span data-stu-id="19d4e-109">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

### <a name="azure-resources"></a><span data-ttu-id="19d4e-110">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="19d4e-110">Azure resources</span></span>

| <span data-ttu-id="19d4e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="19d4e-111">Permission type</span></span> | <span data-ttu-id="19d4e-112">权限</span><span class="sxs-lookup"><span data-stu-id="19d4e-112">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="19d4e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19d4e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="19d4e-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="19d4e-114">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="19d4e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19d4e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19d4e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="19d4e-116">Not supported.</span></span> |
| <span data-ttu-id="19d4e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="19d4e-117">Application</span></span> | <span data-ttu-id="19d4e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="19d4e-118">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="19d4e-119">Azure AD</span><span class="sxs-lookup"><span data-stu-id="19d4e-119">Azure AD</span></span>

| <span data-ttu-id="19d4e-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="19d4e-120">Permission type</span></span> | <span data-ttu-id="19d4e-121">权限</span><span class="sxs-lookup"><span data-stu-id="19d4e-121">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="19d4e-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19d4e-122">Delegated (work or school account)</span></span> | <span data-ttu-id="19d4e-123">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="19d4e-123">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="19d4e-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19d4e-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19d4e-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="19d4e-125">Not supported.</span></span> |
| <span data-ttu-id="19d4e-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="19d4e-126">Application</span></span> | <span data-ttu-id="19d4e-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="19d4e-127">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="19d4e-128">组</span><span class="sxs-lookup"><span data-stu-id="19d4e-128">Groups</span></span>

|<span data-ttu-id="19d4e-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="19d4e-129">Permission type</span></span> | <span data-ttu-id="19d4e-130">权限</span><span class="sxs-lookup"><span data-stu-id="19d4e-130">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="19d4e-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19d4e-131">Delegated (work or school account)</span></span> | <span data-ttu-id="19d4e-132">PrivilegedAccess AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="19d4e-132">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="19d4e-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19d4e-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19d4e-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="19d4e-134">Not supported.</span></span> |
| <span data-ttu-id="19d4e-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="19d4e-135">Application</span></span> | <span data-ttu-id="19d4e-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="19d4e-136">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19d4e-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19d4e-137">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19d4e-138">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="19d4e-138">Optional query parameters</span></span>

<span data-ttu-id="19d4e-139">此方法 **仅** 支持 `$select` 和 `$expand` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="19d4e-139">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19d4e-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="19d4e-140">Request headers</span></span>

| <span data-ttu-id="19d4e-141">名称</span><span class="sxs-lookup"><span data-stu-id="19d4e-141">Name</span></span> | <span data-ttu-id="19d4e-142">说明</span><span class="sxs-lookup"><span data-stu-id="19d4e-142">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="19d4e-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="19d4e-143">Authorization</span></span> | <span data-ttu-id="19d4e-144">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="19d4e-144">Bearer {token}</span></span> |
| <span data-ttu-id="19d4e-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="19d4e-145">Content-type</span></span> | <span data-ttu-id="19d4e-146">application/json</span><span class="sxs-lookup"><span data-stu-id="19d4e-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="19d4e-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="19d4e-147">Request body</span></span>

| <span data-ttu-id="19d4e-148">属性</span><span class="sxs-lookup"><span data-stu-id="19d4e-148">Properties</span></span> | <span data-ttu-id="19d4e-149">类型</span><span class="sxs-lookup"><span data-stu-id="19d4e-149">Type</span></span> | <span data-ttu-id="19d4e-150">说明</span><span class="sxs-lookup"><span data-stu-id="19d4e-150">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="19d4e-151">externalId</span><span class="sxs-lookup"><span data-stu-id="19d4e-151">externalId</span></span> | <span data-ttu-id="19d4e-152">String</span><span class="sxs-lookup"><span data-stu-id="19d4e-152">String</span></span> | <span data-ttu-id="19d4e-153">要在 PIM 中注册的资源的外部标识符。</span><span class="sxs-lookup"><span data-stu-id="19d4e-153">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="19d4e-154">如果注册订阅，则标识符为预置的订阅标识符 `/subscriptions/` 。</span><span class="sxs-lookup"><span data-stu-id="19d4e-154">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="19d4e-155">例如，`/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`。</span><span class="sxs-lookup"><span data-stu-id="19d4e-155">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="19d4e-156">响应</span><span class="sxs-lookup"><span data-stu-id="19d4e-156">Response</span></span>

<span data-ttu-id="19d4e-157">如果成功，此方法将返回 `200 OK` 响应。</span><span class="sxs-lookup"><span data-stu-id="19d4e-157">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="19d4e-158">示例</span><span class="sxs-lookup"><span data-stu-id="19d4e-158">Example</span></span>

<span data-ttu-id="19d4e-159">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="19d4e-159">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="19d4e-160">请求</span><span class="sxs-lookup"><span data-stu-id="19d4e-160">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="19d4e-161">响应</span><span class="sxs-lookup"><span data-stu-id="19d4e-161">Response</span></span>
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


