---
title: 列出 managementActions
description: 获取 managementAction 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 03aedec0464908bf25deb004e6cbe4bdb5027acb
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402033"
---
# <a name="list-managementactions"></a><span data-ttu-id="dc4b3-103">列出 managementActions</span><span class="sxs-lookup"><span data-stu-id="dc4b3-103">List managementActions</span></span>
<span data-ttu-id="dc4b3-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="dc4b3-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc4b3-105">获取 [managementAction 对象](../resources/managedtenants-managementaction.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="dc4b3-105">Get a list of the [managementAction](../resources/managedtenants-managementaction.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc4b3-106">权限</span><span class="sxs-lookup"><span data-stu-id="dc4b3-106">Permissions</span></span>
<span data-ttu-id="dc4b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc4b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc4b3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc4b3-109">Permission type</span></span>|<span data-ttu-id="dc4b3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc4b3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc4b3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc4b3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc4b3-112">ManagedTenants.Read.All、ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc4b3-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="dc4b3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc4b3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc4b3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc4b3-114">Not supported.</span></span>|
|<span data-ttu-id="dc4b3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc4b3-115">Application</span></span>|<span data-ttu-id="dc4b3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc4b3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc4b3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc4b3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementActions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dc4b3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dc4b3-118">Optional query parameters</span></span>
<span data-ttu-id="dc4b3-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="dc4b3-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc4b3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc4b3-120">Request headers</span></span>
|<span data-ttu-id="dc4b3-121">名称</span><span class="sxs-lookup"><span data-stu-id="dc4b3-121">Name</span></span>|<span data-ttu-id="dc4b3-122">说明</span><span class="sxs-lookup"><span data-stu-id="dc4b3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dc4b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc4b3-123">Authorization</span></span>|<span data-ttu-id="dc4b3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dc4b3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc4b3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc4b3-126">Request body</span></span>
<span data-ttu-id="dc4b3-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dc4b3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc4b3-128">响应</span><span class="sxs-lookup"><span data-stu-id="dc4b3-128">Response</span></span>

<span data-ttu-id="dc4b3-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [managementAction](../resources/managedtenants-managementaction.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dc4b3-129">If successful, this method returns a `200 OK` response code and a collection of [managementAction](../resources/managedtenants-managementaction.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dc4b3-130">示例</span><span class="sxs-lookup"><span data-stu-id="dc4b3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dc4b3-131">请求</span><span class="sxs-lookup"><span data-stu-id="dc4b3-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_managementaction"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActions
```


### <a name="response"></a><span data-ttu-id="dc4b3-132">响应</span><span class="sxs-lookup"><span data-stu-id="dc4b3-132">Response</span></span>
><span data-ttu-id="dc4b3-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dc4b3-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managementAction)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementActions",
    "value": [
        {
            "id": "4274db74-99c4-40be-bbeb-da4351136be2",
            "referenceTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
            "displayName": "Baseline - Require MFA for end users",
            "description": null,
            "category": "identity",
            "workloadActions": [
                {
                    "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
                    "category": "automated",
                    "displayName": "ConditionalAccessPolicy",
                    "description": null,
                    "service": "AAD",
                    "settings": [
                        {
                            "valueType": "string",
                            "displayName": "DisplayName",
                            "overwriteAllowed": false,
                            "jsonValue": "\"Baseline - Require MFA for end users\""
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
                            "jsonValue": "[\"All\"]"
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
                            "jsonValue": "[\"mfa\"]"
                        }
                    ]
                }
            ]
        }
    ]
}
```
