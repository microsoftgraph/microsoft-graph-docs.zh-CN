---
title: 获取 managementTemplate
description: 读取 managementTemplate 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: f0bb547fd1e82a7e6ee5a5f7cf1ac51009c51209
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402378"
---
# <a name="get-managementtemplate"></a><span data-ttu-id="d6291-103">获取 managementTemplate</span><span class="sxs-lookup"><span data-stu-id="d6291-103">Get managementTemplate</span></span>
<span data-ttu-id="d6291-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="d6291-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6291-105">读取 [managementTemplate](../resources/managedtenants-managementtemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d6291-105">Read the properties and relationships of a [managementTemplate](../resources/managedtenants-managementtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6291-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6291-106">Permissions</span></span>
<span data-ttu-id="d6291-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6291-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6291-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6291-109">Permission type</span></span>|<span data-ttu-id="d6291-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6291-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6291-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6291-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6291-112">ManagedTenants.Read.All、ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6291-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="d6291-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6291-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6291-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6291-114">Not supported.</span></span>|
|<span data-ttu-id="d6291-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6291-115">Application</span></span>|<span data-ttu-id="d6291-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6291-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6291-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6291-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementTemplates/{managementTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6291-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d6291-118">Optional query parameters</span></span>
<span data-ttu-id="d6291-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="d6291-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6291-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6291-120">Request headers</span></span>
|<span data-ttu-id="d6291-121">名称</span><span class="sxs-lookup"><span data-stu-id="d6291-121">Name</span></span>|<span data-ttu-id="d6291-122">说明</span><span class="sxs-lookup"><span data-stu-id="d6291-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d6291-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6291-123">Authorization</span></span>|<span data-ttu-id="d6291-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6291-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6291-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6291-126">Request body</span></span>
<span data-ttu-id="d6291-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d6291-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6291-128">响应</span><span class="sxs-lookup"><span data-stu-id="d6291-128">Response</span></span>

<span data-ttu-id="d6291-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [managementTemplate](../resources/managedtenants-managementtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6291-129">If successful, this method returns a `200 OK` response code and a [managementTemplate](../resources/managedtenants-managementtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6291-130">示例</span><span class="sxs-lookup"><span data-stu-id="d6291-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6291-131">请求</span><span class="sxs-lookup"><span data-stu-id="d6291-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_managementtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementTemplates/{managementTemplateId}
```


### <a name="response"></a><span data-ttu-id="d6291-132">响应</span><span class="sxs-lookup"><span data-stu-id="d6291-132">Response</span></span>
><span data-ttu-id="d6291-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d6291-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
