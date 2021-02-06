---
title: 列出 accessPackageResourceEnvironments
description: 检索 accessPackageResourceEnvironment 对象的列表。
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cf7116ef1512dca40cae66d92030b032d3aefa23
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137695"
---
# <a name="list-accesspackageresourceenvironments"></a><span data-ttu-id="08329-103">列出 accessPackageResourceEnvironments</span><span class="sxs-lookup"><span data-stu-id="08329-103">List accessPackageResourceEnvironments</span></span>
<span data-ttu-id="08329-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08329-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08329-105">检索 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="08329-105">Retrieve a list of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="08329-106">权限</span><span class="sxs-lookup"><span data-stu-id="08329-106">Permissions</span></span>
<span data-ttu-id="08329-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08329-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08329-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="08329-109">Permission type</span></span>|<span data-ttu-id="08329-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08329-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08329-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08329-111">Delegated (work or school account)</span></span>|<span data-ttu-id="08329-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08329-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="08329-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08329-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08329-114">不支持</span><span class="sxs-lookup"><span data-stu-id="08329-114">Not supported</span></span>|
|<span data-ttu-id="08329-115">Application</span><span class="sxs-lookup"><span data-stu-id="08329-115">Application</span></span>|<span data-ttu-id="08329-116">不支持</span><span class="sxs-lookup"><span data-stu-id="08329-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="08329-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08329-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08329-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="08329-118">Optional query parameters</span></span>
<span data-ttu-id="08329-119">此方法需要 `$filter` [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="08329-119">This method requires the `$filter` [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="08329-120">你必须申请 `$filter` **originSystem** 设置为 `eq` `SharePointOnline` () 。</span><span class="sxs-lookup"><span data-stu-id="08329-120">You must apply `$filter` for an **originSystem** set to (`eq`) `SharePointOnline`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08329-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="08329-121">Request headers</span></span>
|<span data-ttu-id="08329-122">名称</span><span class="sxs-lookup"><span data-stu-id="08329-122">Name</span></span>|<span data-ttu-id="08329-123">说明</span><span class="sxs-lookup"><span data-stu-id="08329-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="08329-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="08329-124">Authorization</span></span>|<span data-ttu-id="08329-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="08329-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="08329-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="08329-127">Request body</span></span>
<span data-ttu-id="08329-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="08329-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08329-129">响应</span><span class="sxs-lookup"><span data-stu-id="08329-129">Response</span></span>

<span data-ttu-id="08329-130">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="08329-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="08329-131">示例</span><span class="sxs-lookup"><span data-stu-id="08329-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="08329-132">请求</span><span class="sxs-lookup"><span data-stu-id="08329-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```


### <a name="response"></a><span data-ttu-id="08329-133">响应</span><span class="sxs-lookup"><span data-stu-id="08329-133">Response</span></span>
<span data-ttu-id="08329-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="08329-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

