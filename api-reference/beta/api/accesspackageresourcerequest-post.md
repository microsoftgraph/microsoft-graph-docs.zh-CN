---
title: 创建 accessPackageResourceRequest
description: 创建新的 accessPackageResourceRequest。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7766eb9f6468ee93ce63a034b501e17d9653541a
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439132"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="57961-103">创建 accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="57961-103">Create accessPackageResourceRequest</span></span>

<span data-ttu-id="57961-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57961-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57961-105">创建新的 [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) 对象，以请求向访问包目录添加资源，或者从目录中删除资源。</span><span class="sxs-lookup"><span data-stu-id="57961-105">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog, or the removal of a resource from a catalog.</span></span>  <span data-ttu-id="57961-106">必须先将资源包含在访问包目录中，然后才能将资源的角色添加到访问包中。</span><span class="sxs-lookup"><span data-stu-id="57961-106">A resource must be included in an access package catalog before the role of that resource can be added to an access package.</span></span>

## <a name="permissions"></a><span data-ttu-id="57961-107">权限</span><span class="sxs-lookup"><span data-stu-id="57961-107">Permissions</span></span>

<span data-ttu-id="57961-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57961-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57961-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="57961-110">Permission type</span></span>                        | <span data-ttu-id="57961-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57961-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="57961-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57961-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="57961-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57961-113">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="57961-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57961-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57961-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="57961-115">Not supported.</span></span> |
| <span data-ttu-id="57961-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="57961-116">Application</span></span>                            | <span data-ttu-id="57961-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="57961-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="57961-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57961-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="57961-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="57961-119">Request headers</span></span>

| <span data-ttu-id="57961-120">名称</span><span class="sxs-lookup"><span data-stu-id="57961-120">Name</span></span>          | <span data-ttu-id="57961-121">说明</span><span class="sxs-lookup"><span data-stu-id="57961-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="57961-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="57961-122">Authorization</span></span> | <span data-ttu-id="57961-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="57961-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57961-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57961-125">Content-Type</span></span>  | <span data-ttu-id="57961-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="57961-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="57961-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="57961-128">Request body</span></span>

<span data-ttu-id="57961-129">在请求正文中，提供 [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57961-129">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="57961-130">在 `accessPackageResource` 请求中包括与 [accessPackageResource](../resources/accesspackageresource.md) 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="57961-130">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="57961-131">若要将 Azure AD 组作为资源添加到目录，将 **catalogId** 设置为目录的 ID，将 **requestType** 设置为 ，将 `AdminAdd` 设置为 表示 `accessPackageResource` 资源的 。</span><span class="sxs-lookup"><span data-stu-id="57961-131">To add an Azure AD group as a resource to a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminAdd`, and an `accessPackageResource` representing the resource.</span></span> <span data-ttu-id="57961-132">内的 **originSystem** 属性的值 `accessPackageResource` 应为 `AadGroup` **，originId** 的值是组的标识符。</span><span class="sxs-lookup"><span data-stu-id="57961-132">The value of the **originSystem** property within the `accessPackageResource` should be `AadGroup` and the value of the **originId** is the identifier of the group.</span></span>

<span data-ttu-id="57961-133">若要从目录中删除 Azure AD 应用，请设置 **catalogId** 为目录 ID， **将 requestType** 设置为 ，将 资源对象设置为 要 `AdminRemove` `accessPackageResource` 删除的资源对象。</span><span class="sxs-lookup"><span data-stu-id="57961-133">To remove an Azure AD app from a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminRemove`, and the `accessPackageResource` the resource object to be removed.</span></span>  <span data-ttu-id="57961-134">资源对象可以使用列表 [accessPackageResources 检索](accesspackagecatalog-list-accesspackageresources.md)。</span><span class="sxs-lookup"><span data-stu-id="57961-134">The resource object can be retrieved using [list accessPackageResources](accesspackagecatalog-list-accesspackageresources.md).</span></span>

<span data-ttu-id="57961-135">若要为多地理位置 Sharepoint Online 资源分配地理位置环境，请包含对象中的 **accessPackageResourceEnvironment** `accessPackageResource` 关系。</span><span class="sxs-lookup"><span data-stu-id="57961-135">To assign the geolocation environment for a multi-geolocation Sharepoint Online resource, include the **accessPackageResourceEnvironment** relationship in the `accessPackageResource` object.</span></span> <span data-ttu-id="57961-136">可通过两种方式完成此操作：</span><span class="sxs-lookup"><span data-stu-id="57961-136">This can be done in two ways:</span></span>
+ <span data-ttu-id="57961-137">使用 `@odata.bind` annotation 将 的 `id` `accessPackageResourceEnvironment` 分配给 `accessPackageResourceEnvironment` 对象。</span><span class="sxs-lookup"><span data-stu-id="57961-137">Use `@odata.bind` annotation to assign the `id` of the `accessPackageResourceEnvironment` to an `accessPackageResourceEnvironment` object.</span></span>
+ <span data-ttu-id="57961-138">指定 `originId` 对象中的 `accessPackageResourceEnvironment` 参数 `accessPackageResourceEnvironment` 。</span><span class="sxs-lookup"><span data-stu-id="57961-138">Specify the `originId` parameter of the `accessPackageResourceEnvironment` in an `accessPackageResourceEnvironment` object.</span></span>


## <a name="response"></a><span data-ttu-id="57961-139">响应</span><span class="sxs-lookup"><span data-stu-id="57961-139">Response</span></span>

<span data-ttu-id="57961-140">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="57961-140">If successful, this method returns a `201 Created` response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57961-141">示例</span><span class="sxs-lookup"><span data-stu-id="57961-141">Examples</span></span>

### <a name="example-1-create-an-accesspackageresourcerequest-for-adding-a-site-as-a-resource"></a><span data-ttu-id="57961-142">示例 1：创建 accessPackageResourceRequest 以将网站添加为资源</span><span class="sxs-lookup"><span data-stu-id="57961-142">Example 1: Create an accessPackageResourceRequest for adding a site as a resource</span></span>

#### <a name="request"></a><span data-ttu-id="57961-143">请求</span><span class="sxs-lookup"><span data-stu-id="57961-143">Request</span></span>

<span data-ttu-id="57961-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="57961-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="57961-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="57961-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="57961-146">C#</span><span class="sxs-lookup"><span data-stu-id="57961-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57961-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57961-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57961-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57961-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57961-149">Java</span><span class="sxs-lookup"><span data-stu-id="57961-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="57961-150">响应</span><span class="sxs-lookup"><span data-stu-id="57961-150">Response</span></span>

<span data-ttu-id="57961-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="57961-151">The following is an example of the response.</span></span>

> <span data-ttu-id="57961-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="57961-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-an-accesspackageresourcerequest-for-adding-a-site-as-a-resource-and-assign-an-accesspackageresourceenvironment-using-odatabind"></a><span data-ttu-id="57961-153">示例 2：创建 accessPackageResourceRequest 以将网站添加为资源，然后使用 @odata.bind 分配 accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="57961-153">Example 2: Create an accessPackageResourceRequest for adding a site as a resource and assign an accessPackageResourceEnvironment using @odata.bind</span></span>

#### <a name="request"></a><span data-ttu-id="57961-154">请求</span><span class="sxs-lookup"><span data-stu-id="57961-154">Request</span></span>

<span data-ttu-id="57961-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="57961-155">The following is an example of the request.</span></span> <span data-ttu-id="57961-156">本示例中， `@odata.bind` 批注用于将 分配给 `id` `accessPackageResourceEnvironment` `accessPackageResourceEnvironment` 对象。</span><span class="sxs-lookup"><span data-stu-id="57961-156">In this example, the `@odata.bind` annotation is used to assign the `id` of the `accessPackageResourceEnvironment` to an `accessPackageResourceEnvironment` object.</span></span>



# <a name="http"></a>[<span data-ttu-id="57961-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="57961-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="57961-158">C#</span><span class="sxs-lookup"><span data-stu-id="57961-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57961-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57961-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57961-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57961-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57961-161">Java</span><span class="sxs-lookup"><span data-stu-id="57961-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="57961-162">响应</span><span class="sxs-lookup"><span data-stu-id="57961-162">Response</span></span>

<span data-ttu-id="57961-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="57961-163">The following is an example of the response.</span></span>

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

### <a name="example-3-create-an-accesspackageresourcerequest-for-adding-a-site-as-a-resource-and-assign-an-accesspackageresourceenvironment-using-originid"></a><span data-ttu-id="57961-164">示例 3：创建 accessPackageResourceRequest 以将网站添加为资源，然后使用 originId 分配 accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="57961-164">Example 3: Create an accessPackageResourceRequest for adding a site as a resource and assign an accessPackageResourceEnvironment using originId</span></span>

#### <a name="request"></a><span data-ttu-id="57961-165">请求</span><span class="sxs-lookup"><span data-stu-id="57961-165">Request</span></span>

<span data-ttu-id="57961-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="57961-166">The following is an example of the request.</span></span> <span data-ttu-id="57961-167">本示例在对象中 `accessPackageResourceEnvironment` 指定 的参数 `accessPackageResourceEnvironment` 。</span><span class="sxs-lookup"><span data-stu-id="57961-167">In this example, the parameters of an `accessPackageResourceEnvironment` are specified in an `accessPackageResourceEnvironment` object.</span></span>



# <a name="http"></a>[<span data-ttu-id="57961-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="57961-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="57961-169">C#</span><span class="sxs-lookup"><span data-stu-id="57961-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57961-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57961-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57961-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57961-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57961-172">Java</span><span class="sxs-lookup"><span data-stu-id="57961-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="57961-173">响应</span><span class="sxs-lookup"><span data-stu-id="57961-173">Response</span></span>

<span data-ttu-id="57961-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="57961-174">The following is an example of the response.</span></span>

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

### <a name="example-4-create-an-accesspackageresourcerequest-for-adding-a-group-as-a-resource"></a><span data-ttu-id="57961-175">示例 4：创建 accessPackageResourceRequest 以将组添加为资源</span><span class="sxs-lookup"><span data-stu-id="57961-175">Example 4: Create an accessPackageResourceRequest for adding a group as a resource</span></span>

#### <a name="request"></a><span data-ttu-id="57961-176">请求</span><span class="sxs-lookup"><span data-stu-id="57961-176">Request</span></span>

<span data-ttu-id="57961-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="57961-177">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="57961-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="57961-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests4"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{

  "catalogId":"beedadfe-01d5-4025-910b-84abb9369997",
  "requestType": "AdminAdd",
  "accessPackageResource": {
     "originId": "c6294667-7348-4f5a-be73-9d2c65f574f3",
     "originSystem": "AadGroup"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="57961-179">C#</span><span class="sxs-lookup"><span data-stu-id="57961-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57961-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57961-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57961-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57961-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57961-182">Java</span><span class="sxs-lookup"><span data-stu-id="57961-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="57961-183">响应</span><span class="sxs-lookup"><span data-stu-id="57961-183">Response</span></span>

<span data-ttu-id="57961-184">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="57961-184">The following is an example of the response.</span></span>

> <span data-ttu-id="57961-185">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="57961-185">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
  "id": "acc2294e-f37f-42d3-981d-4e83847ed0ce",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled"
}
```

### <a name="example-5-create-an-accesspackageresourcerequest-for-removing-a-resource"></a><span data-ttu-id="57961-186">示例 5：创建用于删除资源的 accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="57961-186">Example 5: Create an accessPackageResourceRequest for removing a resource</span></span>

#### <a name="request"></a><span data-ttu-id="57961-187">请求</span><span class="sxs-lookup"><span data-stu-id="57961-187">Request</span></span>

<span data-ttu-id="57961-188">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="57961-188">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="57961-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="57961-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests5"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
  "requestType": "AdminRemove",
  "accessPackageResource": {
    "id": "354078e5-dbce-4894-8af4-0ab274d41662"
  }
}

```
# <a name="c"></a>[<span data-ttu-id="57961-190">C#</span><span class="sxs-lookup"><span data-stu-id="57961-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57961-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57961-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57961-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57961-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57961-193">Java</span><span class="sxs-lookup"><span data-stu-id="57961-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="57961-194">响应</span><span class="sxs-lookup"><span data-stu-id="57961-194">Response</span></span>

<span data-ttu-id="57961-195">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="57961-195">The following is an example of the response.</span></span>

> <span data-ttu-id="57961-196">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="57961-196">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
  "id": "65c3340d-defb-49a9-8930-63841fda0e68",
  "requestType": "AdminRemove",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled"
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
