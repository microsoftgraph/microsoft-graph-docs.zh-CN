---
title: 更新 externalConnection
description: 更新 externalConnection 的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 3caef56676060c37c092aed63bf12a4939bd551e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938644"
---
# <a name="update-connection"></a><span data-ttu-id="f5482-103">更新连接</span><span class="sxs-lookup"><span data-stu-id="f5482-103">Update connection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5482-104">更新[externalConnection](../resources/externalconnection.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="f5482-104">Update the properties of an [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5482-105">权限</span><span class="sxs-lookup"><span data-stu-id="f5482-105">Permissions</span></span>

<span data-ttu-id="f5482-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5482-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5482-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5482-108">Permission type</span></span>                        | <span data-ttu-id="f5482-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5482-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f5482-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5482-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5482-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5482-111">Not supported.</span></span> |
| <span data-ttu-id="f5482-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5482-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5482-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5482-113">Not supported.</span></span> |
| <span data-ttu-id="f5482-114">Application</span><span class="sxs-lookup"><span data-stu-id="f5482-114">Application</span></span>                            | <span data-ttu-id="f5482-115">ExternalItem</span><span class="sxs-lookup"><span data-stu-id="f5482-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5482-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5482-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f5482-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5482-117">Request headers</span></span>

| <span data-ttu-id="f5482-118">名称</span><span class="sxs-lookup"><span data-stu-id="f5482-118">Name</span></span>          | <span data-ttu-id="f5482-119">说明</span><span class="sxs-lookup"><span data-stu-id="f5482-119">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="f5482-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5482-120">Authorization</span></span> | <span data-ttu-id="f5482-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f5482-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f5482-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5482-123">Content-Type</span></span>  | <span data-ttu-id="f5482-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f5482-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5482-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5482-126">Request body</span></span>

<span data-ttu-id="f5482-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="f5482-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f5482-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="f5482-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f5482-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f5482-129">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="f5482-130">可更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="f5482-130">The following properties can be updated.</span></span>

| <span data-ttu-id="f5482-131">属性</span><span class="sxs-lookup"><span data-stu-id="f5482-131">Property</span></span>      | <span data-ttu-id="f5482-132">类型</span><span class="sxs-lookup"><span data-stu-id="f5482-132">Type</span></span>                                           | <span data-ttu-id="f5482-133">描述</span><span class="sxs-lookup"><span data-stu-id="f5482-133">Description</span></span> |
|:--------------|:-----------------------------------------------|:------------|
| <span data-ttu-id="f5482-134">设置</span><span class="sxs-lookup"><span data-stu-id="f5482-134">configuration</span></span> | [<span data-ttu-id="f5482-135">configuration</span><span class="sxs-lookup"><span data-stu-id="f5482-135">configuration</span></span>](../resources/configuration.md) | <span data-ttu-id="f5482-136">指定允许管理连接和索引连接中的内容的其他应用程序 Id。</span><span class="sxs-lookup"><span data-stu-id="f5482-136">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> |
| <span data-ttu-id="f5482-137">description</span><span class="sxs-lookup"><span data-stu-id="f5482-137">description</span></span>   | <span data-ttu-id="f5482-138">String</span><span class="sxs-lookup"><span data-stu-id="f5482-138">String</span></span>                                         | <span data-ttu-id="f5482-139">Microsoft 365 管理中心显示的连接的说明。</span><span class="sxs-lookup"><span data-stu-id="f5482-139">Description of the connection displayed in the Microsoft 365 admin center.</span></span> |
| <span data-ttu-id="f5482-140">name</span><span class="sxs-lookup"><span data-stu-id="f5482-140">name</span></span>          | <span data-ttu-id="f5482-141">字符串</span><span class="sxs-lookup"><span data-stu-id="f5482-141">String</span></span>                                         | <span data-ttu-id="f5482-142">要显示在 Microsoft 365 管理中心中的连接的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f5482-142">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="f5482-143">最大长度为128个字符。</span><span class="sxs-lookup"><span data-stu-id="f5482-143">Maximum length of 128 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="f5482-144">响应</span><span class="sxs-lookup"><span data-stu-id="f5482-144">Response</span></span>

<span data-ttu-id="f5482-145">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f5482-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f5482-146">示例</span><span class="sxs-lookup"><span data-stu-id="f5482-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5482-147">请求</span><span class="sxs-lookup"><span data-stu-id="f5482-147">Request</span></span>

<span data-ttu-id="f5482-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f5482-148">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connection"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr
Content-type: application/json

{
  "name": "Contoso HR Service Tickets",
  "description": "Connection to index HR service tickets"
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="f5482-149">响应</span><span class="sxs-lookup"><span data-stu-id="f5482-149">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="f5482-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f5482-150">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update connection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
