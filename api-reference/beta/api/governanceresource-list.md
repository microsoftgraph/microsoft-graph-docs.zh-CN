---
title: 列表 governanceResources
description: 检索请求者有权访问的 governanceResource 的集合。
ms.openlocfilehash: 0c50fa03cc8294650fa592e3ff7a1692d89cfbb9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044574"
---
# <a name="list-governanceresources"></a><span data-ttu-id="223f7-103">列表 governanceResources</span><span class="sxs-lookup"><span data-stu-id="223f7-103">List governanceResources</span></span>

> <span data-ttu-id="223f7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="223f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="223f7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="223f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="223f7-106">检索[governanceResource](../resources/governanceresource.md)的请求者有权访问的集合。</span><span class="sxs-lookup"><span data-stu-id="223f7-106">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="223f7-107">权限</span><span class="sxs-lookup"><span data-stu-id="223f7-107">Permissions</span></span>
<span data-ttu-id="223f7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="223f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="223f7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="223f7-110">Permission type</span></span>      | <span data-ttu-id="223f7-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="223f7-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="223f7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="223f7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="223f7-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="223f7-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="223f7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="223f7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="223f7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="223f7-115">Not supported.</span></span>    |
|<span data-ttu-id="223f7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="223f7-116">Application</span></span> | <span data-ttu-id="223f7-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="223f7-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="223f7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="223f7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="223f7-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="223f7-119">Optional query parameters</span></span>
<span data-ttu-id="223f7-120">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="223f7-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="223f7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="223f7-121">Request headers</span></span>
| <span data-ttu-id="223f7-122">名称</span><span class="sxs-lookup"><span data-stu-id="223f7-122">Name</span></span>      |<span data-ttu-id="223f7-123">说明</span><span class="sxs-lookup"><span data-stu-id="223f7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="223f7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="223f7-124">Authorization</span></span>  | <span data-ttu-id="223f7-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="223f7-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="223f7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="223f7-126">Request body</span></span>
<span data-ttu-id="223f7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="223f7-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="223f7-128">响应</span><span class="sxs-lookup"><span data-stu-id="223f7-128">Response</span></span>
<span data-ttu-id="223f7-129">如果成功，此方法返回`200 OK`响应代码和响应正文中的[governanceResource](../resources/governanceresource.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="223f7-129">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="223f7-130">示例</span><span class="sxs-lookup"><span data-stu-id="223f7-130">Examples</span></span>

<span data-ttu-id="223f7-131">此示例将列出当前可以访问的所有资源。</span><span class="sxs-lookup"><span data-stu-id="223f7-131">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="223f7-132">请求</span><span class="sxs-lookup"><span data-stu-id="223f7-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
##### <a name="response"></a><span data-ttu-id="223f7-133">响应</span><span class="sxs-lookup"><span data-stu-id="223f7-133">Response</span></span>
<span data-ttu-id="223f7-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="223f7-134">Here is an example of the response.</span></span> 

><span data-ttu-id="223f7-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="223f7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "onboardDateTime": null
        },
        {
            "id": "0e0e4461-0c46-4d13-bf69-7cacbec75471",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/ARPJ-TESTRG-01/providers/Microsoft.Compute/virtualMachines/APRJ-VM-01-T",
            "type": "Microsoft.Compute/virtualMachines",
            "displayName": "APRJ-VM-01-T",
            "status": "Active",
            "onboardDateTime": null
        },
        {
            "id": "c072eb85-e47b-4627-81cb-5af82a8fc9fb",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/ARPJ-TESTRG-01/providers/Microsoft.Compute/virtualMachines/APRJ-VM-01-T/extensions/IaaSAntimalware",
            "type": "Microsoft.Compute/virtualMachines/extensions",
            "displayName": "APRJ-VM-01-T/IaaSAntimalware",
            "status": "Active",
            "onboardDateTime": null
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
