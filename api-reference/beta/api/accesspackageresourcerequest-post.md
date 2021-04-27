---
title: 创建 accessPackageResourceRequest
description: 创建新的 accessPackageResourceRequest。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e0d85470f8217887364d8c37e760945205edec51
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048524"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="99659-103">创建 accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="99659-103">Create accessPackageResourceRequest</span></span>

<span data-ttu-id="99659-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99659-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99659-105">创建新的 [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) 对象，以请求向访问包目录添加资源，或者从目录中删除资源。</span><span class="sxs-lookup"><span data-stu-id="99659-105">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog, or the removal of a resource from a catalog.</span></span>

## <a name="permissions"></a><span data-ttu-id="99659-106">权限</span><span class="sxs-lookup"><span data-stu-id="99659-106">Permissions</span></span>

<span data-ttu-id="99659-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99659-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99659-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="99659-109">Permission type</span></span>                        | <span data-ttu-id="99659-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99659-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="99659-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99659-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="99659-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99659-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="99659-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99659-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99659-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="99659-114">Not supported.</span></span> |
| <span data-ttu-id="99659-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="99659-115">Application</span></span>                            | <span data-ttu-id="99659-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="99659-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99659-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99659-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="99659-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="99659-118">Request headers</span></span>

| <span data-ttu-id="99659-119">名称</span><span class="sxs-lookup"><span data-stu-id="99659-119">Name</span></span>          | <span data-ttu-id="99659-120">说明</span><span class="sxs-lookup"><span data-stu-id="99659-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="99659-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="99659-121">Authorization</span></span> | <span data-ttu-id="99659-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="99659-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99659-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99659-124">Content-Type</span></span>  | <span data-ttu-id="99659-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="99659-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99659-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="99659-127">Request body</span></span>

<span data-ttu-id="99659-128">在请求正文中，提供 [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99659-128">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="99659-129">在 `accessPackageResource` 请求中包括与 [accessPackageResource](../resources/accesspackageresource.md) 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="99659-129">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="99659-130">若要将 Azure AD 组作为资源添加到目录，将 **catalogId** 设置为目录的 ID，将 **requestType** 设置为 ，将 `AdminAdd` 设置为 表示 `accessPackageResource` 资源的 。</span><span class="sxs-lookup"><span data-stu-id="99659-130">To add an Azure AD group as a resource to a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminAdd`, and an `accessPackageResource` representing the resource.</span></span> <span data-ttu-id="99659-131">内的 **originSystem** 属性的值 `accessPackageResource` 应为 `AadGroup` **，originId** 的值是组的标识符。</span><span class="sxs-lookup"><span data-stu-id="99659-131">The value of the **originSystem** property within the `accessPackageResource` should be `AadGroup` and the value of the **originId** is the identifier of the group.</span></span>

<span data-ttu-id="99659-132">若要从目录中删除 Azure AD 应用，请设置 **catalogId** 为目录 ID， **将 requestType** 设置为 ，将 资源对象设置为 要 `AdminRemove` `accessPackageResource` 删除的资源对象。</span><span class="sxs-lookup"><span data-stu-id="99659-132">To remove an Azure AD app from a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminRemove`, and the `accessPackageResource` the resource object to be removed.</span></span>  <span data-ttu-id="99659-133">资源对象可以使用列表 [accessPackageResources 检索](accesspackagecatalog-list-accesspackageresources.md)。</span><span class="sxs-lookup"><span data-stu-id="99659-133">The resource object can be retrieved using [list accessPackageResources](accesspackagecatalog-list-accesspackageresources.md).</span></span>

<span data-ttu-id="99659-134">若要为多地理位置 Sharepoint Online 资源分配地理位置环境，请包含对象中的 **accessPackageResourceEnvironment** `accessPackageResource` 关系。</span><span class="sxs-lookup"><span data-stu-id="99659-134">To assign the geolocation environment for a multi-geolocation Sharepoint Online resource, include the **accessPackageResourceEnvironment** relationship in the `accessPackageResource` object.</span></span> <span data-ttu-id="99659-135">可通过两种方式完成此操作：</span><span class="sxs-lookup"><span data-stu-id="99659-135">This can be done in two ways:</span></span>
+ <span data-ttu-id="99659-136">使用 `@odata.bind` annotation 将 的 `id` `accessPackageResourceEnvironment` 分配给 `accessPackageResourceEnvironment` 对象。</span><span class="sxs-lookup"><span data-stu-id="99659-136">Use `@odata.bind` annotation to assign the `id` of the `accessPackageResourceEnvironment` to an `accessPackageResourceEnvironment` object.</span></span>
+ <span data-ttu-id="99659-137">指定 `originId` 对象中的 `accessPackageResourceEnvironment` 参数 `accessPackageResourceEnvironment` 。</span><span class="sxs-lookup"><span data-stu-id="99659-137">Specify the `originId` parameter of the `accessPackageResourceEnvironment` in an `accessPackageResourceEnvironment` object.</span></span>


## <a name="response"></a><span data-ttu-id="99659-138">响应</span><span class="sxs-lookup"><span data-stu-id="99659-138">Response</span></span>

<span data-ttu-id="99659-139">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="99659-139">If successful, this method returns a `201 Created` response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="99659-140">示例</span><span class="sxs-lookup"><span data-stu-id="99659-140">Examples</span></span>

### <a name="example-1-create-an-accesspackageresourcerequest"></a><span data-ttu-id="99659-141">示例 1：创建 accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="99659-141">Example 1: Create an accessPackageResourceRequest</span></span>

#### <a name="request"></a><span data-ttu-id="99659-142">请求</span><span class="sxs-lookup"><span data-stu-id="99659-142">Request</span></span>

<span data-ttu-id="99659-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="99659-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99659-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="99659-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="99659-145">C#</span><span class="sxs-lookup"><span data-stu-id="99659-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99659-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99659-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99659-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99659-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99659-148">Java</span><span class="sxs-lookup"><span data-stu-id="99659-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="99659-149">响应</span><span class="sxs-lookup"><span data-stu-id="99659-149">Response</span></span>

<span data-ttu-id="99659-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="99659-150">The following is an example of the response.</span></span>

> <span data-ttu-id="99659-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="99659-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-an-accesspackageresourcerequest-for-a-resource-and-assign-an-accesspackageresourceenvironment-using-odatabind"></a><span data-ttu-id="99659-152">示例 2：为资源创建 accessPackageResourceRequest，然后使用 @odata.bind 分配 accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="99659-152">Example 2: Create an accessPackageResourceRequest for a resource and assign an accessPackageResourceEnvironment using @odata.bind</span></span>

#### <a name="request"></a><span data-ttu-id="99659-153">请求</span><span class="sxs-lookup"><span data-stu-id="99659-153">Request</span></span>

<span data-ttu-id="99659-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="99659-154">The following is an example of the request.</span></span> <span data-ttu-id="99659-155">本示例中， `@odata.bind` 批注用于将 分配给 `id` `accessPackageResourceEnvironment` `accessPackageResourceEnvironment` 对象。</span><span class="sxs-lookup"><span data-stu-id="99659-155">In this example, the `@odata.bind` annotation is used to assign the `id` of the `accessPackageResourceEnvironment` to an `accessPackageResourceEnvironment` object.</span></span>



# <a name="http"></a>[<span data-ttu-id="99659-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="99659-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests_with_accessPackageResourceEnvironment"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
    "catalogId": "de9315c1-272b-4905-924b-cc112ca180c7",
    "accessPackageResource": {
        "displayName": "Community Outreach",
        "description": "https://contoso.sharepoint.com/sites/CSR",
        "resourceType": "SharePoint Online Site",
        "originId": "https://contoso.sharepoint.com/sites/CSR",
        "originSystem": "SharePointOnline",
        "accessPackageResourceEnvironment@odata.bind": "accessPackageResourceEnvironments/615f2218-678f-471f-a60a-02c2f4f80c57"
    },
    "requestType": "AdminAdd"
}
```
# <a name="c"></a>[<span data-ttu-id="99659-157">C#</span><span class="sxs-lookup"><span data-stu-id="99659-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99659-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99659-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99659-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99659-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99659-160">Java</span><span class="sxs-lookup"><span data-stu-id="99659-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="99659-161">响应</span><span class="sxs-lookup"><span data-stu-id="99659-161">Response</span></span>

<span data-ttu-id="99659-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="99659-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceRequests/$entity",
    "catalogId": "de9315c1-272b-4905-924b-cc112ca180c7",
    "executeImmediately": false,
    "id": "d3f800d5-0dd6-47f3-9e90-ef562c7551dc",
    "requestType": "AdminAdd",
    "requestState": "Delivered",
    "requestStatus": "Fulfilled",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

### <a name="example-3-create-an-accesspackageresourcerequest-for-a-resource-and-assign-an-accesspackageresourceenvironment-using-originid"></a><span data-ttu-id="99659-163">示例 3：为资源创建 accessPackageResourceRequest，然后使用 originId 分配 accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="99659-163">Example 3: Create an accessPackageResourceRequest for a resource and assign an accessPackageResourceEnvironment using originId</span></span>

#### <a name="request"></a><span data-ttu-id="99659-164">请求</span><span class="sxs-lookup"><span data-stu-id="99659-164">Request</span></span>

<span data-ttu-id="99659-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="99659-165">The following is an example of the request.</span></span> <span data-ttu-id="99659-166">本示例在对象中 `accessPackageResourceEnvironment` 指定 的参数 `accessPackageResourceEnvironment` 。</span><span class="sxs-lookup"><span data-stu-id="99659-166">In this example, the parameters of an `accessPackageResourceEnvironment` are specified in an `accessPackageResourceEnvironment` object.</span></span>



# <a name="http"></a>[<span data-ttu-id="99659-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="99659-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests_with_accessPackageResourceEnvironment_New"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
    "catalogId": "de9315c1-272b-4905-924b-cc112ca180c7",
    "accessPackageResource": {
        "displayName": "Community Outreach",
        "description": "https://contoso.sharepoint.com/sites/CSR",
        "resourceType": "SharePoint Online Site",
        "originId": "https://contoso.sharepoint.com/sites/CSR",
        "originSystem": "SharePointOnline",
        "accessPackageResourceEnvironment": {
            "originId": "https://contoso-admin.sharepoint.com/"
        }
    },
    "requestType": "AdminAdd"
}
```
# <a name="c"></a>[<span data-ttu-id="99659-168">C#</span><span class="sxs-lookup"><span data-stu-id="99659-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99659-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99659-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99659-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99659-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99659-171">Java</span><span class="sxs-lookup"><span data-stu-id="99659-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="99659-172">响应</span><span class="sxs-lookup"><span data-stu-id="99659-172">Response</span></span>

<span data-ttu-id="99659-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="99659-173">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceRequests/$entity",
    "catalogId": "de9315c1-272b-4905-924b-cc112ca180c7",
    "executeImmediately": false,
    "id": "eadf3fbb-668c-4c3a-8d84-7c8bd73dc3e4",
    "requestType": "AdminAdd",
    "requestState": "Delivered",
    "requestStatus": "Fulfilled",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
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
