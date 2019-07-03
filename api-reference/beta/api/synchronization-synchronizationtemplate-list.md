---
title: 列出现有同步模板
description: 列出与给定应用程序或服务主体相关联的同步模板。
localization_priority: Normal
ms.openlocfilehash: 34307df326d122bbea5d89d095b6513d3668ccb5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458141"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="fe95e-103">列出现有同步模板</span><span class="sxs-lookup"><span data-stu-id="fe95e-103">List existing synchronization templates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe95e-104">列出与给定应用程序或服务主体相关联的同步模板。</span><span class="sxs-lookup"><span data-stu-id="fe95e-104">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe95e-105">权限</span><span class="sxs-lookup"><span data-stu-id="fe95e-105">Permissions</span></span>
<span data-ttu-id="fe95e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe95e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe95e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe95e-108">Permission type</span></span>                        | <span data-ttu-id="fe95e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe95e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe95e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe95e-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="fe95e-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe95e-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="fe95e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe95e-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="fe95e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe95e-113">Not supported.</span></span>|
|<span data-ttu-id="fe95e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe95e-114">Application</span></span>                            |<span data-ttu-id="fe95e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe95e-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="fe95e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe95e-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="fe95e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe95e-117">Request headers</span></span>

| <span data-ttu-id="fe95e-118">名称</span><span class="sxs-lookup"><span data-stu-id="fe95e-118">Name</span></span>           | <span data-ttu-id="fe95e-119">类型</span><span class="sxs-lookup"><span data-stu-id="fe95e-119">Type</span></span>    | <span data-ttu-id="fe95e-120">说明</span><span class="sxs-lookup"><span data-stu-id="fe95e-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="fe95e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe95e-121">Authorization</span></span>  | <span data-ttu-id="fe95e-122">string</span><span class="sxs-lookup"><span data-stu-id="fe95e-122">string</span></span>  | <span data-ttu-id="fe95e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe95e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe95e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe95e-125">Request body</span></span>

<span data-ttu-id="fe95e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe95e-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="fe95e-127">响应</span><span class="sxs-lookup"><span data-stu-id="fe95e-127">Response</span></span>

<span data-ttu-id="fe95e-128">如果成功, 此方法在响应`200 OK`正文中返回[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象的响应代码和集合。</span><span class="sxs-lookup"><span data-stu-id="fe95e-128">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="fe95e-129">示例</span><span class="sxs-lookup"><span data-stu-id="fe95e-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fe95e-130">请求</span><span class="sxs-lookup"><span data-stu-id="fe95e-130">Request</span></span>
<span data-ttu-id="fe95e-131">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="fe95e-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fe95e-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fe95e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fe95e-133">C#</span><span class="sxs-lookup"><span data-stu-id="fe95e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe95e-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="fe95e-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fe95e-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="fe95e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fe95e-136">响应</span><span class="sxs-lookup"><span data-stu-id="fe95e-136">Response</span></span>
<span data-ttu-id="fe95e-137">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="fe95e-137">The following is an example of a response.</span></span>
><span data-ttu-id="fe95e-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fe95e-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fe95e-139">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="fe95e-139">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "Slack",
            "factoryTag": "CustomSCIM",
            "schema": {
                    "directories": [],
                    "synchronizationRules": []
                    }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
