---
title: 'synchronizationSchema: parseExpression'
description: '(../ resources/synchronization_attributemappingsource.md) 对象。 '
localization_priority: Normal
ms.openlocfilehash: dbde03b9ae85377801ad894c8b8ca22c6baebc85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811023"
---
# <a name="synchronizationschema-parseexpression"></a><span data-ttu-id="d8b72-103">synchronizationSchema: parseExpression</span><span class="sxs-lookup"><span data-stu-id="d8b72-103">synchronizationSchema: parseExpression</span></span>

> <span data-ttu-id="d8b72-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d8b72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8b72-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d8b72-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8b72-106">分析给定的字符串表达式转换 [attributeMappingSource | (.../ resources/synchronization_attributemappingsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d8b72-106">Parse a given string expression into an [attributeMappingSource|(../resources/synchronization_attributemappingsource.md) object.</span></span> 

<span data-ttu-id="d8b72-107">有关表达式的详细信息，请参阅[在 Azure Active Directory 中的属性映射的编写表达式](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings)。</span><span class="sxs-lookup"><span data-stu-id="d8b72-107">For more information about expressions, see [Writing Expressions for Attribute Mappings in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span></span>

## <a name="permissions"></a><span data-ttu-id="d8b72-108">权限</span><span class="sxs-lookup"><span data-stu-id="d8b72-108">Permissions</span></span>
<span data-ttu-id="d8b72-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8b72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8b72-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8b72-111">Permission type</span></span>                        | <span data-ttu-id="d8b72-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8b72-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8b72-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8b72-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="d8b72-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8b72-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="d8b72-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8b72-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="d8b72-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8b72-116">Not supported.</span></span>|
|<span data-ttu-id="d8b72-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8b72-117">Application</span></span>                            |<span data-ttu-id="d8b72-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8b72-118">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="d8b72-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8b72-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
POST /servicePrincipals/{id}/synchronization/templates/{id}/schema/parseExpression

```
## <a name="request-headers"></a><span data-ttu-id="d8b72-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8b72-120">Request headers</span></span>
| <span data-ttu-id="d8b72-121">名称</span><span class="sxs-lookup"><span data-stu-id="d8b72-121">Name</span></span>       | <span data-ttu-id="d8b72-122">说明</span><span class="sxs-lookup"><span data-stu-id="d8b72-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d8b72-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8b72-123">Authorization</span></span>  | <span data-ttu-id="d8b72-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d8b72-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8b72-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8b72-125">Request body</span></span>
<span data-ttu-id="d8b72-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d8b72-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d8b72-127">参数</span><span class="sxs-lookup"><span data-stu-id="d8b72-127">Parameter</span></span>    | <span data-ttu-id="d8b72-128">类型</span><span class="sxs-lookup"><span data-stu-id="d8b72-128">Type</span></span>   |<span data-ttu-id="d8b72-129">Description</span><span class="sxs-lookup"><span data-stu-id="d8b72-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8b72-130">表达式</span><span class="sxs-lookup"><span data-stu-id="d8b72-130">expression</span></span>               |<span data-ttu-id="d8b72-131">字符串</span><span class="sxs-lookup"><span data-stu-id="d8b72-131">String</span></span>               |<span data-ttu-id="d8b72-132">若要分析的表达式。</span><span class="sxs-lookup"><span data-stu-id="d8b72-132">Expression to parse.</span></span>|
|<span data-ttu-id="d8b72-133">testInputObject</span><span class="sxs-lookup"><span data-stu-id="d8b72-133">testInputObject</span></span>          |[<span data-ttu-id="d8b72-134">expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="d8b72-134">expressionInputObject</span></span>](../resources/synchronization-expressioninputobject.md)|<span data-ttu-id="d8b72-135">测试针对表达式进行求值的数据对象。</span><span class="sxs-lookup"><span data-stu-id="d8b72-135">Test data object to evaluate expression against.</span></span> <span data-ttu-id="d8b72-136">可选。</span><span class="sxs-lookup"><span data-stu-id="d8b72-136">Optional.</span></span>|
|<span data-ttu-id="d8b72-137">targetAttributeDefinition</span><span class="sxs-lookup"><span data-stu-id="d8b72-137">targetAttributeDefinition</span></span>|[<span data-ttu-id="d8b72-138">attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="d8b72-138">attributeDefinition</span></span>](../resources/synchronization-attributedefinition.md) |<span data-ttu-id="d8b72-139">将映射到此表达式的属性的定义。</span><span class="sxs-lookup"><span data-stu-id="d8b72-139">Definition of the attribute that will be mapped to this expression.</span></span> <span data-ttu-id="d8b72-140">可选。</span><span class="sxs-lookup"><span data-stu-id="d8b72-140">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="d8b72-141">响应</span><span class="sxs-lookup"><span data-stu-id="d8b72-141">Response</span></span>
<span data-ttu-id="d8b72-142">如果成功，此方法返回`200 OK`响应代码和响应正文中的[parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d8b72-142">If successful, this method returns a `200 OK` response code and a [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8b72-143">示例</span><span class="sxs-lookup"><span data-stu-id="d8b72-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d8b72-144">请求</span><span class="sxs-lookup"><span data-stu-id="d8b72-144">Request</span></span>
<span data-ttu-id="d8b72-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d8b72-145">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d8b72-146">响应</span><span class="sxs-lookup"><span data-stu-id="d8b72-146">Response</span></span>
<span data-ttu-id="d8b72-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d8b72-147">The following is an example of the response.</span></span> 

><span data-ttu-id="d8b72-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d8b72-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: parseExpression",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
