---
title: 获取 tenantDetailedInformation
description: 读取 tenantDetailedInformation 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: a9e771d5391989dd884d77240091ffba4f523353
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441805"
---
# <a name="get-tenantdetailedinformation"></a><span data-ttu-id="0e3b5-103">获取 tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="0e3b5-103">Get tenantDetailedInformation</span></span>
<span data-ttu-id="0e3b5-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="0e3b5-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e3b5-105">读取 [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-105">Read the properties and relationships of a [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e3b5-106">权限</span><span class="sxs-lookup"><span data-stu-id="0e3b5-106">Permissions</span></span>
<span data-ttu-id="0e3b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e3b5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e3b5-109">Permission type</span></span>|<span data-ttu-id="0e3b5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e3b5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e3b5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e3b5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e3b5-112">ManagedTenants.Read.All、ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e3b5-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="0e3b5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e3b5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e3b5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-114">Not supported.</span></span>|
|<span data-ttu-id="0e3b5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e3b5-115">Application</span></span>|<span data-ttu-id="0e3b5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e3b5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e3b5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantsDetailedInformation/{tenantDetailedInformationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e3b5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0e3b5-118">Optional query parameters</span></span>
<span data-ttu-id="0e3b5-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e3b5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e3b5-120">Request headers</span></span>
|<span data-ttu-id="0e3b5-121">名称</span><span class="sxs-lookup"><span data-stu-id="0e3b5-121">Name</span></span>|<span data-ttu-id="0e3b5-122">说明</span><span class="sxs-lookup"><span data-stu-id="0e3b5-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0e3b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e3b5-123">Authorization</span></span>|<span data-ttu-id="0e3b5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e3b5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e3b5-126">Request body</span></span>
<span data-ttu-id="0e3b5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e3b5-128">响应</span><span class="sxs-lookup"><span data-stu-id="0e3b5-128">Response</span></span>

<span data-ttu-id="0e3b5-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-129">If successful, this method returns a `200 OK` response code and a [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e3b5-130">示例</span><span class="sxs-lookup"><span data-stu-id="0e3b5-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e3b5-131">请求</span><span class="sxs-lookup"><span data-stu-id="0e3b5-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0e3b5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e3b5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tenantdetailedinformation"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantsDetailedInformation/{tenantDetailedInformationId}
```
# <a name="c"></a>[<span data-ttu-id="0e3b5-133">C#</span><span class="sxs-lookup"><span data-stu-id="0e3b5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tenantdetailedinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e3b5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e3b5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tenantdetailedinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e3b5-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e3b5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tenantdetailedinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e3b5-136">Java</span><span class="sxs-lookup"><span data-stu-id="0e3b5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tenantdetailedinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0e3b5-137">响应</span><span class="sxs-lookup"><span data-stu-id="0e3b5-137">Response</span></span>
><span data-ttu-id="0e3b5-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantDetailedInformation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantDetailedInformation",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "companyName": "Fourth Coffee",
  "defaultDomainName": "fourthcoffee001.onmicrosoft.com",
  "countryName": "United States",
  "countryCode": "US",
  "city": "Redmond",
  "region": "NA",
  "verticalName": "Software",
  "industryName": "Computer",
  "segmentName": "Service"
}
```
