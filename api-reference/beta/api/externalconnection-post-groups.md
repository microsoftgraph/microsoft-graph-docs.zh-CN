---
title: 创建 externalGroup
description: 创建新的 externalGroup 对象。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6ca8968daf3abb98bba66a4146fc3b41c9d54441
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873043"
---
# <a name="create-externalgroup"></a><span data-ttu-id="b2759-103">创建 externalGroup</span><span class="sxs-lookup"><span data-stu-id="b2759-103">Create externalGroup</span></span>

<span data-ttu-id="b2759-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2759-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2759-105">创建新的 [externalGroup](../resources/externalgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2759-105">Create a new [externalGroup](../resources/externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2759-106">权限</span><span class="sxs-lookup"><span data-stu-id="b2759-106">Permissions</span></span>

<span data-ttu-id="b2759-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2759-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2759-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2759-109">Permission type</span></span>                        | <span data-ttu-id="b2759-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2759-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b2759-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2759-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2759-112">不支持</span><span class="sxs-lookup"><span data-stu-id="b2759-112">Not supported</span></span>                               |
| <span data-ttu-id="b2759-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2759-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2759-114">不支持</span><span class="sxs-lookup"><span data-stu-id="b2759-114">Not supported</span></span>                               |
| <span data-ttu-id="b2759-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2759-115">Application</span></span>                            | <span data-ttu-id="b2759-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2759-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="b2759-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2759-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionId}/groups
```

## <a name="request-headers"></a><span data-ttu-id="b2759-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2759-118">Request headers</span></span>

| <span data-ttu-id="b2759-119">名称</span><span class="sxs-lookup"><span data-stu-id="b2759-119">Name</span></span>          | <span data-ttu-id="b2759-120">说明</span><span class="sxs-lookup"><span data-stu-id="b2759-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="b2759-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2759-121">Authorization</span></span> | <span data-ttu-id="b2759-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2759-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b2759-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b2759-124">Content-Type</span></span>  | <span data-ttu-id="b2759-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b2759-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2759-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2759-127">Request body</span></span>

<span data-ttu-id="b2759-128">在请求正文中，提供 [externalGroup](../resources/externalgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2759-128">In the request body, supply a JSON representation of the [externalGroup](../resources/externalgroup.md) object.</span></span>

<span data-ttu-id="b2759-129">下表显示创建 [externalGroup](../resources/externalgroup.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b2759-129">The following table shows the properties that are required when you create the [externalGroup](../resources/externalgroup.md).</span></span>

| <span data-ttu-id="b2759-130">属性</span><span class="sxs-lookup"><span data-stu-id="b2759-130">Property</span></span>    | <span data-ttu-id="b2759-131">类型</span><span class="sxs-lookup"><span data-stu-id="b2759-131">Type</span></span>   | <span data-ttu-id="b2759-132">说明</span><span class="sxs-lookup"><span data-stu-id="b2759-132">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b2759-133">id</span><span class="sxs-lookup"><span data-stu-id="b2759-133">id</span></span>          | <span data-ttu-id="b2759-134">String</span><span class="sxs-lookup"><span data-stu-id="b2759-134">String</span></span> | <span data-ttu-id="b2759-135">连接内外部组的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="b2759-135">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="b2759-136">它必须是字母数字，并且最多为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="b2759-136">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="b2759-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b2759-137">displayName</span></span> | <span data-ttu-id="b2759-138">String</span><span class="sxs-lookup"><span data-stu-id="b2759-138">String</span></span> | <span data-ttu-id="b2759-139">外部组的友好名称。</span><span class="sxs-lookup"><span data-stu-id="b2759-139">The friendly name of the external group.</span></span> <span data-ttu-id="b2759-140">可选。</span><span class="sxs-lookup"><span data-stu-id="b2759-140">Optional.</span></span>                                                                      |
| <span data-ttu-id="b2759-141">说明</span><span class="sxs-lookup"><span data-stu-id="b2759-141">description</span></span> | <span data-ttu-id="b2759-142">String</span><span class="sxs-lookup"><span data-stu-id="b2759-142">String</span></span> | <span data-ttu-id="b2759-143">外部组的说明。</span><span class="sxs-lookup"><span data-stu-id="b2759-143">The description of the external group.</span></span> <span data-ttu-id="b2759-144">可选。</span><span class="sxs-lookup"><span data-stu-id="b2759-144">Optional.</span></span>                                                                         |

## <a name="response"></a><span data-ttu-id="b2759-145">响应</span><span class="sxs-lookup"><span data-stu-id="b2759-145">Response</span></span>

<span data-ttu-id="b2759-146">如果成功，此方法在响应 `201 Created` 正文中返回响应代码和 [externalGroup](../resources/externalgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2759-146">If successful, this method returns a `201 Created` response code and an [externalGroup](../resources/externalgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b2759-147">示例</span><span class="sxs-lookup"><span data-stu-id="b2759-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b2759-148">请求</span><span class="sxs-lookup"><span data-stu-id="b2759-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b2759-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2759-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroup_from_connection"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
# <a name="c"></a>[<span data-ttu-id="b2759-150">C#</span><span class="sxs-lookup"><span data-stu-id="b2759-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroup-from-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2759-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2759-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroup-from-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2759-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2759-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroup-from-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2759-153">Java</span><span class="sxs-lookup"><span data-stu-id="b2759-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroup-from-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="b2759-154">响应</span><span class="sxs-lookup"><span data-stu-id="b2759-154">Response</span></span>

<span data-ttu-id="b2759-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b2759-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroup"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
