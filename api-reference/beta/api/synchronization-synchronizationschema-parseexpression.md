---
title: 'synchronizationSchema: parseExpression'
description: " ( .。。/resources/synchronization_attributemappingsource) 对象。 "
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0ad35d176f2807b2daedc7296a2adc657a285b6f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969156"
---
# <a name="synchronizationschema-parseexpression"></a><span data-ttu-id="eb72a-103">synchronizationSchema: parseExpression</span><span class="sxs-lookup"><span data-stu-id="eb72a-103">synchronizationSchema: parseExpression</span></span>

<span data-ttu-id="eb72a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb72a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb72a-105">将给定的字符串表达式分析为 [attributeMappingSource](../resources/synchronization-attributemappingsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb72a-105">Parse a given string expression into an [attributeMappingSource](../resources/synchronization-attributemappingsource.md) object.</span></span>

<span data-ttu-id="eb72a-106">有关表达式的详细信息，请参阅 [在 Azure Active Directory 中编写属性映射的表达式](/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings)。</span><span class="sxs-lookup"><span data-stu-id="eb72a-106">For more information about expressions, see [Writing Expressions for Attribute Mappings in Azure Active Directory](/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb72a-107">权限</span><span class="sxs-lookup"><span data-stu-id="eb72a-107">Permissions</span></span>
<span data-ttu-id="eb72a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb72a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb72a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb72a-110">Permission type</span></span>                        | <span data-ttu-id="eb72a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb72a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb72a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb72a-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="eb72a-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb72a-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="eb72a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb72a-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="eb72a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb72a-115">Not supported.</span></span>|
|<span data-ttu-id="eb72a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb72a-116">Application</span></span>                            |<span data-ttu-id="eb72a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb72a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb72a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb72a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
POST /servicePrincipals/{id}/synchronization/templates/{id}/schema/parseExpression

```
## <a name="request-headers"></a><span data-ttu-id="eb72a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb72a-119">Request headers</span></span>
| <span data-ttu-id="eb72a-120">名称</span><span class="sxs-lookup"><span data-stu-id="eb72a-120">Name</span></span>       | <span data-ttu-id="eb72a-121">说明</span><span class="sxs-lookup"><span data-stu-id="eb72a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eb72a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb72a-122">Authorization</span></span>  | <span data-ttu-id="eb72a-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="eb72a-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb72a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb72a-124">Request body</span></span>
<span data-ttu-id="eb72a-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="eb72a-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eb72a-126">参数</span><span class="sxs-lookup"><span data-stu-id="eb72a-126">Parameter</span></span>    | <span data-ttu-id="eb72a-127">类型</span><span class="sxs-lookup"><span data-stu-id="eb72a-127">Type</span></span>   |<span data-ttu-id="eb72a-128">说明</span><span class="sxs-lookup"><span data-stu-id="eb72a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb72a-129">表达式</span><span class="sxs-lookup"><span data-stu-id="eb72a-129">expression</span></span>               |<span data-ttu-id="eb72a-130">String</span><span class="sxs-lookup"><span data-stu-id="eb72a-130">String</span></span>               |<span data-ttu-id="eb72a-131">要分析的表达式。</span><span class="sxs-lookup"><span data-stu-id="eb72a-131">Expression to parse.</span></span>|
|<span data-ttu-id="eb72a-132">testInputObject</span><span class="sxs-lookup"><span data-stu-id="eb72a-132">testInputObject</span></span>          |[<span data-ttu-id="eb72a-133">expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="eb72a-133">expressionInputObject</span></span>](../resources/synchronization-expressioninputobject.md)|<span data-ttu-id="eb72a-134">要对表达式进行求值的测试数据对象。</span><span class="sxs-lookup"><span data-stu-id="eb72a-134">Test data object to evaluate expression against.</span></span> <span data-ttu-id="eb72a-135">可选。</span><span class="sxs-lookup"><span data-stu-id="eb72a-135">Optional.</span></span>|
|<span data-ttu-id="eb72a-136">targetAttributeDefinition</span><span class="sxs-lookup"><span data-stu-id="eb72a-136">targetAttributeDefinition</span></span>|[<span data-ttu-id="eb72a-137">attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="eb72a-137">attributeDefinition</span></span>](../resources/synchronization-attributedefinition.md) |<span data-ttu-id="eb72a-138">将映射到此表达式的属性的定义。</span><span class="sxs-lookup"><span data-stu-id="eb72a-138">Definition of the attribute that will be mapped to this expression.</span></span> <span data-ttu-id="eb72a-139">可选。</span><span class="sxs-lookup"><span data-stu-id="eb72a-139">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="eb72a-140">响应</span><span class="sxs-lookup"><span data-stu-id="eb72a-140">Response</span></span>
<span data-ttu-id="eb72a-141">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb72a-141">If successful, this method returns a `200 OK` response code and a [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb72a-142">示例</span><span class="sxs-lookup"><span data-stu-id="eb72a-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eb72a-143">请求</span><span class="sxs-lookup"><span data-stu-id="eb72a-143">Request</span></span>
<span data-ttu-id="eb72a-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eb72a-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eb72a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb72a-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_parseexpression"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
Content-type: application/json

{
    "expression":"Replace([preferredLanguage], \"-\", , , \"_\", ,  )",
    "targetAttributeDefinition":null,
    "testInputObject": {
        definition: null,
        properties:[
            { key: "objectId", value : "66E4A8CC-1B7B-435E-95F8-F06CEA133828" },
            { key: "IsSoftDeleted", value: "false"},
            { key: "accountEnabled", value: "true"},
            { key: "streetAddress", value: "1 Redmond Way"},
            { key: "city", value: "Redmond"},
            { key: "state", value: "WA"},
            { key: "postalCode", value: "98052"},
            { key: "country", value: "USA"},
            { key: "department", value: "Sales"},
            { key: "displayName", value: "John Smith"},
            { key: "extensionAttribute1", value: "Sample 1"},
            { key: "extensionAttribute2", value: "Sample 2"},
            { key: "extensionAttribute3", value: "Sample 3"},
            { key: "extensionAttribute4", value: "Sample 4"},
            { key: "extensionAttribute5", value: "Sample 5"},
            { key: "extensionAttribute6", value: "Sample 6"},
            { key: "extensionAttribute7", value: "Sample 1"},
            { key: "extensionAttribute8", value: "Sample 1"},
            { key: "extensionAttribute9", value: "Sample 1"},
            { key: "extensionAttribute10", value: "Sample 1"},
            { key: "extensionAttribute11", value: "Sample 1"},
            { key: "extensionAttribute12", value: "Sample 1"},
            { key: "extensionAttribute13", value: "Sample 1"},
            { key: "extensionAttribute14", value: "Sample 1"},
            { key: "extensionAttribute15", value: "Sample 1"},
            { key: "givenName", value: "John"},
            { key: "jobTitle", value: "Finance manager"},
            { key: "mail", value: "johns@contoso.com"},
            { key: "mailNickname", value: "johns"},
            { key: "manager", value: "maxs@contoso.com"},
            { key: "mobile", value: "425-555-0010"},
            { key: "onPremisesSecurityIdentifier", value: "66E4A8CC-1B7B-435E-95F8-F06CEA133828"},
            { key: "passwordProfile.password", value: ""},
            { key: "physicalDeliveryOfficeName", value: "Main Office"},
            { key: "preferredLanguage", value: "EN-US"},
            { key: "proxyAddresses", value: ""},
            { key: "surname", value: "Smith"},
            { key: "telephoneNumber", value: "425-555-0011"},
            { key: "userPrincipalName", value: "johns@contoso.com"},
            { key: "appRoleAssignments", "value@odata.type":"#Collection(String)", value: ["Default Assignment"] }
        ]
    }
}
```
# <a name="c"></a>[<span data-ttu-id="eb72a-146">C#</span><span class="sxs-lookup"><span data-stu-id="eb72a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-parseexpression-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb72a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb72a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-parseexpression-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb72a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb72a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-parseexpression-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eb72a-149">响应</span><span class="sxs-lookup"><span data-stu-id="eb72a-149">Response</span></span>
<span data-ttu-id="eb72a-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="eb72a-150">The following is an example of the response.</span></span>

><span data-ttu-id="eb72a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="eb72a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.parseExpressionResponse"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "error": null,
    "evaluationSucceeded": true,
    "evaluationResult": [
        "EN_US"
    ],
    "parsedExpression": {
        "expression": "Replace([preferredLanguage], \"-\", , , \"_\", , )",
        "name": "Replace",
        "parameters": [
            {
                "key": "source",
                "value": {
                    "expression": "[preferredLanguage]",
                    "name": "preferredLanguage",
                    "parameters": [],
                    "type": "Attribute"
                }
            },
            {
                "key": "Find",
                "value": {
                    "expression": "\"-\"",
                    "name": "-",
                    "parameters": [],
                    "type": "Constant"
                }
            },
            {
                "key": "Replacement",
                "value": {
                    "expression": "\"_\"",
                    "name": "_",
                    "parameters": [],
                    "type": "Constant"
                }
            }
        ],
        "type": "Function"
    },
    "parsingSucceeded": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema: parseExpression",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


