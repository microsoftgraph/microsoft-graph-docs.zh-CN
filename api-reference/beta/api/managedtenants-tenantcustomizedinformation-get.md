---
title: 获取 tenantCustomizedInformation
description: 读取 tenantCustomizedInformation 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 2a91d3640c542de3ee0dea96c408f2fdf5c18fdc
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402244"
---
# <a name="get-tenantcustomizedinformation"></a><span data-ttu-id="c36f7-103">获取 tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="c36f7-103">Get tenantCustomizedInformation</span></span>
<span data-ttu-id="c36f7-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="c36f7-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c36f7-105">读取 [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c36f7-105">Read the properties and relationships of a [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c36f7-106">权限</span><span class="sxs-lookup"><span data-stu-id="c36f7-106">Permissions</span></span>
<span data-ttu-id="c36f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c36f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c36f7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c36f7-109">Permission type</span></span>|<span data-ttu-id="c36f7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c36f7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c36f7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c36f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c36f7-112">ManagedTenants.Read.All、ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c36f7-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="c36f7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c36f7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c36f7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c36f7-114">Not supported.</span></span>|
|<span data-ttu-id="c36f7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c36f7-115">Application</span></span>|<span data-ttu-id="c36f7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c36f7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c36f7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c36f7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c36f7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c36f7-118">Optional query parameters</span></span>
<span data-ttu-id="c36f7-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="c36f7-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c36f7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c36f7-120">Request headers</span></span>
|<span data-ttu-id="c36f7-121">名称</span><span class="sxs-lookup"><span data-stu-id="c36f7-121">Name</span></span>|<span data-ttu-id="c36f7-122">说明</span><span class="sxs-lookup"><span data-stu-id="c36f7-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c36f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c36f7-123">Authorization</span></span>|<span data-ttu-id="c36f7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c36f7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c36f7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c36f7-126">Request body</span></span>
<span data-ttu-id="c36f7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c36f7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c36f7-128">响应</span><span class="sxs-lookup"><span data-stu-id="c36f7-128">Response</span></span>

<span data-ttu-id="c36f7-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c36f7-129">If successful, this method returns a `200 OK` response code and a [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c36f7-130">示例</span><span class="sxs-lookup"><span data-stu-id="c36f7-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c36f7-131">请求</span><span class="sxs-lookup"><span data-stu-id="c36f7-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tenantcustomizedinformation"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}
```


### <a name="response"></a><span data-ttu-id="c36f7-132">响应</span><span class="sxs-lookup"><span data-stu-id="c36f7-132">Response</span></span>
><span data-ttu-id="c36f7-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c36f7-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantCustomizedInformation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "website": "https://www.fourthcoffee.com",
  "contacts": [
    {
      "name": "Sally",
      "email": "sally@fourthcoffee.com",
      "phone": "5558009731"
    },
    {
      "name": "Hector",
      "email": "hector@fourthcoffee.com",
      "phone": "5558009732"
    }
  ]
}
```
