---
title: 列出 governanceResources
description: 检索请求者有权访问的 governanceResource 的集合。
localization_priority: Normal
ms.openlocfilehash: e68e4633735d1eecb5d4994e3c2c70bf06a70e6a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593533"
---
# <a name="list-governanceresources"></a><span data-ttu-id="46be0-103">列出 governanceResources</span><span class="sxs-lookup"><span data-stu-id="46be0-103">List governanceResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46be0-104">检索请求者有权访问的[governanceResource](../resources/governanceresource.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="46be0-104">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="46be0-105">权限</span><span class="sxs-lookup"><span data-stu-id="46be0-105">Permissions</span></span>
<span data-ttu-id="46be0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46be0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46be0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="46be0-108">Permission type</span></span>      | <span data-ttu-id="46be0-109">权限</span><span class="sxs-lookup"><span data-stu-id="46be0-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46be0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46be0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="46be0-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="46be0-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="46be0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46be0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46be0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="46be0-113">Not supported.</span></span>    |
|<span data-ttu-id="46be0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="46be0-114">Application</span></span> | <span data-ttu-id="46be0-115">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="46be0-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="46be0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46be0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="46be0-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="46be0-117">Optional query parameters</span></span>
<span data-ttu-id="46be0-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="46be0-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46be0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="46be0-119">Request headers</span></span>
| <span data-ttu-id="46be0-120">名称</span><span class="sxs-lookup"><span data-stu-id="46be0-120">Name</span></span>      |<span data-ttu-id="46be0-121">说明</span><span class="sxs-lookup"><span data-stu-id="46be0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46be0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="46be0-122">Authorization</span></span>  | <span data-ttu-id="46be0-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="46be0-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="46be0-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="46be0-124">Request body</span></span>
<span data-ttu-id="46be0-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="46be0-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="46be0-126">响应</span><span class="sxs-lookup"><span data-stu-id="46be0-126">Response</span></span>
<span data-ttu-id="46be0-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[governanceResource](../resources/governanceresource.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="46be0-127">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="46be0-128">示例</span><span class="sxs-lookup"><span data-stu-id="46be0-128">Examples</span></span>

<span data-ttu-id="46be0-129">本示例列出了我当前可以访问的所有资源。</span><span class="sxs-lookup"><span data-stu-id="46be0-129">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="46be0-130">请求</span><span class="sxs-lookup"><span data-stu-id="46be0-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
##### <a name="response"></a><span data-ttu-id="46be0-131">响应</span><span class="sxs-lookup"><span data-stu-id="46be0-131">Response</span></span>
<span data-ttu-id="46be0-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="46be0-132">Here is an example of the response.</span></span> 

><span data-ttu-id="46be0-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="46be0-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="46be0-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="46be0-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="46be0-136">语言</span><span class="sxs-lookup"><span data-stu-id="46be0-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_governanceresources-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46be0-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="46be0-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_governanceresources-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/governanceresource-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceresource-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
