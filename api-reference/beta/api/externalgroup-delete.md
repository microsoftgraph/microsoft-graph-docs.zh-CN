---
title: 删除 externalGroup
description: 删除一个 externalGroup 对象。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 4358c162e8ba07690c5bf19a11656ffcf292939e
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193849"
---
# <a name="delete-externalgroup"></a><span data-ttu-id="c8855-103">删除 externalGroup</span><span class="sxs-lookup"><span data-stu-id="c8855-103">Delete externalGroup</span></span>

<span data-ttu-id="c8855-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8855-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8855-105">删除 [externalGroup](../resources/externalgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c8855-105">Delete an [externalGroup](../resources/externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8855-106">权限</span><span class="sxs-lookup"><span data-stu-id="c8855-106">Permissions</span></span>

<span data-ttu-id="c8855-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8855-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8855-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8855-109">Permission type</span></span>                        | <span data-ttu-id="c8855-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c8855-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c8855-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8855-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8855-112">不支持</span><span class="sxs-lookup"><span data-stu-id="c8855-112">Not supported</span></span>                               |
| <span data-ttu-id="c8855-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8855-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8855-114">不支持</span><span class="sxs-lookup"><span data-stu-id="c8855-114">Not supported</span></span>                               |
| <span data-ttu-id="c8855-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8855-115">Application</span></span>                            | <span data-ttu-id="c8855-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8855-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="c8855-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8855-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="c8855-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8855-118">Request headers</span></span>

| <span data-ttu-id="c8855-119">名称</span><span class="sxs-lookup"><span data-stu-id="c8855-119">Name</span></span>          | <span data-ttu-id="c8855-120">说明</span><span class="sxs-lookup"><span data-stu-id="c8855-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c8855-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8855-121">Authorization</span></span> | <span data-ttu-id="c8855-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8855-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8855-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8855-124">Request body</span></span>

<span data-ttu-id="c8855-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c8855-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8855-126">响应</span><span class="sxs-lookup"><span data-stu-id="c8855-126">Response</span></span>

<span data-ttu-id="c8855-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c8855-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c8855-128">示例</span><span class="sxs-lookup"><span data-stu-id="c8855-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8855-129">请求</span><span class="sxs-lookup"><span data-stu-id="c8855-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_externalgroup"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="c8855-130">响应</span><span class="sxs-lookup"><span data-stu-id="c8855-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
