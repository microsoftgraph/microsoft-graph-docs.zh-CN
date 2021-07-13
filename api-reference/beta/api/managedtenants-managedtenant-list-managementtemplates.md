---
title: List managementTemplates
description: 获取 managementTemplate 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 0a133a0340d8bfb52da24400a8760b34735d765d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402233"
---
# <a name="list-managementtemplates"></a><span data-ttu-id="1663a-103">List managementTemplates</span><span class="sxs-lookup"><span data-stu-id="1663a-103">List managementTemplates</span></span>
<span data-ttu-id="1663a-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="1663a-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1663a-105">获取 [managementTemplate 对象](../resources/managedtenants-managementtemplate.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="1663a-105">Get a list of the [managementTemplate](../resources/managedtenants-managementtemplate.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="1663a-106">权限</span><span class="sxs-lookup"><span data-stu-id="1663a-106">Permissions</span></span>
<span data-ttu-id="1663a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1663a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1663a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1663a-109">Permission type</span></span>|<span data-ttu-id="1663a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1663a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1663a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1663a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1663a-112">ManagedTenants.Read.All、ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1663a-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="1663a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1663a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1663a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1663a-114">Not supported.</span></span>|
|<span data-ttu-id="1663a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1663a-115">Application</span></span>|<span data-ttu-id="1663a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1663a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1663a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1663a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1663a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1663a-118">Optional query parameters</span></span>
<span data-ttu-id="1663a-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="1663a-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1663a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1663a-120">Request headers</span></span>
|<span data-ttu-id="1663a-121">名称</span><span class="sxs-lookup"><span data-stu-id="1663a-121">Name</span></span>|<span data-ttu-id="1663a-122">说明</span><span class="sxs-lookup"><span data-stu-id="1663a-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1663a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1663a-123">Authorization</span></span>|<span data-ttu-id="1663a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1663a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1663a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1663a-126">Request body</span></span>
<span data-ttu-id="1663a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1663a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1663a-128">响应</span><span class="sxs-lookup"><span data-stu-id="1663a-128">Response</span></span>

<span data-ttu-id="1663a-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [managementTemplate](../resources/managedtenants-managementtemplate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1663a-129">If successful, this method returns a `200 OK` response code and a collection of [managementTemplate](../resources/managedtenants-managementtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1663a-130">示例</span><span class="sxs-lookup"><span data-stu-id="1663a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1663a-131">请求</span><span class="sxs-lookup"><span data-stu-id="1663a-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_managementtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementTemplates
```


### <a name="response"></a><span data-ttu-id="1663a-132">响应</span><span class="sxs-lookup"><span data-stu-id="1663a-132">Response</span></span>
><span data-ttu-id="1663a-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1663a-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managementTemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementTemplates",
  "value": [
    {
      "id": "e5834405-43d2-4815-867d-3dd600308d1c_1",
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
  ]
}
```
