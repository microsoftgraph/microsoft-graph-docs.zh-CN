---
title: 获取 accessPackageResourceEnvironment
description: 读取 accessPackageResourceEnvironment 对象的属性和关系。
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0169ad18a24ff27392c5679f91dfaecd43d76567
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176285"
---
# <a name="get-accesspackageresourceenvironment"></a><span data-ttu-id="42808-103">获取 accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="42808-103">Get accessPackageResourceEnvironment</span></span>
<span data-ttu-id="42808-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42808-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42808-105">读取 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="42808-105">Read the properties and relationships of an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="42808-106">权限</span><span class="sxs-lookup"><span data-stu-id="42808-106">Permissions</span></span>
<span data-ttu-id="42808-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42808-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="42808-109">Permission type</span></span>|<span data-ttu-id="42808-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42808-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42808-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42808-111">Delegated (work or school account)</span></span>|<span data-ttu-id="42808-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42808-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="42808-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42808-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42808-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="42808-114">Not supported.</span></span>|
|<span data-ttu-id="42808-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="42808-115">Application</span></span>|<span data-ttu-id="42808-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="42808-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42808-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42808-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42808-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="42808-118">Optional query parameters</span></span>
<span data-ttu-id="42808-119">此方法当前不支持 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="42808-119">This method does not currently support [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="42808-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="42808-120">Request headers</span></span>
|<span data-ttu-id="42808-121">名称</span><span class="sxs-lookup"><span data-stu-id="42808-121">Name</span></span>|<span data-ttu-id="42808-122">说明</span><span class="sxs-lookup"><span data-stu-id="42808-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="42808-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42808-123">Authorization</span></span>|<span data-ttu-id="42808-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="42808-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42808-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="42808-126">Request body</span></span>
<span data-ttu-id="42808-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="42808-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42808-128">响应</span><span class="sxs-lookup"><span data-stu-id="42808-128">Response</span></span>

<span data-ttu-id="42808-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="42808-129">If successful, this method returns a `200 OK` response code and an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42808-130">示例</span><span class="sxs-lookup"><span data-stu-id="42808-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42808-131">请求</span><span class="sxs-lookup"><span data-stu-id="42808-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="42808-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="42808-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}
```
# <a name="c"></a>[<span data-ttu-id="42808-133">C#</span><span class="sxs-lookup"><span data-stu-id="42808-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42808-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42808-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42808-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42808-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42808-136">Java</span><span class="sxs-lookup"><span data-stu-id="42808-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="42808-137">响应</span><span class="sxs-lookup"><span data-stu-id="42808-137">Response</span></span>
<span data-ttu-id="42808-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="42808-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceEnvironment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceEnvironments/$entity",
    "id": "615f2218-678f-471f-a60a-02c2f4f80c57",
    "displayName": "https://contoso.sharepoint.com/",
    "description": "GeoLocation: , RootSiteUrl: https://contoso.sharepoint.com/, TenantAdminUrl: https://contoso-admin.sharepoint.com/",
    "originSystem": "SharePointOnline",
    "originId": "https://contoso-admin.sharepoint.com/",
    "isDefaultEnvironment": false,
    "connectionInfo": {
        "url": "https://contoso-admin.sharepoint.com/"
    }
}
```

