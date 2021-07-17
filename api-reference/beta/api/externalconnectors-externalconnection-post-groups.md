---
title: 创建 externalGroup
description: 创建新的 externalGroup 对象。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 128396676462bcf2231f566b7a9830d58ddbc2c8
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467583"
---
# <a name="create-externalgroup"></a><span data-ttu-id="aa45c-103">创建 externalGroup</span><span class="sxs-lookup"><span data-stu-id="aa45c-103">Create externalGroup</span></span>

<span data-ttu-id="aa45c-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="aa45c-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa45c-105">创建新的 [externalGroup](../resources/externalconnectors-externalgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aa45c-105">Create a new [externalGroup](../resources/externalconnectors-externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa45c-106">权限</span><span class="sxs-lookup"><span data-stu-id="aa45c-106">Permissions</span></span>

<span data-ttu-id="aa45c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa45c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aa45c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa45c-109">Permission type</span></span>                        | <span data-ttu-id="aa45c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa45c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aa45c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa45c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa45c-112">不支持</span><span class="sxs-lookup"><span data-stu-id="aa45c-112">Not supported</span></span>                               |
| <span data-ttu-id="aa45c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa45c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa45c-114">不支持</span><span class="sxs-lookup"><span data-stu-id="aa45c-114">Not supported</span></span>                               |
| <span data-ttu-id="aa45c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa45c-115">Application</span></span>                            | <span data-ttu-id="aa45c-116">ExternalItem.ReadWrite.OwnedBy、ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa45c-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="aa45c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa45c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionId}/groups
```

## <a name="request-headers"></a><span data-ttu-id="aa45c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa45c-118">Request headers</span></span>

| <span data-ttu-id="aa45c-119">名称</span><span class="sxs-lookup"><span data-stu-id="aa45c-119">Name</span></span>          | <span data-ttu-id="aa45c-120">说明</span><span class="sxs-lookup"><span data-stu-id="aa45c-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="aa45c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa45c-121">Authorization</span></span> | <span data-ttu-id="aa45c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa45c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="aa45c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aa45c-124">Content-Type</span></span>  | <span data-ttu-id="aa45c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="aa45c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa45c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa45c-127">Request body</span></span>

<span data-ttu-id="aa45c-128">在请求正文中，提供 [externalGroup](../resources/externalconnectors-externalgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa45c-128">In the request body, supply a JSON representation of the [externalGroup](../resources/externalconnectors-externalgroup.md) object.</span></span>

<span data-ttu-id="aa45c-129">下表显示创建 [externalGroup](../resources/externalconnectors-externalgroup.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aa45c-129">The following table shows the properties that are required when you create the [externalGroup](../resources/externalconnectors-externalgroup.md).</span></span>

| <span data-ttu-id="aa45c-130">属性</span><span class="sxs-lookup"><span data-stu-id="aa45c-130">Property</span></span>    | <span data-ttu-id="aa45c-131">类型</span><span class="sxs-lookup"><span data-stu-id="aa45c-131">Type</span></span>   | <span data-ttu-id="aa45c-132">说明</span><span class="sxs-lookup"><span data-stu-id="aa45c-132">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="aa45c-133">id</span><span class="sxs-lookup"><span data-stu-id="aa45c-133">id</span></span>          | <span data-ttu-id="aa45c-134">String</span><span class="sxs-lookup"><span data-stu-id="aa45c-134">String</span></span> | <span data-ttu-id="aa45c-135">连接内外部组的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="aa45c-135">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="aa45c-136">它必须是字母数字，并且最多为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="aa45c-136">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="aa45c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="aa45c-137">displayName</span></span> | <span data-ttu-id="aa45c-138">String</span><span class="sxs-lookup"><span data-stu-id="aa45c-138">String</span></span> | <span data-ttu-id="aa45c-139">外部组的友好名称。</span><span class="sxs-lookup"><span data-stu-id="aa45c-139">The friendly name of the external group.</span></span> <span data-ttu-id="aa45c-140">可选。</span><span class="sxs-lookup"><span data-stu-id="aa45c-140">Optional.</span></span>                                                                      |
| <span data-ttu-id="aa45c-141">说明</span><span class="sxs-lookup"><span data-stu-id="aa45c-141">description</span></span> | <span data-ttu-id="aa45c-142">String</span><span class="sxs-lookup"><span data-stu-id="aa45c-142">String</span></span> | <span data-ttu-id="aa45c-143">外部组的说明。</span><span class="sxs-lookup"><span data-stu-id="aa45c-143">The description of the external group.</span></span> <span data-ttu-id="aa45c-144">可选。</span><span class="sxs-lookup"><span data-stu-id="aa45c-144">Optional.</span></span>                                                                         |

## <a name="response"></a><span data-ttu-id="aa45c-145">响应</span><span class="sxs-lookup"><span data-stu-id="aa45c-145">Response</span></span>

<span data-ttu-id="aa45c-146">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [externalGroup](../resources/externalconnectors-externalgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aa45c-146">If successful, this method returns a `201 Created` response code and an [externalGroup](../resources/externalconnectors-externalgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aa45c-147">示例</span><span class="sxs-lookup"><span data-stu-id="aa45c-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aa45c-148">请求</span><span class="sxs-lookup"><span data-stu-id="aa45c-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="aa45c-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa45c-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroup_from_connection"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups
Content-Type: application/json

{
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
# <a name="c"></a>[<span data-ttu-id="aa45c-150">C#</span><span class="sxs-lookup"><span data-stu-id="aa45c-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroup-from-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa45c-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa45c-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroup-from-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa45c-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa45c-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroup-from-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa45c-153">Java</span><span class="sxs-lookup"><span data-stu-id="aa45c-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroup-from-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="aa45c-154">响应</span><span class="sxs-lookup"><span data-stu-id="aa45c-154">Response</span></span>

<span data-ttu-id="aa45c-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aa45c-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
