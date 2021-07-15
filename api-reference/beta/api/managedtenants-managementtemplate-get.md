---
title: 获取 managementTemplate
description: 读取 managementTemplate 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: c30201c322a1e71f893320e6dc2625334b35b0b7
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441422"
---
# <a name="get-managementtemplate"></a><span data-ttu-id="6f163-103">获取 managementTemplate</span><span class="sxs-lookup"><span data-stu-id="6f163-103">Get managementTemplate</span></span>
<span data-ttu-id="6f163-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="6f163-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f163-105">读取 [managementTemplate](../resources/managedtenants-managementtemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6f163-105">Read the properties and relationships of a [managementTemplate](../resources/managedtenants-managementtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f163-106">权限</span><span class="sxs-lookup"><span data-stu-id="6f163-106">Permissions</span></span>
<span data-ttu-id="6f163-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f163-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f163-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f163-109">Permission type</span></span>|<span data-ttu-id="6f163-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f163-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f163-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f163-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6f163-112">ManagedTenants.Read.All、ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f163-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="6f163-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f163-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f163-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f163-114">Not supported.</span></span>|
|<span data-ttu-id="6f163-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f163-115">Application</span></span>|<span data-ttu-id="6f163-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f163-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f163-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f163-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementTemplates/{managementTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f163-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6f163-118">Optional query parameters</span></span>
<span data-ttu-id="6f163-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="6f163-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f163-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f163-120">Request headers</span></span>
|<span data-ttu-id="6f163-121">名称</span><span class="sxs-lookup"><span data-stu-id="6f163-121">Name</span></span>|<span data-ttu-id="6f163-122">说明</span><span class="sxs-lookup"><span data-stu-id="6f163-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6f163-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f163-123">Authorization</span></span>|<span data-ttu-id="6f163-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6f163-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f163-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f163-126">Request body</span></span>
<span data-ttu-id="6f163-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6f163-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f163-128">响应</span><span class="sxs-lookup"><span data-stu-id="6f163-128">Response</span></span>

<span data-ttu-id="6f163-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [managementTemplate](../resources/managedtenants-managementtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6f163-129">If successful, this method returns a `200 OK` response code and a [managementTemplate](../resources/managedtenants-managementtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f163-130">示例</span><span class="sxs-lookup"><span data-stu-id="6f163-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6f163-131">请求</span><span class="sxs-lookup"><span data-stu-id="6f163-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6f163-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f163-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_managementtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementTemplates/{managementTemplateId}
```
# <a name="c"></a>[<span data-ttu-id="6f163-133">C#</span><span class="sxs-lookup"><span data-stu-id="6f163-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-managementtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f163-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f163-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-managementtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f163-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f163-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-managementtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f163-136">Java</span><span class="sxs-lookup"><span data-stu-id="6f163-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-managementtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6f163-137">响应</span><span class="sxs-lookup"><span data-stu-id="6f163-137">Response</span></span>
><span data-ttu-id="6f163-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6f163-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementTemplate"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementTemplates/$entity",
  "displayName": "Baseline - Block Legacy Authentication",
  "description": null,
  "category": "identity",
  "parameters": [
    {
      "valueType": "string",
      "displayName": "DisplayName",
      "description": null,
      "jsonDefaultValue": "\"Baseline - Block Legacy Authentication\"",
      "jsonAllowedValues": "null"
    },
    {
      "valueType": "string",
      "displayName": "State",
      "description": null,
      "jsonDefaultValue": "\"enabledForReportingButNotEnforced\"",
      "jsonAllowedValues": "[\"enabled\",\"disabled\",\"enabledForReportingButNotEnforced\"]"
    },
    {
      "valueType": "stringCollection",
      "displayName": "ClientAppTypes",
      "description": null,
      "jsonDefaultValue": "[\"exchangeActiveSync\",\"other\"]",
      "jsonAllowedValues": "[\"exchangeActiveSync\",\"other\"]"
    },
    {
      "valueType": "stringCollection",
      "displayName": "IncludeApplications",
      "description": null,
      "jsonDefaultValue": "[\"All\"]",
      "jsonAllowedValues": "[\"All\"]"
    },
    {
      "valueType": "stringCollection",
      "displayName": "IncludeUsers",
      "description": null,
      "jsonDefaultValue": "[\"None\"]",
      "jsonAllowedValues": "[\"All\",\"None\"]"
    },
    {
      "valueType": "stringCollection",
      "displayName": "IncludeLocations",
      "description": null,
      "jsonDefaultValue": "[\"All\"]",
      "jsonAllowedValues": "[\"All\",\"AllTrusted\"]"
    },
    {
      "valueType": "string",
      "displayName": "GrantControls.Operator",
      "description": null,
      "jsonDefaultValue": "\"OR\"",
      "jsonAllowedValues": "[\"OR\",\"AND\"]"
    },
    {
      "valueType": "stringCollection",
      "displayName": "GrantControls.BuiltInControls",
      "description": null,
      "jsonDefaultValue": "[\"block\"]",
      "jsonAllowedValues": "[\"block\"]"
    }
  ],
  "workloadActions": [
    {
      "actionId": "6a3ad0bc-5d7e-4a49-a105-c559aa4633e1",
      "category": "automated",
      "displayName": "ConditionalAccessPolicy",
      "description": null,
      "service": "AAD",
      "settings": [
        {
          "valueType": "string",
          "displayName": "DisplayName",
          "overwriteAllowed": false,
          "jsonValue": "\"Baseline - Block Legacy Authentication\""
        },
        {
          "valueType": "string",
          "displayName": "State",
          "overwriteAllowed": false,
          "jsonValue": "\"enabledForReportingButNotEnforced\""
        },
        {
          "valueType": "stringCollection",
          "displayName": "ClientAppTypes",
          "overwriteAllowed": false,
          "jsonValue": "[\"exchangeActiveSync\",\"other\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeApplications",
          "overwriteAllowed": false,
          "jsonValue": "[\"All\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeUsers",
          "overwriteAllowed": false,
          "jsonValue": "[\"None\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeLocations",
          "overwriteAllowed": false,
          "jsonValue": "[\"All\"]"
        },
        {
          "valueType": "string",
          "displayName": "GrantControls.Operator",
          "overwriteAllowed": false,
          "jsonValue": "\"OR\""
        },
        {
          "valueType": "stringCollection",
          "displayName": "GrantControls.BuiltInControls",
          "overwriteAllowed": false,
          "jsonValue": "[\"block\"]"
        }
      ]
    }
  ]
}
```
