---
title: 创建 accessPackageResourceRequest
description: 创建新的 accessPackageResourceRequest。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 70699361c862a2c372eca68649db516b111533f0
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176333"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="17fa8-103">创建 accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="17fa8-103">Create accessPackageResourceRequest</span></span>

<span data-ttu-id="17fa8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17fa8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17fa8-105">创建新的 [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) 对象，以请求向访问包目录添加资源，或者从目录中删除资源。</span><span class="sxs-lookup"><span data-stu-id="17fa8-105">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog, or the removal of a resource from a catalog.</span></span>

## <a name="permissions"></a><span data-ttu-id="17fa8-106">权限</span><span class="sxs-lookup"><span data-stu-id="17fa8-106">Permissions</span></span>

<span data-ttu-id="17fa8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17fa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="17fa8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="17fa8-109">Permission type</span></span>                        | <span data-ttu-id="17fa8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17fa8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="17fa8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17fa8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="17fa8-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17fa8-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="17fa8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17fa8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17fa8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="17fa8-114">Not supported.</span></span> |
| <span data-ttu-id="17fa8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="17fa8-115">Application</span></span>                            | <span data-ttu-id="17fa8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="17fa8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17fa8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17fa8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="17fa8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="17fa8-118">Request headers</span></span>

| <span data-ttu-id="17fa8-119">名称</span><span class="sxs-lookup"><span data-stu-id="17fa8-119">Name</span></span>          | <span data-ttu-id="17fa8-120">说明</span><span class="sxs-lookup"><span data-stu-id="17fa8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="17fa8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="17fa8-121">Authorization</span></span> | <span data-ttu-id="17fa8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17fa8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="17fa8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17fa8-124">Content-Type</span></span>  | <span data-ttu-id="17fa8-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="17fa8-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="17fa8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="17fa8-127">Request body</span></span>

<span data-ttu-id="17fa8-128">在请求正文中，提供 [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17fa8-128">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="17fa8-129">包含 `accessPackageResource` 与 [accessPackageResource](../resources/accesspackageresource.md) 对象的关系作为请求的一部分。</span><span class="sxs-lookup"><span data-stu-id="17fa8-129">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="17fa8-130">若要将 Azure AD 组作为资源添加到目录，请设置 **catalogId** 为目录 **ID、requestType** 为和 `AdminAdd` 表示 `accessPackageResource` 资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="17fa8-130">To add an Azure AD group as a resource to a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminAdd`, and an `accessPackageResource` representing the resource.</span></span> <span data-ttu-id="17fa8-131">内的 **originSystem** 属性的值 `accessPackageResource` 应为 `AadGroup` **，originId** 的值是组的标识符。</span><span class="sxs-lookup"><span data-stu-id="17fa8-131">The value of the **originSystem** property within the `accessPackageResource` should be `AadGroup` and the value of the **originId** is the identifier of the group.</span></span>

<span data-ttu-id="17fa8-132">若要从目录中删除 Azure AD 应用，请设置 **catalogId** 作为目录的 **ID、requestType** 和要删除 `AdminRemove` `accessPackageResource` 的资源对象。</span><span class="sxs-lookup"><span data-stu-id="17fa8-132">To remove an Azure AD app from a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminRemove`, and the `accessPackageResource` the resource object to be removed.</span></span>  <span data-ttu-id="17fa8-133">可以使用列表 [accessPackageResources 检索资源对象](accesspackagecatalog-list-accesspackageresources.md)。</span><span class="sxs-lookup"><span data-stu-id="17fa8-133">The resource object can be retrieved using [list accessPackageResources](accesspackagecatalog-list-accesspackageresources.md).</span></span>

<span data-ttu-id="17fa8-134">若要为多地理位置 Sharepoint Online 资源分配地理位置环境，请包含对象中的 **accessPackageResourceEnvironment** `accessPackageResource` 关系。</span><span class="sxs-lookup"><span data-stu-id="17fa8-134">To assign the geolocation environment for a multi-geolocation Sharepoint Online resource, include the **accessPackageResourceEnvironment** relationship in the `accessPackageResource` object.</span></span> <span data-ttu-id="17fa8-135">可通过两种方式完成此操作：</span><span class="sxs-lookup"><span data-stu-id="17fa8-135">This can be done in two ways:</span></span>
+ <span data-ttu-id="17fa8-136">使用 `@odata.bind` 批注将 `id` 对象 `accessPackageResourceEnvironment` 分配给 `accessPackageResourceEnvironment` 对象。</span><span class="sxs-lookup"><span data-stu-id="17fa8-136">Use `@odata.bind` annotation to assign the `id` of the `accessPackageResourceEnvironment` to an `accessPackageResourceEnvironment` object.</span></span>
+ <span data-ttu-id="17fa8-137">指定 `originId` 对象 `accessPackageResourceEnvironment` 中的参数 `accessPackageResourceEnvironment` 。</span><span class="sxs-lookup"><span data-stu-id="17fa8-137">Specify the `originId` parameter of the `accessPackageResourceEnvironment` in an `accessPackageResourceEnvironment` object.</span></span>


## <a name="response"></a><span data-ttu-id="17fa8-138">响应</span><span class="sxs-lookup"><span data-stu-id="17fa8-138">Response</span></span>

<span data-ttu-id="17fa8-139">如果成功，此方法在响应正文中返回响应 `201 Created` 代码和新的 [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="17fa8-139">If successful, this method returns a `201 Created` response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="17fa8-140">示例</span><span class="sxs-lookup"><span data-stu-id="17fa8-140">Examples</span></span>

### <a name="example-1-create-an-accesspackageresourcerequest"></a><span data-ttu-id="17fa8-141">示例 1：创建 accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="17fa8-141">Example 1: Create an accessPackageResourceRequest</span></span>

#### <a name="request"></a><span data-ttu-id="17fa8-142">请求</span><span class="sxs-lookup"><span data-stu-id="17fa8-142">Request</span></span>

<span data-ttu-id="17fa8-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="17fa8-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="17fa8-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="17fa8-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="17fa8-145">C#</span><span class="sxs-lookup"><span data-stu-id="17fa8-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17fa8-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17fa8-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17fa8-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17fa8-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17fa8-148">Java</span><span class="sxs-lookup"><span data-stu-id="17fa8-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="17fa8-149">响应</span><span class="sxs-lookup"><span data-stu-id="17fa8-149">Response</span></span>

<span data-ttu-id="17fa8-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="17fa8-150">The following is an example of the response.</span></span>

> <span data-ttu-id="17fa8-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="17fa8-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-an-accesspackageresourcerequest-for-a-resource-and-assign-an-accesspackageresourceenvironment-using-odatabind"></a><span data-ttu-id="17fa8-153">示例 2：为资源创建 accessPackageResourceRequest，然后使用 @odata.bind 分配 accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="17fa8-153">Example 2: Create an accessPackageResourceRequest for a resource and assign an accessPackageResourceEnvironment using @odata.bind</span></span>

#### <a name="request"></a><span data-ttu-id="17fa8-154">请求</span><span class="sxs-lookup"><span data-stu-id="17fa8-154">Request</span></span>

<span data-ttu-id="17fa8-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="17fa8-155">The following is an example of the request.</span></span> <span data-ttu-id="17fa8-156">本示例中， `@odata.bind` 批注用于将对象 `id` `accessPackageResourceEnvironment` 分配给 `accessPackageResourceEnvironment` 对象。</span><span class="sxs-lookup"><span data-stu-id="17fa8-156">In this example, the `@odata.bind` annotation is used to assign the `id` of the `accessPackageResourceEnvironment` to an `accessPackageResourceEnvironment` object.</span></span>



# <a name="http"></a>[<span data-ttu-id="17fa8-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="17fa8-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="17fa8-158">C#</span><span class="sxs-lookup"><span data-stu-id="17fa8-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17fa8-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17fa8-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17fa8-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17fa8-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17fa8-161">Java</span><span class="sxs-lookup"><span data-stu-id="17fa8-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="17fa8-162">响应</span><span class="sxs-lookup"><span data-stu-id="17fa8-162">Response</span></span>

<span data-ttu-id="17fa8-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="17fa8-163">The following is an example of the response.</span></span>

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

### <a name="example-3-create-an-accesspackageresourcerequest-for-a-resource-and-assign-an-accesspackageresourceenvironment-using-originid"></a><span data-ttu-id="17fa8-164">示例 3：为资源创建 accessPackageResourceRequest，然后使用 originId 分配 accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="17fa8-164">Example 3: Create an accessPackageResourceRequest for a resource and assign an accessPackageResourceEnvironment using originId</span></span>

#### <a name="request"></a><span data-ttu-id="17fa8-165">请求</span><span class="sxs-lookup"><span data-stu-id="17fa8-165">Request</span></span>

<span data-ttu-id="17fa8-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="17fa8-166">The following is an example of the request.</span></span> <span data-ttu-id="17fa8-167">本示例中，在对象 `accessPackageResourceEnvironment` 中指定参数 `accessPackageResourceEnvironment` 。</span><span class="sxs-lookup"><span data-stu-id="17fa8-167">In this example, the parameters of an `accessPackageResourceEnvironment` are specified in an `accessPackageResourceEnvironment` object.</span></span>



# <a name="http"></a>[<span data-ttu-id="17fa8-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="17fa8-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="17fa8-169">C#</span><span class="sxs-lookup"><span data-stu-id="17fa8-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17fa8-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17fa8-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17fa8-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17fa8-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17fa8-172">Java</span><span class="sxs-lookup"><span data-stu-id="17fa8-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-with-accesspackageresourceenvironment-new-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="17fa8-173">响应</span><span class="sxs-lookup"><span data-stu-id="17fa8-173">Response</span></span>

<span data-ttu-id="17fa8-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="17fa8-174">The following is an example of the response.</span></span>

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
