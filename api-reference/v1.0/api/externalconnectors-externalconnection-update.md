---
title: 更新 externalConnection
description: 更新 externalConnection 对象的属性。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 4dc8c4ff93b160b34028aee250eb1b7f6f0cc86d
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467261"
---
# <a name="update-externalconnection"></a><span data-ttu-id="1d20c-103">更新 externalConnection</span><span class="sxs-lookup"><span data-stu-id="1d20c-103">Update externalConnection</span></span>

<span data-ttu-id="1d20c-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="1d20c-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="1d20c-105">更新 [externalConnection 对象](../resources/externalconnectors-externalconnection.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="1d20c-105">Update the properties of an [externalConnection](../resources/externalconnectors-externalconnection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d20c-106">权限</span><span class="sxs-lookup"><span data-stu-id="1d20c-106">Permissions</span></span>
<span data-ttu-id="1d20c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d20c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1d20c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d20c-109">Permission type</span></span>                        | <span data-ttu-id="1d20c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1d20c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1d20c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d20c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1d20c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d20c-112">Not supported.</span></span> |
| <span data-ttu-id="1d20c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d20c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d20c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d20c-114">Not supported.</span></span> |
| <span data-ttu-id="1d20c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d20c-115">Application</span></span>                            | <span data-ttu-id="1d20c-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="1d20c-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d20c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d20c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /connections/{connectionsId}
```

## <a name="request-headers"></a><span data-ttu-id="1d20c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d20c-118">Request headers</span></span>

| <span data-ttu-id="1d20c-119">名称</span><span class="sxs-lookup"><span data-stu-id="1d20c-119">Name</span></span>          | <span data-ttu-id="1d20c-120">说明</span><span class="sxs-lookup"><span data-stu-id="1d20c-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="1d20c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d20c-121">Authorization</span></span> | <span data-ttu-id="1d20c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1d20c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1d20c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d20c-124">Content-Type</span></span>  | <span data-ttu-id="1d20c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1d20c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d20c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d20c-127">Request body</span></span>
<span data-ttu-id="1d20c-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="1d20c-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1d20c-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="1d20c-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1d20c-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1d20c-130">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="1d20c-131">可更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="1d20c-131">The following properties can be updated.</span></span>

| <span data-ttu-id="1d20c-132">属性</span><span class="sxs-lookup"><span data-stu-id="1d20c-132">Property</span></span>      | <span data-ttu-id="1d20c-133">类型</span><span class="sxs-lookup"><span data-stu-id="1d20c-133">Type</span></span>                                           | <span data-ttu-id="1d20c-134">说明</span><span class="sxs-lookup"><span data-stu-id="1d20c-134">Description</span></span> |
|:--------------|:-----------------------------------------------|:------------|
| <span data-ttu-id="1d20c-135">configuration</span><span class="sxs-lookup"><span data-stu-id="1d20c-135">configuration</span></span> | [<span data-ttu-id="1d20c-136">microsoft.graph.externalConnectors.configuration</span><span class="sxs-lookup"><span data-stu-id="1d20c-136">microsoft.graph.externalConnectors.configuration</span></span>](../resources/externalconnectors-configuration.md) | <span data-ttu-id="1d20c-137">指定允许管理连接和索引连接内容的其他应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="1d20c-137">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> |
| <span data-ttu-id="1d20c-138">说明</span><span class="sxs-lookup"><span data-stu-id="1d20c-138">description</span></span>   | <span data-ttu-id="1d20c-139">String</span><span class="sxs-lookup"><span data-stu-id="1d20c-139">String</span></span>                                         | <span data-ttu-id="1d20c-140">网站中显示的连接Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="1d20c-140">Description of the connection displayed in the Microsoft 365 admin center.</span></span> |
| <span data-ttu-id="1d20c-141">name</span><span class="sxs-lookup"><span data-stu-id="1d20c-141">name</span></span>          | <span data-ttu-id="1d20c-142">String</span><span class="sxs-lookup"><span data-stu-id="1d20c-142">String</span></span>                                         | <span data-ttu-id="1d20c-143">要显示名称中显示的连接的Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="1d20c-143">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="1d20c-144">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="1d20c-144">Maximum length of 128 characters.</span></span> |


## <a name="response"></a><span data-ttu-id="1d20c-145">响应</span><span class="sxs-lookup"><span data-stu-id="1d20c-145">Response</span></span>

<span data-ttu-id="1d20c-146">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1d20c-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1d20c-147">示例</span><span class="sxs-lookup"><span data-stu-id="1d20c-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1d20c-148">请求</span><span class="sxs-lookup"><span data-stu-id="1d20c-148">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_externalconnection"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/connections/contosohr
Content-type: application/json

{
  "name": "Contoso HR Service Tickets",
  "description": "Connection to index HR service tickets"
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="1d20c-149">响应</span><span class="sxs-lookup"><span data-stu-id="1d20c-149">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="1d20c-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1d20c-150">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```