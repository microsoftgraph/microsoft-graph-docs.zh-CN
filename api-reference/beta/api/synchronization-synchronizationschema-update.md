---
title: 更新 synchronizationSchema
description: 更新给定作业或模板的同步架构。 此方法将当前架构完全替换为请求中提供的架构。 若要更新模板的架构，请对 application 对象进行调用。 您必须是应用程序的所有者。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8211b5fc15e6648fea9ba1b4b44c28a93eb5e0f5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452902"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="e2eaf-106">更新 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="e2eaf-106">Update synchronizationSchema</span></span>

<span data-ttu-id="e2eaf-107">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e2eaf-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2eaf-108">更新给定作业或模板的同步架构。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-108">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="e2eaf-109">此方法将当前架构完全替换为请求中提供的架构。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-109">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="e2eaf-110">若要更新模板的架构，请对 application 对象进行调用。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-110">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="e2eaf-111">您必须是应用程序的所有者。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-111">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2eaf-112">权限</span><span class="sxs-lookup"><span data-stu-id="e2eaf-112">Permissions</span></span>
<span data-ttu-id="e2eaf-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2eaf-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2eaf-115">Permission type</span></span>                        | <span data-ttu-id="e2eaf-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2eaf-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2eaf-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2eaf-117">Delegated (work or school account)</span></span>     |<span data-ttu-id="e2eaf-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2eaf-118">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e2eaf-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2eaf-119">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e2eaf-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-120">Not supported.</span></span>|
|<span data-ttu-id="e2eaf-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2eaf-121">Application</span></span>                            |<span data-ttu-id="e2eaf-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-122">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="e2eaf-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2eaf-123">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="e2eaf-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2eaf-124">Request headers</span></span>

| <span data-ttu-id="e2eaf-125">名称</span><span class="sxs-lookup"><span data-stu-id="e2eaf-125">Name</span></span>           | <span data-ttu-id="e2eaf-126">类型</span><span class="sxs-lookup"><span data-stu-id="e2eaf-126">Type</span></span>    | <span data-ttu-id="e2eaf-127">说明</span><span class="sxs-lookup"><span data-stu-id="e2eaf-127">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e2eaf-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2eaf-128">Authorization</span></span>  | <span data-ttu-id="e2eaf-129">string</span><span class="sxs-lookup"><span data-stu-id="e2eaf-129">string</span></span>  | <span data-ttu-id="e2eaf-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2eaf-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2eaf-132">Request body</span></span>

<span data-ttu-id="e2eaf-133">在请求正文中，提供[synchronizationSchema](../resources/synchronization-synchronizationschema.md)对象以将现有架构替换为。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-133">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="e2eaf-134">响应</span><span class="sxs-lookup"><span data-stu-id="e2eaf-134">Response</span></span>

<span data-ttu-id="e2eaf-135">如果成功，则返回`204 No Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-135">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="e2eaf-136">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2eaf-137">示例</span><span class="sxs-lookup"><span data-stu-id="e2eaf-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e2eaf-138">请求</span><span class="sxs-lookup"><span data-stu-id="e2eaf-138">Request</span></span>
<span data-ttu-id="e2eaf-139">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-139">The following is an example of a request.</span></span>

><span data-ttu-id="e2eaf-140">**注意：** 为了提高可读性，此处显示的请求对象已缩短。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-140">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="e2eaf-141">在实际调用中提供所有属性。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-141">Supply all the properties in an actual call.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2eaf-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2eaf-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e2eaf-143">C#</span><span class="sxs-lookup"><span data-stu-id="e2eaf-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2eaf-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2eaf-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2eaf-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2eaf-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e2eaf-146">响应</span><span class="sxs-lookup"><span data-stu-id="e2eaf-146">Response</span></span>
<span data-ttu-id="e2eaf-147">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="e2eaf-147">The following is an example of a response.</span></span>
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
