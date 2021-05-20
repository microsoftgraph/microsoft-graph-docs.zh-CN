---
title: 列出 mobileAppManagementPolicies
description: 获取移动应用管理策略对象及其属性的列表。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2bf705f17ec34b3dd3738668c782a75772e0f824
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547342"
---
# <a name="list-mobileappmanagementpolicies"></a><span data-ttu-id="b1154-103">列出 mobileAppManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="b1154-103">List mobileAppManagementPolicies</span></span>

<span data-ttu-id="b1154-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1154-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1154-105">获取 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="b1154-105">Get a list of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1154-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b1154-106">Permissions</span></span>

<span data-ttu-id="b1154-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1154-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1154-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1154-109">Permission type</span></span>|<span data-ttu-id="b1154-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b1154-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1154-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1154-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b1154-112">Policy.Read.All、Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1154-112">Policy.Read.All, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="b1154-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1154-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1154-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1154-114">Not supported.</span></span>|
|<span data-ttu-id="b1154-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1154-115">Application</span></span> | <span data-ttu-id="b1154-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1154-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1154-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1154-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileAppManagementPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1154-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b1154-118">Optional query parameters</span></span>

<span data-ttu-id="b1154-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b1154-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b1154-120">例如：</span><span class="sxs-lookup"><span data-stu-id="b1154-120">For example:</span></span>

- <span data-ttu-id="b1154-121">若要选择特定属性，请添加 `$select=id,displayname` 。</span><span class="sxs-lookup"><span data-stu-id="b1154-121">To select specific attributes add `$select=id,displayname`.</span></span>
- <span data-ttu-id="b1154-122">若要检索每个策略包含的组，请添加 `$expand=includedGroups` 。</span><span class="sxs-lookup"><span data-stu-id="b1154-122">To retrieve included groups for each policy, add `$expand=includedGroups`.</span></span>
- <span data-ttu-id="b1154-123">若要根据属性进行筛选，请使用 `$filter=displayName eq 'Microsoft Intune'` 。</span><span class="sxs-lookup"><span data-stu-id="b1154-123">To filter based on an attribute, use `$filter=displayName eq 'Microsoft Intune'`.</span></span>

<span data-ttu-id="b1154-124">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b1154-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1154-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1154-125">Request headers</span></span>

|<span data-ttu-id="b1154-126">名称</span><span class="sxs-lookup"><span data-stu-id="b1154-126">Name</span></span>|<span data-ttu-id="b1154-127">说明</span><span class="sxs-lookup"><span data-stu-id="b1154-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b1154-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1154-128">Authorization</span></span>|<span data-ttu-id="b1154-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b1154-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1154-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1154-131">Request body</span></span>

<span data-ttu-id="b1154-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b1154-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1154-133">响应</span><span class="sxs-lookup"><span data-stu-id="b1154-133">Response</span></span>

<span data-ttu-id="b1154-134">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b1154-134">If successful, this method returns a `200 OK` response code and a collection of [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b1154-135">示例</span><span class="sxs-lookup"><span data-stu-id="b1154-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1154-136">请求</span><span class="sxs-lookup"><span data-stu-id="b1154-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_mobilitymanagementpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies
```

### <a name="response"></a><span data-ttu-id="b1154-137">响应</span><span class="sxs-lookup"><span data-stu-id="b1154-137">Response</span></span>

><span data-ttu-id="b1154-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b1154-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobilityManagementPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
   {
    "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
    "id": "ab90bacf-55a3-4a3e-839a-aa4b74e4f020",
    "appliesTo": "selected",
    "complianceUrl": "https://portal.manage.contoso.com/?portalAction=Compliance",
    "description": "Contoso mobilty app is a cloud-based  Endpoint Management solution for managing Windows.",
    "discoveryUrl": "https://enrollment.manage.contoso.com/enrollmentserver/discovery.svc",
    "displayName": "Contoso mobilty app",
    "termsOfUseUrl": "https://portal.manage.contoso.com/TermsofUse.aspx",
    "includedGroups": [
      {
        "id": "800c583d-cc3d-4361-8e4a-3fbf668f27f4",
        "displayName": "Test Group"
      }
    ]
  }
  ]
}
```

<!-- uuid: 5c98f801-d1c4-44eb-ac11-f72b6754deda
2020-03-23T22:34:45.203Z -->
<!-- {
  "type": "#page.annotation",
  "description": "List mobileAppManagementPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
