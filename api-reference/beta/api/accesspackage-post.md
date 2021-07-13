---
title: 创建 accessPackage
description: 创建新的 accessPackage。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ccbe9c22f04087431ba0b4ae4df53eca1ff76a04
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400955"
---
# <a name="create-accesspackage"></a><span data-ttu-id="97904-103">创建 accessPackage</span><span class="sxs-lookup"><span data-stu-id="97904-103">Create accessPackage</span></span>

<span data-ttu-id="97904-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97904-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97904-105">创建新的 [accessPackage](../resources/accesspackage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="97904-105">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

<span data-ttu-id="97904-106">访问包将添加到现有的 [accessPackageCatalog](../resources/accesspackagecatalog.md)。</span><span class="sxs-lookup"><span data-stu-id="97904-106">The access package will be added to an existing [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span> <span data-ttu-id="97904-107">创建访问包后，可以创建 [accessPackageAssignmentPolicies，](../resources/accesspackageassignmentpolicy.md) 以指定如何向访问包分配用户。</span><span class="sxs-lookup"><span data-stu-id="97904-107">After the access package is created, you can then create [accessPackageAssignmentPolicies](../resources/accesspackageassignmentpolicy.md) which specify how users are assigned to the access package.</span></span>


## <a name="permissions"></a><span data-ttu-id="97904-108">权限</span><span class="sxs-lookup"><span data-stu-id="97904-108">Permissions</span></span>

<span data-ttu-id="97904-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97904-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97904-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="97904-111">Permission type</span></span>                        | <span data-ttu-id="97904-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97904-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="97904-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97904-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="97904-114">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97904-114">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="97904-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97904-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97904-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="97904-116">Not supported.</span></span> |
| <span data-ttu-id="97904-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="97904-117">Application</span></span>                            | <span data-ttu-id="97904-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97904-118">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97904-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97904-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="97904-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="97904-120">Request headers</span></span>

| <span data-ttu-id="97904-121">名称</span><span class="sxs-lookup"><span data-stu-id="97904-121">Name</span></span>          | <span data-ttu-id="97904-122">说明</span><span class="sxs-lookup"><span data-stu-id="97904-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="97904-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="97904-123">Authorization</span></span> | <span data-ttu-id="97904-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="97904-p103">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="97904-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="97904-126">Content-type</span></span>  | <span data-ttu-id="97904-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="97904-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97904-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="97904-129">Request body</span></span>

<span data-ttu-id="97904-130">在请求正文中，提供 [accessPackage](../resources/accesspackage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97904-130">In the request body, supply a JSON representation of an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="97904-131">响应</span><span class="sxs-lookup"><span data-stu-id="97904-131">Response</span></span>

<span data-ttu-id="97904-132">如果成功，此方法在响应正文中返回 201 Created 响应代码和新 [accessPackage](../resources/accesspackage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="97904-132">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="97904-133">示例</span><span class="sxs-lookup"><span data-stu-id="97904-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="97904-134">请求</span><span class="sxs-lookup"><span data-stu-id="97904-134">Request</span></span>

<span data-ttu-id="97904-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="97904-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="97904-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="97904-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackage_from_accesspackages"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
Content-type: application/json

{
  "catalogId": "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  "displayName": "sales reps",
  "description": "outside sales representatives"
}
```
# <a name="c"></a>[<span data-ttu-id="97904-137">C#</span><span class="sxs-lookup"><span data-stu-id="97904-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackage-from-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97904-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97904-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackage-from-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97904-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97904-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackage-from-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97904-140">Java</span><span class="sxs-lookup"><span data-stu-id="97904-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackage-from-accesspackages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="97904-141">响应</span><span class="sxs-lookup"><span data-stu-id="97904-141">Response</span></span>

<span data-ttu-id="97904-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="97904-142">The following is an example of the response.</span></span>

> <span data-ttu-id="97904-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="97904-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "catalogId": "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  "displayName": "sales reps",
  "description": "outside sales representatives",
  "isHidden": false,
  "isRoleScopesVisible": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


