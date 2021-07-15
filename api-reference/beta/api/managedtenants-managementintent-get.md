---
title: 获取 managementIntent
description: 读取 managementIntent 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: f074678ca774e66c659465fe4f7fc37fedd25cd0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442580"
---
# <a name="get-managementintent"></a><span data-ttu-id="534ab-103">获取 managementIntent</span><span class="sxs-lookup"><span data-stu-id="534ab-103">Get managementIntent</span></span>
<span data-ttu-id="534ab-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="534ab-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="534ab-105">读取 [managementIntent](../resources/managedtenants-managementintent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="534ab-105">Read the properties and relationships of a [managementIntent](../resources/managedtenants-managementintent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="534ab-106">权限</span><span class="sxs-lookup"><span data-stu-id="534ab-106">Permissions</span></span>
<span data-ttu-id="534ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="534ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="534ab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="534ab-109">Permission type</span></span>|<span data-ttu-id="534ab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="534ab-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="534ab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="534ab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="534ab-112">ManagedTenants.Read.All、ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="534ab-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="534ab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="534ab-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="534ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="534ab-114">Not supported.</span></span>|
|<span data-ttu-id="534ab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="534ab-115">Application</span></span>|<span data-ttu-id="534ab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="534ab-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="534ab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="534ab-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementIntents/{managementIntentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="534ab-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="534ab-118">Optional query parameters</span></span>
<span data-ttu-id="534ab-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="534ab-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="534ab-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="534ab-120">Request headers</span></span>
|<span data-ttu-id="534ab-121">名称</span><span class="sxs-lookup"><span data-stu-id="534ab-121">Name</span></span>|<span data-ttu-id="534ab-122">说明</span><span class="sxs-lookup"><span data-stu-id="534ab-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="534ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="534ab-123">Authorization</span></span>|<span data-ttu-id="534ab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="534ab-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="534ab-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="534ab-126">Request body</span></span>
<span data-ttu-id="534ab-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="534ab-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="534ab-128">响应</span><span class="sxs-lookup"><span data-stu-id="534ab-128">Response</span></span>

<span data-ttu-id="534ab-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [managementIntent](../resources/managedtenants-managementintent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="534ab-129">If successful, this method returns a `200 OK` response code and a [managementIntent](../resources/managedtenants-managementintent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="534ab-130">示例</span><span class="sxs-lookup"><span data-stu-id="534ab-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="534ab-131">请求</span><span class="sxs-lookup"><span data-stu-id="534ab-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="534ab-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="534ab-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_managementintent"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementIntents/{managementIntentId}
```
# <a name="c"></a>[<span data-ttu-id="534ab-133">C#</span><span class="sxs-lookup"><span data-stu-id="534ab-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-managementintent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="534ab-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="534ab-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-managementintent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="534ab-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="534ab-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-managementintent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="534ab-136">Java</span><span class="sxs-lookup"><span data-stu-id="534ab-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-managementintent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="534ab-137">响应</span><span class="sxs-lookup"><span data-stu-id="534ab-137">Response</span></span>
><span data-ttu-id="534ab-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="534ab-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementIntent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementIntents/$entity",
    "id": "586895ab-8a59-4b79-be25-b06949a819bb",
    "displayName": "Default Baseline",
    "isGlobal": true,
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
```
