---
title: 列出 tenantTags
description: 获取 tenantTag 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: a277228444b527082360eb1fc9e3ad886dbe7b55
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402325"
---
# <a name="list-tenanttags"></a><span data-ttu-id="66591-103">列出 tenantTags</span><span class="sxs-lookup"><span data-stu-id="66591-103">List tenantTags</span></span>
<span data-ttu-id="66591-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="66591-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66591-105">获取 [tenantTag 对象](../resources/managedtenants-tenanttag.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="66591-105">Get a list of the [tenantTag](../resources/managedtenants-tenanttag.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="66591-106">权限</span><span class="sxs-lookup"><span data-stu-id="66591-106">Permissions</span></span>
<span data-ttu-id="66591-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66591-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66591-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="66591-109">Permission type</span></span>|<span data-ttu-id="66591-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66591-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66591-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66591-111">Delegated (work or school account)</span></span>|<span data-ttu-id="66591-112">ManagedTenants.Read.All、ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="66591-112">ManagedTenants.Read.All, ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="66591-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66591-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66591-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="66591-114">Not supported.</span></span>|
|<span data-ttu-id="66591-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="66591-115">Application</span></span>|<span data-ttu-id="66591-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="66591-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66591-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66591-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantTags
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66591-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="66591-118">Optional query parameters</span></span>
<span data-ttu-id="66591-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="66591-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66591-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="66591-120">Request headers</span></span>
|<span data-ttu-id="66591-121">名称</span><span class="sxs-lookup"><span data-stu-id="66591-121">Name</span></span>|<span data-ttu-id="66591-122">说明</span><span class="sxs-lookup"><span data-stu-id="66591-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="66591-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66591-123">Authorization</span></span>|<span data-ttu-id="66591-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66591-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="66591-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="66591-126">Request body</span></span>
<span data-ttu-id="66591-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66591-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66591-128">响应</span><span class="sxs-lookup"><span data-stu-id="66591-128">Response</span></span>

<span data-ttu-id="66591-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [tenantTag](../resources/managedtenants-tenanttag.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="66591-129">If successful, this method returns a `200 OK` response code and a collection of [tenantTag](../resources/managedtenants-tenanttag.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66591-130">示例</span><span class="sxs-lookup"><span data-stu-id="66591-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="66591-131">请求</span><span class="sxs-lookup"><span data-stu-id="66591-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_tenanttag"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags
```


### <a name="response"></a><span data-ttu-id="66591-132">响应</span><span class="sxs-lookup"><span data-stu-id="66591-132">Response</span></span>
><span data-ttu-id="66591-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="66591-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenantTag)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantTags",
    "value": [
        {
            "id": "913391c0-5466-42b4-900d-0a7501399cb0",
            "displayName": "Onboarding",
            "description": "Tenants that we are currently onboarding",
            "properties": null,
            "tenantIds": [
                "38227791-a88b-4fcc-81c5-58cf77668320",
                "34298981-4fc8-4974-9486-c8909ed1521b",
                "4d262a25-c70a-430b-9e8e-46c31dec116b"
            ],
            "isDeleted": null,
            "createdDateTime": "2021-06-16T20:36:31.086644Z",
            "createdByUserId": "9bf6a5ad-aecb-4194-a16b-38e02702a602",
            "lastActionDateTime": "2021-06-28T20:46:09.0071888Z",
            "lastActionByUserId": "08ea0285-30cb-46cc-abc8-3d8422e21ecb",
            "tenants": [
                {
                    "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
                },
                {
                    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b"
                },
                {
                    "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b"
                }
            ]
        },
        {
            "id": "bfd883e8-10f3-40ee-994c-111fa1c5d1db",
            "displayName": "ExtendedSupport",
            "description": "Tenants that have purchased extended support.",
            "properties": null,
            "tenantIds": [
                "38227791-a88b-4fcc-81c5-58cf77668320",
                "4d262a25-c70a-430b-9e8e-46c31dec116b"
            ],
            "isDeleted": null,
            "createdDateTime": "2021-06-16T20:43:31.8917383Z",
            "createdByUserId": "43a2424c-0fa3-446d-bee9-4ab500bb1603",
            "lastActionDateTime": "2021-06-17T03:23:31.3531635Z",
            "lastActionByUserId": "248f617e-a6a7-4d31-922d-726c24074bb6",
            "tenants": [
                {
                    "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
                },
                {
                    "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b"
                }
            ]
        }
    ]
}
```
