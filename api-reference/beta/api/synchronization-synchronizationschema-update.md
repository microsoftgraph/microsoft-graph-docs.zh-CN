---
title: 更新 synchronizationSchema
description: 更新给定作业或模板的同步架构。 此方法将当前架构完全替换为请求中提供的架构。 若要更新模板的架构, 请对 application 对象进行调用。 您必须是应用程序的所有者。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 63e1ed50035cd7d04775a3af66b0127d6da17395
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869104"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="dc189-106">更新 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="dc189-106">Update synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc189-107">更新给定作业或模板的同步架构。</span><span class="sxs-lookup"><span data-stu-id="dc189-107">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="dc189-108">此方法将当前架构完全替换为请求中提供的架构。</span><span class="sxs-lookup"><span data-stu-id="dc189-108">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="dc189-109">若要更新模板的架构, 请对 application 对象进行调用。</span><span class="sxs-lookup"><span data-stu-id="dc189-109">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="dc189-110">您必须是应用程序的所有者。</span><span class="sxs-lookup"><span data-stu-id="dc189-110">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc189-111">权限</span><span class="sxs-lookup"><span data-stu-id="dc189-111">Permissions</span></span>
<span data-ttu-id="dc189-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc189-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc189-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc189-114">Permission type</span></span>                        | <span data-ttu-id="dc189-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc189-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc189-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc189-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="dc189-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc189-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="dc189-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc189-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="dc189-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc189-119">Not supported.</span></span>|
|<span data-ttu-id="dc189-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc189-120">Application</span></span>                            |<span data-ttu-id="dc189-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc189-121">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="dc189-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc189-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="dc189-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc189-123">Request headers</span></span>

| <span data-ttu-id="dc189-124">名称</span><span class="sxs-lookup"><span data-stu-id="dc189-124">Name</span></span>           | <span data-ttu-id="dc189-125">类型</span><span class="sxs-lookup"><span data-stu-id="dc189-125">Type</span></span>    | <span data-ttu-id="dc189-126">说明</span><span class="sxs-lookup"><span data-stu-id="dc189-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="dc189-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc189-127">Authorization</span></span>  | <span data-ttu-id="dc189-128">string</span><span class="sxs-lookup"><span data-stu-id="dc189-128">string</span></span>  | <span data-ttu-id="dc189-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dc189-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc189-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc189-131">Request body</span></span>

<span data-ttu-id="dc189-132">在请求正文中, 提供[synchronizationSchema](../resources/synchronization-synchronizationschema.md)对象以将现有架构替换为。</span><span class="sxs-lookup"><span data-stu-id="dc189-132">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="dc189-133">响应</span><span class="sxs-lookup"><span data-stu-id="dc189-133">Response</span></span>

<span data-ttu-id="dc189-134">如果成功, 则返回`204 No Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="dc189-134">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="dc189-135">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dc189-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc189-136">示例</span><span class="sxs-lookup"><span data-stu-id="dc189-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dc189-137">请求</span><span class="sxs-lookup"><span data-stu-id="dc189-137">Request</span></span>
<span data-ttu-id="dc189-138">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="dc189-138">The following is an example of a request.</span></span>

><span data-ttu-id="dc189-139">**注意:** 为了提高可读性, 此处显示的请求对象已缩短。</span><span class="sxs-lookup"><span data-stu-id="dc189-139">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="dc189-140">在实际调用中提供所有属性。</span><span class="sxs-lookup"><span data-stu-id="dc189-140">Supply all the properties in an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dc189-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="dc189-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_synchronizationschema"
}-->
```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
Content-type: application/json

{
    "directories": [
        {
            "name": "Azure Active Directory",
            "objects": [
                {
                    "name": "User",
                    "attributes": [
                        {
                            "name": "userPrincipalName",
                            "type": "string"
                        }
                    ]
                },
            ]
        },
        {
            "name": "Salesforce",
        }
    ],
    "synchronizationRules":[
        {
            "name": "USER_TO_USER",
            "sourceDirectoryName": "Azure Active Directory",
            "targetDirectoryName": "Salesforce",
            "objectMappings": [
                {
                    "sourceObjectName": "User",
                    "targetObjectName": "User",
                    "attributeMappings": [
                        {
                            "source": {},
                            "targetAttributeName": "userName"
                        },
                    ]
                },
            ]
        },
    ]
}

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc189-142">C#</span><span class="sxs-lookup"><span data-stu-id="dc189-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc189-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="dc189-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc189-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="dc189-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dc189-145">Java</span><span class="sxs-lookup"><span data-stu-id="dc189-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dc189-146">响应</span><span class="sxs-lookup"><span data-stu-id="dc189-146">Response</span></span>
<span data-ttu-id="dc189-147">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="dc189-147">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationschema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
