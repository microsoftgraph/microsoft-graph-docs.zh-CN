---
title: 获取 tenantGroup
description: 读取 tenantGroup 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 9269178355aac2f864952d79d06e9592717caa48
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441107"
---
# <a name="get-tenantgroup"></a><span data-ttu-id="ffc59-103">获取 tenantGroup</span><span class="sxs-lookup"><span data-stu-id="ffc59-103">Get tenantGroup</span></span>
<span data-ttu-id="ffc59-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="ffc59-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffc59-105">读取 [tenantGroup](../resources/managedtenants-tenantgroup.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ffc59-105">Read the properties and relationships of a [tenantGroup](../resources/managedtenants-tenantgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffc59-106">权限</span><span class="sxs-lookup"><span data-stu-id="ffc59-106">Permissions</span></span>
<span data-ttu-id="ffc59-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ffc59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffc59-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ffc59-109">Permission type</span></span>|<span data-ttu-id="ffc59-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ffc59-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffc59-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ffc59-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ffc59-112">ManagedTenants.Read.All、ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffc59-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="ffc59-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ffc59-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffc59-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffc59-114">Not supported.</span></span>|
|<span data-ttu-id="ffc59-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ffc59-115">Application</span></span>|<span data-ttu-id="ffc59-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffc59-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffc59-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffc59-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantGroups/{tenantGroupId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ffc59-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ffc59-118">Optional query parameters</span></span>
<span data-ttu-id="ffc59-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="ffc59-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ffc59-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ffc59-120">Request headers</span></span>
|<span data-ttu-id="ffc59-121">名称</span><span class="sxs-lookup"><span data-stu-id="ffc59-121">Name</span></span>|<span data-ttu-id="ffc59-122">说明</span><span class="sxs-lookup"><span data-stu-id="ffc59-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ffc59-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffc59-123">Authorization</span></span>|<span data-ttu-id="ffc59-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ffc59-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffc59-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ffc59-126">Request body</span></span>
<span data-ttu-id="ffc59-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ffc59-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffc59-128">响应</span><span class="sxs-lookup"><span data-stu-id="ffc59-128">Response</span></span>

<span data-ttu-id="ffc59-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [tenantGroup](../resources/managedtenants-tenantgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ffc59-129">If successful, this method returns a `200 OK` response code and a [tenantGroup](../resources/managedtenants-tenantgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ffc59-130">示例</span><span class="sxs-lookup"><span data-stu-id="ffc59-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ffc59-131">请求</span><span class="sxs-lookup"><span data-stu-id="ffc59-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ffc59-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ffc59-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tenantgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantGroups/{tenantGroupId}
```
# <a name="c"></a>[<span data-ttu-id="ffc59-133">C#</span><span class="sxs-lookup"><span data-stu-id="ffc59-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tenantgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ffc59-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ffc59-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tenantgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ffc59-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ffc59-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tenantgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ffc59-136">Java</span><span class="sxs-lookup"><span data-stu-id="ffc59-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tenantgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ffc59-137">响应</span><span class="sxs-lookup"><span data-stu-id="ffc59-137">Response</span></span>
><span data-ttu-id="ffc59-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ffc59-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantGroup"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantGroups/$entity",
    "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
    "displayName": "Default",
    "allTenantsIncluded": true,
    "tenantIds": [],
    "managementIntents": [
        {
            "managementIntentId": "586895ab-8a59-4b79-be25-b06949a819bb",
            "managementIntentDisplayName": "Default Baseline",
            "managementTemplates": [
                {
                    "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
                    "displayName": "Baseline - Block Legacy Authentication",
                    "category": "identity"
                },
                {
                    "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
                    "displayName": "Baseline - Require MFA for Admins",
                    "category": "identity"
                },
                {
                    "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
                    "displayName": "Baseline - Require MFA for end users",
                    "category": "identity"
                },
                {
                    "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
                    "displayName": "Baseline - Enroll devices in MEM",
                    "category": "devices"
                },
                {
                    "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
                    "displayName": "Baseline - Setup Compliance Policy for Windows 10 devices",
                    "category": "devices"
                },
                {
                    "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
                    "displayName": "Baseline - Setup Microsoft Defender Antivirus Policy for Windows 10 devices",
                    "category": "devices"
                }
            ]
        }
    ],
    "managementActions": [
        {
            "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
            "managementActionId": "eac82706-9f32-4274-ba5b-cf1f8ecf042b"
        },
        {
            "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
            "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5"
        },
        {
            "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
            "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2"
        },
        {
            "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
            "managementActionId": "e96a8cdb-0435-4808-9956-cf6b8ae77aa6"
        },
        {
            "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
            "managementActionId": "55f8da1a-4eec-4fb2-9c58-4c4b3cdf7222"
        },
        {
            "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
            "managementActionId": "b22a4713-8428-4952-8cac-d48962ecbdc9"
        }
    ]
}
```
