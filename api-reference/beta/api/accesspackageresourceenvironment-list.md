---
title: 列出 accessPackageResourceEnvironments
description: 检索 accessPackageResourceEnvironment 对象的列表。
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2843300c166cf064c3cd79c79551ae6c7b764ecf
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176236"
---
# <a name="list-accesspackageresourceenvironments"></a><span data-ttu-id="d56bd-103">列出 accessPackageResourceEnvironments</span><span class="sxs-lookup"><span data-stu-id="d56bd-103">List accessPackageResourceEnvironments</span></span>
<span data-ttu-id="d56bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d56bd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d56bd-105">检索 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="d56bd-105">Retrieve a list of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="d56bd-106">权限</span><span class="sxs-lookup"><span data-stu-id="d56bd-106">Permissions</span></span>
<span data-ttu-id="d56bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d56bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d56bd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d56bd-109">Permission type</span></span>|<span data-ttu-id="d56bd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d56bd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d56bd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d56bd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d56bd-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d56bd-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="d56bd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d56bd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d56bd-114">不支持</span><span class="sxs-lookup"><span data-stu-id="d56bd-114">Not supported</span></span>|
|<span data-ttu-id="d56bd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d56bd-115">Application</span></span>|<span data-ttu-id="d56bd-116">不支持</span><span class="sxs-lookup"><span data-stu-id="d56bd-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="d56bd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d56bd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d56bd-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d56bd-118">Optional query parameters</span></span>
<span data-ttu-id="d56bd-119">此方法需要 `$filter` [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d56bd-119">This method requires the `$filter` [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="d56bd-120">你必须申请 `$filter` **originSystem** 设置为 `eq` `SharePointOnline` () 。</span><span class="sxs-lookup"><span data-stu-id="d56bd-120">You must apply `$filter` for an **originSystem** set to (`eq`) `SharePointOnline`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d56bd-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d56bd-121">Request headers</span></span>
|<span data-ttu-id="d56bd-122">名称</span><span class="sxs-lookup"><span data-stu-id="d56bd-122">Name</span></span>|<span data-ttu-id="d56bd-123">说明</span><span class="sxs-lookup"><span data-stu-id="d56bd-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d56bd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d56bd-124">Authorization</span></span>|<span data-ttu-id="d56bd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d56bd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d56bd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d56bd-127">Request body</span></span>
<span data-ttu-id="d56bd-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d56bd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d56bd-129">响应</span><span class="sxs-lookup"><span data-stu-id="d56bd-129">Response</span></span>

<span data-ttu-id="d56bd-130">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d56bd-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d56bd-131">示例</span><span class="sxs-lookup"><span data-stu-id="d56bd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d56bd-132">请求</span><span class="sxs-lookup"><span data-stu-id="d56bd-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d56bd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d56bd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```
# <a name="c"></a>[<span data-ttu-id="d56bd-134">C#</span><span class="sxs-lookup"><span data-stu-id="d56bd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d56bd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d56bd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d56bd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d56bd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d56bd-137">Java</span><span class="sxs-lookup"><span data-stu-id="d56bd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d56bd-138">响应</span><span class="sxs-lookup"><span data-stu-id="d56bd-138">Response</span></span>
<span data-ttu-id="d56bd-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d56bd-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

