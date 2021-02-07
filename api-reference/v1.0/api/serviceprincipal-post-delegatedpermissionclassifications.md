---
title: 创建 delegatedPermissionClassification
description: 通过将 delegatedPermissionClassification 添加到 API 的服务主体来对权限进行分类。
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: c8ec9f622adcbd823df3219cea8876e8077d8977
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128706"
---
# <a name="create-delegatedpermissionclassification"></a><span data-ttu-id="5910e-103">创建 delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="5910e-103">Create delegatedPermissionClassification</span></span>

<span data-ttu-id="5910e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5910e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5910e-105">通过将 [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) 添加到表示 API 的 [servicePrincipal，](../resources/servicePrincipal.md) 对委派权限进行分类。</span><span class="sxs-lookup"><span data-stu-id="5910e-105">Classify a delegated permission by adding a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) to the [servicePrincipal](../resources/servicePrincipal.md) representing the API.</span></span>

## <a name="permissions"></a><span data-ttu-id="5910e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="5910e-106">Permissions</span></span>

<span data-ttu-id="5910e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5910e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5910e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5910e-109">Permission type</span></span>      | <span data-ttu-id="5910e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5910e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5910e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5910e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5910e-112">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5910e-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="5910e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5910e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5910e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5910e-114">Not supported.</span></span>    |
|<span data-ttu-id="5910e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5910e-115">Application</span></span> | <span data-ttu-id="5910e-116">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5910e-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5910e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5910e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="request-headers"></a><span data-ttu-id="5910e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5910e-118">Request headers</span></span>

| <span data-ttu-id="5910e-119">名称</span><span class="sxs-lookup"><span data-stu-id="5910e-119">Name</span></span>       | <span data-ttu-id="5910e-120">说明</span><span class="sxs-lookup"><span data-stu-id="5910e-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="5910e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5910e-121">Authorization</span></span> | <span data-ttu-id="5910e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5910e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5910e-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="5910e-124">Content-type</span></span> | <span data-ttu-id="5910e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5910e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5910e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5910e-127">Request body</span></span>

<span data-ttu-id="5910e-128">在请求正文中，提供 [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5910e-128">In the request body, supply a JSON representation of an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5910e-129">响应</span><span class="sxs-lookup"><span data-stu-id="5910e-129">Response</span></span>

<span data-ttu-id="5910e-130">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5910e-130">If successful, this method returns a `201 Created` response code and an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5910e-131">示例</span><span class="sxs-lookup"><span data-stu-id="5910e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5910e-132">请求</span><span class="sxs-lookup"><span data-stu-id="5910e-132">Request</span></span>

<span data-ttu-id="5910e-133">在下面的示例中，委派权限"User.Read"被分类为"低"。</span><span class="sxs-lookup"><span data-stu-id="5910e-133">In the following example, the delegated permission "User.Read" is being classified "low".</span></span>


# <a name="http"></a>[<span data-ttu-id="5910e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5910e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_delegatedpermissionclassification"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/delegatedPermissionClassifications
Content-Type: application/json

{
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```
# <a name="c"></a>[<span data-ttu-id="5910e-135">C#</span><span class="sxs-lookup"><span data-stu-id="5910e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-delegatedpermissionclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5910e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5910e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-delegatedpermissionclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5910e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5910e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-delegatedpermissionclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5910e-138">Java</span><span class="sxs-lookup"><span data-stu-id="5910e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-delegatedpermissionclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5910e-139">响应</span><span class="sxs-lookup"><span data-stu-id="5910e-139">Response</span></span>

<span data-ttu-id="5910e-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5910e-140">The following is an example of the response.</span></span>

> <span data-ttu-id="5910e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5910e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.delegatedPermissionClassification"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "2G3-4TG6YU2J54hjnaRoPQE",
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```
