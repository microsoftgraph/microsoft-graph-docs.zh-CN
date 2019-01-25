---
title: 更新 synchronizationSchema
description: 更新给定的作业或模板的同步架构。 此方法完全请求中提供的一个与替换当前架构。 若要更新的模板架构，进行应用程序对象上的呼叫。 您必须是应用程序的所有者。
localization_priority: Normal
ms.openlocfilehash: 13ee7d996b0e02834b77cd222380747c02d7fcc2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525547"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="368c2-106">更新 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="368c2-106">Update synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="368c2-107">更新给定的作业或模板的同步架构。</span><span class="sxs-lookup"><span data-stu-id="368c2-107">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="368c2-108">此方法完全请求中提供的一个与替换当前架构。</span><span class="sxs-lookup"><span data-stu-id="368c2-108">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="368c2-109">若要更新的模板架构，进行应用程序对象上的呼叫。</span><span class="sxs-lookup"><span data-stu-id="368c2-109">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="368c2-110">您必须是应用程序的所有者。</span><span class="sxs-lookup"><span data-stu-id="368c2-110">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="368c2-111">权限</span><span class="sxs-lookup"><span data-stu-id="368c2-111">Permissions</span></span>
<span data-ttu-id="368c2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="368c2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="368c2-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="368c2-114">Permission type</span></span>                        | <span data-ttu-id="368c2-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="368c2-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="368c2-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="368c2-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="368c2-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="368c2-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="368c2-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="368c2-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="368c2-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="368c2-119">Not supported.</span></span>|
|<span data-ttu-id="368c2-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="368c2-120">Application</span></span>                            |<span data-ttu-id="368c2-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="368c2-121">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="368c2-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="368c2-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="368c2-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="368c2-123">Request headers</span></span>

| <span data-ttu-id="368c2-124">名称</span><span class="sxs-lookup"><span data-stu-id="368c2-124">Name</span></span>           | <span data-ttu-id="368c2-125">类型</span><span class="sxs-lookup"><span data-stu-id="368c2-125">Type</span></span>    | <span data-ttu-id="368c2-126">说明</span><span class="sxs-lookup"><span data-stu-id="368c2-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="368c2-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="368c2-127">Authorization</span></span>  | <span data-ttu-id="368c2-128">string</span><span class="sxs-lookup"><span data-stu-id="368c2-128">string</span></span>  | <span data-ttu-id="368c2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="368c2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="368c2-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="368c2-131">Request body</span></span>

<span data-ttu-id="368c2-132">在请求正文中，提供要替换与现有的架构的[synchronizationSchema](../resources/synchronization-synchronizationschema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="368c2-132">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="368c2-133">响应</span><span class="sxs-lookup"><span data-stu-id="368c2-133">Response</span></span>

<span data-ttu-id="368c2-134">如果成功，返回`204 No Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="368c2-134">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="368c2-135">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="368c2-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="368c2-136">示例</span><span class="sxs-lookup"><span data-stu-id="368c2-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="368c2-137">请求</span><span class="sxs-lookup"><span data-stu-id="368c2-137">Request</span></span>
<span data-ttu-id="368c2-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="368c2-138">The following is an example of a request.</span></span>

><span data-ttu-id="368c2-139">**注意：** 为便于阅读将被截如下所示的请求对象。</span><span class="sxs-lookup"><span data-stu-id="368c2-139">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="368c2-140">提供实际呼叫中的所有属性。</span><span class="sxs-lookup"><span data-stu-id="368c2-140">Supply all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationschema"
}-->
```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema

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

##### <a name="response"></a><span data-ttu-id="368c2-141">响应</span><span class="sxs-lookup"><span data-stu-id="368c2-141">Response</span></span>
<span data-ttu-id="368c2-142">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="368c2-142">The following is an example of a response.</span></span>
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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
