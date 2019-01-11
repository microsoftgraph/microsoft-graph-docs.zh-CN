---
title: 列表 governanceResources
description: 检索请求者有权访问的 governanceResource 的集合。
localization_priority: Normal
ms.openlocfilehash: 4527c7a5f59832fe69181a815af40a0e0e073c90
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838295"
---
# <a name="list-governanceresources"></a><span data-ttu-id="e3270-103">列表 governanceResources</span><span class="sxs-lookup"><span data-stu-id="e3270-103">List governanceResources</span></span>

> <span data-ttu-id="e3270-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e3270-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3270-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e3270-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3270-106">检索[governanceResource](../resources/governanceresource.md)的请求者有权访问的集合。</span><span class="sxs-lookup"><span data-stu-id="e3270-106">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3270-107">权限</span><span class="sxs-lookup"><span data-stu-id="e3270-107">Permissions</span></span>
<span data-ttu-id="e3270-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3270-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3270-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3270-110">Permission type</span></span>      | <span data-ttu-id="e3270-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="e3270-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3270-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3270-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e3270-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e3270-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="e3270-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3270-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3270-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3270-115">Not supported.</span></span>    |
|<span data-ttu-id="e3270-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3270-116">Application</span></span> | <span data-ttu-id="e3270-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e3270-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3270-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3270-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e3270-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e3270-119">Optional query parameters</span></span>
<span data-ttu-id="e3270-120">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="e3270-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3270-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3270-121">Request headers</span></span>
| <span data-ttu-id="e3270-122">名称</span><span class="sxs-lookup"><span data-stu-id="e3270-122">Name</span></span>      |<span data-ttu-id="e3270-123">说明</span><span class="sxs-lookup"><span data-stu-id="e3270-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e3270-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3270-124">Authorization</span></span>  | <span data-ttu-id="e3270-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e3270-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3270-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3270-126">Request body</span></span>
<span data-ttu-id="e3270-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e3270-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e3270-128">响应</span><span class="sxs-lookup"><span data-stu-id="e3270-128">Response</span></span>
<span data-ttu-id="e3270-129">如果成功，此方法返回`200 OK`响应代码和响应正文中的[governanceResource](../resources/governanceresource.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="e3270-129">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="e3270-130">示例</span><span class="sxs-lookup"><span data-stu-id="e3270-130">Examples</span></span>

<span data-ttu-id="e3270-131">此示例将列出当前可以访问的所有资源。</span><span class="sxs-lookup"><span data-stu-id="e3270-131">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="e3270-132">请求</span><span class="sxs-lookup"><span data-stu-id="e3270-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
##### <a name="response"></a><span data-ttu-id="e3270-133">响应</span><span class="sxs-lookup"><span data-stu-id="e3270-133">Response</span></span>
<span data-ttu-id="e3270-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e3270-134">Here is an example of the response.</span></span> 

><span data-ttu-id="e3270-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e3270-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List governanceResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
