---
title: 'synchronizationSchema: parseExpression'
description: '(../resources/synchronization_attributemappingsource.md) 对象。 '
localization_priority: Normal
ms.openlocfilehash: 79cb683571fa7a5e1b48f93a1805ae5d7a4f7202
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536146"
---
# <a name="synchronizationschema-parseexpression"></a><span data-ttu-id="34046-103">synchronizationSchema: parseExpression</span><span class="sxs-lookup"><span data-stu-id="34046-103">synchronizationSchema: parseExpression</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34046-104">将给定的字符串表达式解析为 [attributeMappingSource | (.。。/resources/synchronization_attributemappingsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="34046-104">Parse a given string expression into an [attributeMappingSource|(../resources/synchronization_attributemappingsource.md) object.</span></span> 

<span data-ttu-id="34046-105">有关表达式的详细信息, 请参阅[在 Azure Active Directory 中编写属性映射的表达式](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings)。</span><span class="sxs-lookup"><span data-stu-id="34046-105">For more information about expressions, see [Writing Expressions for Attribute Mappings in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span></span>

## <a name="permissions"></a><span data-ttu-id="34046-106">权限</span><span class="sxs-lookup"><span data-stu-id="34046-106">Permissions</span></span>
<span data-ttu-id="34046-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34046-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34046-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="34046-109">Permission type</span></span>                        | <span data-ttu-id="34046-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="34046-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="34046-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34046-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="34046-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34046-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="34046-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34046-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="34046-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="34046-114">Not supported.</span></span>|
|<span data-ttu-id="34046-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="34046-115">Application</span></span>                            |<span data-ttu-id="34046-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="34046-116">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="34046-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34046-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
POST /servicePrincipals/{id}/synchronization/templates/{id}/schema/parseExpression

```
## <a name="request-headers"></a><span data-ttu-id="34046-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="34046-118">Request headers</span></span>
| <span data-ttu-id="34046-119">名称</span><span class="sxs-lookup"><span data-stu-id="34046-119">Name</span></span>       | <span data-ttu-id="34046-120">说明</span><span class="sxs-lookup"><span data-stu-id="34046-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="34046-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="34046-121">Authorization</span></span>  | <span data-ttu-id="34046-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="34046-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="34046-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="34046-123">Request body</span></span>
<span data-ttu-id="34046-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="34046-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="34046-125">参数</span><span class="sxs-lookup"><span data-stu-id="34046-125">Parameter</span></span>    | <span data-ttu-id="34046-126">类型</span><span class="sxs-lookup"><span data-stu-id="34046-126">Type</span></span>   |<span data-ttu-id="34046-127">说明</span><span class="sxs-lookup"><span data-stu-id="34046-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34046-128">表达式</span><span class="sxs-lookup"><span data-stu-id="34046-128">expression</span></span>               |<span data-ttu-id="34046-129">String</span><span class="sxs-lookup"><span data-stu-id="34046-129">String</span></span>               |<span data-ttu-id="34046-130">要分析的表达式。</span><span class="sxs-lookup"><span data-stu-id="34046-130">Expression to parse.</span></span>|
|<span data-ttu-id="34046-131">testInputObject</span><span class="sxs-lookup"><span data-stu-id="34046-131">testInputObject</span></span>          |[<span data-ttu-id="34046-132">expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="34046-132">expressionInputObject</span></span>](../resources/synchronization-expressioninputobject.md)|<span data-ttu-id="34046-133">要对表达式进行求值的测试数据对象。</span><span class="sxs-lookup"><span data-stu-id="34046-133">Test data object to evaluate expression against.</span></span> <span data-ttu-id="34046-134">可选。</span><span class="sxs-lookup"><span data-stu-id="34046-134">Optional.</span></span>|
|<span data-ttu-id="34046-135">targetAttributeDefinition</span><span class="sxs-lookup"><span data-stu-id="34046-135">targetAttributeDefinition</span></span>|[<span data-ttu-id="34046-136">attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="34046-136">attributeDefinition</span></span>](../resources/synchronization-attributedefinition.md) |<span data-ttu-id="34046-137">将映射到此表达式的属性的定义。</span><span class="sxs-lookup"><span data-stu-id="34046-137">Definition of the attribute that will be mapped to this expression.</span></span> <span data-ttu-id="34046-138">可选。</span><span class="sxs-lookup"><span data-stu-id="34046-138">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="34046-139">响应</span><span class="sxs-lookup"><span data-stu-id="34046-139">Response</span></span>
<span data-ttu-id="34046-140">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md)对象。</span><span class="sxs-lookup"><span data-stu-id="34046-140">If successful, this method returns a `200 OK` response code and a [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34046-141">示例</span><span class="sxs-lookup"><span data-stu-id="34046-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="34046-142">请求</span><span class="sxs-lookup"><span data-stu-id="34046-142">Request</span></span>
<span data-ttu-id="34046-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="34046-143">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="34046-144">响应</span><span class="sxs-lookup"><span data-stu-id="34046-144">Response</span></span>
<span data-ttu-id="34046-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="34046-145">The following is an example of the response.</span></span> 

><span data-ttu-id="34046-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="34046-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="34046-148">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="34046-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="34046-149">C#</span><span class="sxs-lookup"><span data-stu-id="34046-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationschema_parseexpression-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="34046-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="34046-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationschema_parseexpression-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-parseexpression.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-parseexpression.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
