---
title: 'governanceResource: register'
description: 在 PIM 中注册 governanceResource 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b8457f7ddee4564ca6b6b300121ddb7b8247e34
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713917"
---
# <a name="governanceresource-register"></a><span data-ttu-id="157ff-103">governanceResource: register</span><span class="sxs-lookup"><span data-stu-id="157ff-103">governanceResource: register</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="157ff-104">在特权标识管理中注册[governanceResource](../resources/governanceresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="157ff-104">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="157ff-105">权限</span><span class="sxs-lookup"><span data-stu-id="157ff-105">Permissions</span></span>

<span data-ttu-id="157ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="157ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="157ff-108">**注意:** 此 API 还要求请求者在资源上至少有一个活动角色分配。</span><span class="sxs-lookup"><span data-stu-id="157ff-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

| <span data-ttu-id="157ff-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="157ff-109">Permission type</span></span> | <span data-ttu-id="157ff-110">权限</span><span class="sxs-lookup"><span data-stu-id="157ff-110">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="157ff-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="157ff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="157ff-112">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="157ff-112">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="157ff-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="157ff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="157ff-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="157ff-114">Not supported.</span></span> |
| <span data-ttu-id="157ff-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="157ff-115">Application</span></span> | <span data-ttu-id="157ff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="157ff-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="157ff-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="157ff-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="157ff-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="157ff-118">Optional query parameters</span></span>

<span data-ttu-id="157ff-119">此方法**仅**支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="157ff-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="157ff-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="157ff-120">Request headers</span></span>

| <span data-ttu-id="157ff-121">名称</span><span class="sxs-lookup"><span data-stu-id="157ff-121">Name</span></span> | <span data-ttu-id="157ff-122">说明</span><span class="sxs-lookup"><span data-stu-id="157ff-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="157ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="157ff-123">Authorization</span></span> | <span data-ttu-id="157ff-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="157ff-124">Bearer {token}</span></span> |
| <span data-ttu-id="157ff-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="157ff-125">Content-type</span></span> | <span data-ttu-id="157ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="157ff-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="157ff-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="157ff-127">Request body</span></span>

| <span data-ttu-id="157ff-128">属性</span><span class="sxs-lookup"><span data-stu-id="157ff-128">Properties</span></span> | <span data-ttu-id="157ff-129">类型</span><span class="sxs-lookup"><span data-stu-id="157ff-129">Type</span></span> | <span data-ttu-id="157ff-130">说明</span><span class="sxs-lookup"><span data-stu-id="157ff-130">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="157ff-131">externalId</span><span class="sxs-lookup"><span data-stu-id="157ff-131">externalId</span></span> | <span data-ttu-id="157ff-132">String</span><span class="sxs-lookup"><span data-stu-id="157ff-132">String</span></span> | <span data-ttu-id="157ff-133">要在 PIM 中注册的资源的外部标识符。</span><span class="sxs-lookup"><span data-stu-id="157ff-133">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="157ff-134">如果注册订阅, 则标识符为预置的订阅标识符`/subscriptions/`。</span><span class="sxs-lookup"><span data-stu-id="157ff-134">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="157ff-135">例如，`/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`。</span><span class="sxs-lookup"><span data-stu-id="157ff-135">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="157ff-136">响应</span><span class="sxs-lookup"><span data-stu-id="157ff-136">Response</span></span>

<span data-ttu-id="157ff-137">如果成功, 此方法将`200 OK`返回响应。</span><span class="sxs-lookup"><span data-stu-id="157ff-137">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="157ff-138">示例</span><span class="sxs-lookup"><span data-stu-id="157ff-138">Example</span></span>

<span data-ttu-id="157ff-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="157ff-139">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="157ff-140">请求</span><span class="sxs-lookup"><span data-stu-id="157ff-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="157ff-141">响应</span><span class="sxs-lookup"><span data-stu-id="157ff-141">Response</span></span>
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
