---
title: 列出 governanceResources
description: 检索请求者有权访问的 governanceResource 的集合。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: 98c19e86b80a95d23e12508740f082370997f147
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639868"
---
# <a name="list-governanceresources"></a><span data-ttu-id="ef4b4-103">列出 governanceResources</span><span class="sxs-lookup"><span data-stu-id="ef4b4-103">List governanceResources</span></span>

<span data-ttu-id="ef4b4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef4b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef4b4-105">检索请求者有权访问的[governanceResource](../resources/governanceresource.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="ef4b4-105">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef4b4-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ef4b4-106">Permissions</span></span>
<span data-ttu-id="ef4b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef4b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef4b4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef4b4-109">Permission type</span></span>      | <span data-ttu-id="ef4b4-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="ef4b4-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef4b4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef4b4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ef4b4-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="ef4b4-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="ef4b4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef4b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef4b4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef4b4-114">Not supported.</span></span>    |
|<span data-ttu-id="ef4b4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef4b4-115">Application</span></span> | <span data-ttu-id="ef4b4-116">PrivilegedAccess。 AzureResources</span><span class="sxs-lookup"><span data-stu-id="ef4b4-116">PrivilegedAccess.Read.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef4b4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef4b4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ef4b4-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ef4b4-118">Optional query parameters</span></span>
<span data-ttu-id="ef4b4-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ef4b4-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef4b4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef4b4-120">Request headers</span></span>
| <span data-ttu-id="ef4b4-121">名称</span><span class="sxs-lookup"><span data-stu-id="ef4b4-121">Name</span></span>      |<span data-ttu-id="ef4b4-122">说明</span><span class="sxs-lookup"><span data-stu-id="ef4b4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ef4b4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef4b4-123">Authorization</span></span>  | <span data-ttu-id="ef4b4-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ef4b4-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef4b4-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef4b4-125">Request body</span></span>
<span data-ttu-id="ef4b4-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ef4b4-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ef4b4-127">响应</span><span class="sxs-lookup"><span data-stu-id="ef4b4-127">Response</span></span>
<span data-ttu-id="ef4b4-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[governanceResource](../resources/governanceresource.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ef4b4-128">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="ef4b4-129">示例</span><span class="sxs-lookup"><span data-stu-id="ef4b4-129">Examples</span></span>

<span data-ttu-id="ef4b4-130">本示例列出了我当前可以访问的所有资源。</span><span class="sxs-lookup"><span data-stu-id="ef4b4-130">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="ef4b4-131">请求</span><span class="sxs-lookup"><span data-stu-id="ef4b4-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ef4b4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef4b4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
# <a name="c"></a>[<span data-ttu-id="ef4b4-133">C#</span><span class="sxs-lookup"><span data-stu-id="ef4b4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governanceresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef4b4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef4b4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governanceresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef4b4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef4b4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governanceresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ef4b4-136">响应</span><span class="sxs-lookup"><span data-stu-id="ef4b4-136">Response</span></span>
<span data-ttu-id="ef4b4-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ef4b4-137">Here is an example of the response.</span></span> 

><span data-ttu-id="ef4b4-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ef4b4-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
