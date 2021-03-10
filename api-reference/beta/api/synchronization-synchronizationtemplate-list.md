---
title: 列出现有同步模板
description: 列出与给定应用程序或服务主体关联的同步模板。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 323a870c94ea465ce0cbfa84903090ee944a5ee7
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625926"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="4acac-103">列出现有同步模板</span><span class="sxs-lookup"><span data-stu-id="4acac-103">List existing synchronization templates</span></span>

<span data-ttu-id="4acac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4acac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4acac-105">列出与给定应用程序或服务主体关联的同步模板。</span><span class="sxs-lookup"><span data-stu-id="4acac-105">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="4acac-106">权限</span><span class="sxs-lookup"><span data-stu-id="4acac-106">Permissions</span></span>
<span data-ttu-id="4acac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4acac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4acac-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4acac-109">Permission type</span></span>                        | <span data-ttu-id="4acac-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4acac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4acac-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4acac-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="4acac-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4acac-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="4acac-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4acac-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4acac-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4acac-114">Not supported.</span></span>|
|<span data-ttu-id="4acac-115">Application</span><span class="sxs-lookup"><span data-stu-id="4acac-115">Application</span></span>                            |<span data-ttu-id="4acac-116">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4acac-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

### <a name="http-request"></a><span data-ttu-id="4acac-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4acac-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="4acac-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4acac-118">Request headers</span></span>

| <span data-ttu-id="4acac-119">名称</span><span class="sxs-lookup"><span data-stu-id="4acac-119">Name</span></span>           | <span data-ttu-id="4acac-120">类型</span><span class="sxs-lookup"><span data-stu-id="4acac-120">Type</span></span>    | <span data-ttu-id="4acac-121">说明</span><span class="sxs-lookup"><span data-stu-id="4acac-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="4acac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4acac-122">Authorization</span></span>  | <span data-ttu-id="4acac-123">string</span><span class="sxs-lookup"><span data-stu-id="4acac-123">string</span></span>  | <span data-ttu-id="4acac-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4acac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4acac-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4acac-126">Request body</span></span>

<span data-ttu-id="4acac-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4acac-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="4acac-128">响应</span><span class="sxs-lookup"><span data-stu-id="4acac-128">Response</span></span>

<span data-ttu-id="4acac-129">如果成功，此方法在响应正文中返回 `200 OK` [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) 对象的响应代码和集合。</span><span class="sxs-lookup"><span data-stu-id="4acac-129">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="4acac-130">示例</span><span class="sxs-lookup"><span data-stu-id="4acac-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4acac-131">请求</span><span class="sxs-lookup"><span data-stu-id="4acac-131">Request</span></span>
<span data-ttu-id="4acac-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="4acac-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4acac-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4acac-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```
# <a name="c"></a>[<span data-ttu-id="4acac-134">C#</span><span class="sxs-lookup"><span data-stu-id="4acac-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4acac-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4acac-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4acac-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4acac-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4acac-137">Java</span><span class="sxs-lookup"><span data-stu-id="4acac-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4acac-138">响应</span><span class="sxs-lookup"><span data-stu-id="4acac-138">Response</span></span>
<span data-ttu-id="4acac-139">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="4acac-139">The following is an example of a response.</span></span>
><span data-ttu-id="4acac-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4acac-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4acac-141">在实际调用中将返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4acac-141">All the properties will be returned in an actual call.</span></span>
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


