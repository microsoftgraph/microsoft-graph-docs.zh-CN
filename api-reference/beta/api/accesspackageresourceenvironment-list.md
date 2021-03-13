---
title: 列出 accessPackageResourceEnvironments
description: 检索 accessPackageResourceEnvironment 对象的列表。
author: hanki-microsoft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 823abc8a71cfce4ac7872f4e6e86ae7d08e92411
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759409"
---
# <a name="list-accesspackageresourceenvironments"></a><span data-ttu-id="3cda5-103">列出 accessPackageResourceEnvironments</span><span class="sxs-lookup"><span data-stu-id="3cda5-103">List accessPackageResourceEnvironments</span></span>
<span data-ttu-id="3cda5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cda5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cda5-105">检索 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="3cda5-105">Retrieve a list of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cda5-106">权限</span><span class="sxs-lookup"><span data-stu-id="3cda5-106">Permissions</span></span>
<span data-ttu-id="3cda5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cda5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cda5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cda5-109">Permission type</span></span>|<span data-ttu-id="3cda5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cda5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cda5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cda5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3cda5-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cda5-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="3cda5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cda5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cda5-114">不支持</span><span class="sxs-lookup"><span data-stu-id="3cda5-114">Not supported</span></span>|
|<span data-ttu-id="3cda5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cda5-115">Application</span></span>|<span data-ttu-id="3cda5-116">不支持</span><span class="sxs-lookup"><span data-stu-id="3cda5-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cda5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cda5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3cda5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3cda5-118">Optional query parameters</span></span>
<span data-ttu-id="3cda5-119">此方法需要 `$filter` [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="3cda5-119">This method requires the `$filter` [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="3cda5-120">你必须申请 `$filter` **originSystem** 设置为 (`eq`) `SharePointOnline` 。</span><span class="sxs-lookup"><span data-stu-id="3cda5-120">You must apply `$filter` for an **originSystem** set to (`eq`) `SharePointOnline`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cda5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cda5-121">Request headers</span></span>
|<span data-ttu-id="3cda5-122">名称</span><span class="sxs-lookup"><span data-stu-id="3cda5-122">Name</span></span>|<span data-ttu-id="3cda5-123">说明</span><span class="sxs-lookup"><span data-stu-id="3cda5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3cda5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cda5-124">Authorization</span></span>|<span data-ttu-id="3cda5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3cda5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cda5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cda5-127">Request body</span></span>
<span data-ttu-id="3cda5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3cda5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cda5-129">响应</span><span class="sxs-lookup"><span data-stu-id="3cda5-129">Response</span></span>

<span data-ttu-id="3cda5-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3cda5-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3cda5-131">示例</span><span class="sxs-lookup"><span data-stu-id="3cda5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3cda5-132">请求</span><span class="sxs-lookup"><span data-stu-id="3cda5-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3cda5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cda5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```
# <a name="c"></a>[<span data-ttu-id="3cda5-134">C#</span><span class="sxs-lookup"><span data-stu-id="3cda5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cda5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cda5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cda5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cda5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cda5-137">Java</span><span class="sxs-lookup"><span data-stu-id="3cda5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3cda5-138">响应</span><span class="sxs-lookup"><span data-stu-id="3cda5-138">Response</span></span>
<span data-ttu-id="3cda5-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3cda5-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageResourceEnvironment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceEnvironments",
  "value": [
    {
      "id": "615f2218-678f-471f-a60a-02c2f4f80c57",
      "displayName": "https://contoso.sharepoint.com/",
      "description": "https://contoso.sharepoint.com/",
      "originSystem": "SharePointOnline",
      "originId": "https://contoso-admin.sharepoint.com/",
      "isDefaultEnvironment": false,
      "connectionInfo": {
        "url": "https://contoso-admin.sharepoint.com/"
      }
    }
  ]
}
```

