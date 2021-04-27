---
title: 列出 governanceResources
description: 检索请求者有权访问的 governanceResource 集合。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: d8f78f1e52c91981cef4f0be9a5101f2a7ef9feb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042196"
---
# <a name="list-governanceresources"></a><span data-ttu-id="6c157-103">列出 governanceResources</span><span class="sxs-lookup"><span data-stu-id="6c157-103">List governanceResources</span></span>

<span data-ttu-id="6c157-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c157-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c157-105">检索请求 [者有权访问的 governanceResource](../resources/governanceresource.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="6c157-105">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c157-106">权限</span><span class="sxs-lookup"><span data-stu-id="6c157-106">Permissions</span></span>
<span data-ttu-id="6c157-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="6c157-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="6c157-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="6c157-109">Azure resources</span></span>

| <span data-ttu-id="6c157-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c157-110">Permission type</span></span> | <span data-ttu-id="6c157-111">权限</span><span class="sxs-lookup"><span data-stu-id="6c157-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="6c157-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c157-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6c157-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6c157-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="6c157-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c157-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c157-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c157-115">Not supported.</span></span> |
| <span data-ttu-id="6c157-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c157-116">Application</span></span> | <span data-ttu-id="6c157-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6c157-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="6c157-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="6c157-118">Azure AD</span></span>

| <span data-ttu-id="6c157-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c157-119">Permission type</span></span> | <span data-ttu-id="6c157-120">权限</span><span class="sxs-lookup"><span data-stu-id="6c157-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="6c157-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c157-121">Delegated (work or school account)</span></span> | <span data-ttu-id="6c157-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="6c157-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="6c157-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c157-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c157-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c157-124">Not supported.</span></span> |
| <span data-ttu-id="6c157-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c157-125">Application</span></span> | <span data-ttu-id="6c157-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="6c157-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="6c157-127">组</span><span class="sxs-lookup"><span data-stu-id="6c157-127">Groups</span></span>

|<span data-ttu-id="6c157-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c157-128">Permission type</span></span> | <span data-ttu-id="6c157-129">权限</span><span class="sxs-lookup"><span data-stu-id="6c157-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="6c157-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c157-130">Delegated (work or school account)</span></span> | <span data-ttu-id="6c157-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="6c157-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="6c157-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c157-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c157-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c157-133">Not supported.</span></span> |
| <span data-ttu-id="6c157-134">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c157-134">Application</span></span> | <span data-ttu-id="6c157-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="6c157-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c157-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c157-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6c157-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6c157-137">Optional query parameters</span></span>
<span data-ttu-id="6c157-138">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6c157-138">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c157-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c157-139">Request headers</span></span>
| <span data-ttu-id="6c157-140">名称</span><span class="sxs-lookup"><span data-stu-id="6c157-140">Name</span></span>      |<span data-ttu-id="6c157-141">说明</span><span class="sxs-lookup"><span data-stu-id="6c157-141">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6c157-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c157-142">Authorization</span></span>  | <span data-ttu-id="6c157-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6c157-143">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c157-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c157-144">Request body</span></span>
<span data-ttu-id="6c157-145">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6c157-145">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6c157-146">响应</span><span class="sxs-lookup"><span data-stu-id="6c157-146">Response</span></span>
<span data-ttu-id="6c157-147">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [governanceResource](../resources/governanceresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6c157-147">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="6c157-148">示例</span><span class="sxs-lookup"><span data-stu-id="6c157-148">Examples</span></span>

<span data-ttu-id="6c157-149">此示例列出了我当前可以访问的所有资源。</span><span class="sxs-lookup"><span data-stu-id="6c157-149">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="6c157-150">请求</span><span class="sxs-lookup"><span data-stu-id="6c157-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6c157-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c157-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
# <a name="c"></a>[<span data-ttu-id="6c157-152">C#</span><span class="sxs-lookup"><span data-stu-id="6c157-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governanceresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c157-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c157-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governanceresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c157-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c157-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governanceresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c157-155">Java</span><span class="sxs-lookup"><span data-stu-id="6c157-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-governanceresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6c157-156">响应</span><span class="sxs-lookup"><span data-stu-id="6c157-156">Response</span></span>
<span data-ttu-id="6c157-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6c157-157">Here is an example of the response.</span></span> 

><span data-ttu-id="6c157-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6c157-158">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1289

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources",
    "value":[
        {
            "id": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/AnujRG/providers/Microsoft.Storage/storageAccounts/anujstoragefimdev",
            "type": "Microsoft.Storage/storageAccounts",
            "displayName": "anujstoragefimdev",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        },
        {
            "id": "0e0e4461-0c46-4d13-bf69-7cacbec75471",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/ARPJ-TESTRG-01/providers/Microsoft.Compute/virtualMachines/APRJ-VM-01-T",
            "type": "Microsoft.Compute/virtualMachines",
            "displayName": "APRJ-VM-01-T",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        },
        {
            "id": "c072eb85-e47b-4627-81cb-5af82a8fc9fb",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/ARPJ-TESTRG-01/providers/Microsoft.Compute/virtualMachines/APRJ-VM-01-T/extensions/IaaSAntimalware",
            "type": "Microsoft.Compute/virtualMachines/extensions",
            "displayName": "APRJ-VM-01-T/IaaSAntimalware",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


