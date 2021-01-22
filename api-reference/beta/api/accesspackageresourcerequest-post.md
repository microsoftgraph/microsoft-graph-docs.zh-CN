---
title: 创建 accessPackageResourceRequest
description: 创建新的 accessPackageResourceRequest。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e7ea15dbe0ec63e539246851ce853b83c40229aa
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934535"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="4b215-103">创建 accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="4b215-103">Create accessPackageResourceRequest</span></span>

<span data-ttu-id="4b215-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b215-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b215-105">创建新的 [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) 对象，以请求向访问包目录添加资源，或者从目录中删除资源。</span><span class="sxs-lookup"><span data-stu-id="4b215-105">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog, or the removal of a resource from a catalog.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b215-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4b215-106">Permissions</span></span>

<span data-ttu-id="4b215-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b215-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b215-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b215-109">Permission type</span></span>                        | <span data-ttu-id="4b215-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b215-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b215-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b215-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="4b215-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b215-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="4b215-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b215-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b215-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b215-114">Not supported.</span></span> |
| <span data-ttu-id="4b215-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b215-115">Application</span></span>                            | <span data-ttu-id="4b215-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b215-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b215-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b215-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="4b215-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b215-118">Request headers</span></span>

| <span data-ttu-id="4b215-119">名称</span><span class="sxs-lookup"><span data-stu-id="4b215-119">Name</span></span>          | <span data-ttu-id="4b215-120">说明</span><span class="sxs-lookup"><span data-stu-id="4b215-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4b215-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b215-121">Authorization</span></span> | <span data-ttu-id="4b215-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b215-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b215-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b215-124">Content-Type</span></span>  | <span data-ttu-id="4b215-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4b215-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4b215-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b215-127">Request body</span></span>

<span data-ttu-id="4b215-128">在请求正文中，提供 [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b215-128">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="4b215-129">包含 `accessPackageResource` 与 [accessPackageResource](../resources/accesspackageresource.md) 对象的关系作为请求的一部分。</span><span class="sxs-lookup"><span data-stu-id="4b215-129">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="4b215-130">若要将 Azure AD 组作为资源添加到目录，请设置 **catalogId** 为目录 **ID、requestType** 为和 `AdminAdd` 表示 `accessPackageResource` 资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="4b215-130">To add an Azure AD group as a resource to a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminAdd`, and an `accessPackageResource` representing the resource.</span></span> <span data-ttu-id="4b215-131">内的 **originSystem** 属性的值 `accessPackageResource` 应为 `AadGroup` **，originId** 的值是组的标识符。</span><span class="sxs-lookup"><span data-stu-id="4b215-131">The value of the **originSystem** property within the `accessPackageResource` should be `AadGroup` and the value of the **originId** is the identifier of the group.</span></span>

<span data-ttu-id="4b215-132">若要从目录中删除 Azure AD 应用，请设置 **catalogId** 作为目录的 **ID、requestType** 和要 `AdminRemove` `accessPackageResource` 删除的资源对象。</span><span class="sxs-lookup"><span data-stu-id="4b215-132">To remove an Azure AD app from a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminRemove`, and the `accessPackageResource` the resource object to be removed.</span></span>  <span data-ttu-id="4b215-133">可以使用列表 [accessPackageResources 检索资源对象](accesspackagecatalog-list-accesspackageresources.md)。</span><span class="sxs-lookup"><span data-stu-id="4b215-133">The resource object can be retrieved using [list accessPackageResources](accesspackagecatalog-list-accesspackageresources.md).</span></span>


## <a name="response"></a><span data-ttu-id="4b215-134">响应</span><span class="sxs-lookup"><span data-stu-id="4b215-134">Response</span></span>

<span data-ttu-id="4b215-135">如果成功，此方法在响应正文中返回 200 系列响应代码和新的 [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b215-135">If successful, this method returns a 200-series response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b215-136">示例</span><span class="sxs-lookup"><span data-stu-id="4b215-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4b215-137">请求</span><span class="sxs-lookup"><span data-stu-id="4b215-137">Request</span></span>

<span data-ttu-id="4b215-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4b215-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b215-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b215-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId":"26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "requestType": "AdminAdd",
  "justification": "",
  "accessPackageResource": {
     "displayName": "Sales",
     "description": "https://contoso.sharepoint.com/sites/Sales",
     "url": "https://contoso.sharepoint.com/sites/Sales",
     "resourceType": "SharePoint Online Site",
     "originId": "https://contoso.sharepoint.com/sites/Sales",
     "originSystem": "SharePointOnline"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4b215-140">C#</span><span class="sxs-lookup"><span data-stu-id="4b215-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b215-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b215-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b215-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b215-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b215-143">Java</span><span class="sxs-lookup"><span data-stu-id="4b215-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4b215-144">响应</span><span class="sxs-lookup"><span data-stu-id="4b215-144">Response</span></span>

<span data-ttu-id="4b215-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4b215-145">The following is an example of the response.</span></span>

> <span data-ttu-id="4b215-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4b215-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
  "isValidationOnly": false,
  "justification": "",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "requestType": "AdminAdd"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageResourceRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


