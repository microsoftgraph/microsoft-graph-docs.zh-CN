---
title: 更新 synchronizationSchema
description: 更新给定的作业或模板的同步架构。 此方法完全请求中提供的一个与替换当前架构。 若要更新的模板架构，进行应用程序对象上的呼叫。 您必须是应用程序的所有者。
localization_priority: Normal
ms.openlocfilehash: d4f3f3540fe0d304b4edc3a5fcaec7b3366dbb0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826136"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="6ca47-106">更新 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="6ca47-106">Update synchronizationSchema</span></span>

> <span data-ttu-id="6ca47-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6ca47-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ca47-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6ca47-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ca47-109">更新给定的作业或模板的同步架构。</span><span class="sxs-lookup"><span data-stu-id="6ca47-109">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="6ca47-110">此方法完全请求中提供的一个与替换当前架构。</span><span class="sxs-lookup"><span data-stu-id="6ca47-110">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="6ca47-111">若要更新的模板架构，进行应用程序对象上的呼叫。</span><span class="sxs-lookup"><span data-stu-id="6ca47-111">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="6ca47-112">您必须是应用程序的所有者。</span><span class="sxs-lookup"><span data-stu-id="6ca47-112">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ca47-113">权限</span><span class="sxs-lookup"><span data-stu-id="6ca47-113">Permissions</span></span>
<span data-ttu-id="6ca47-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ca47-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ca47-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ca47-116">Permission type</span></span>                        | <span data-ttu-id="6ca47-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ca47-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ca47-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ca47-118">Delegated (work or school account)</span></span>     |<span data-ttu-id="6ca47-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ca47-119">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="6ca47-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ca47-120">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="6ca47-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ca47-121">Not supported.</span></span>|
|<span data-ttu-id="6ca47-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ca47-122">Application</span></span>                            |<span data-ttu-id="6ca47-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ca47-123">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="6ca47-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ca47-124">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="6ca47-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ca47-125">Request headers</span></span>

| <span data-ttu-id="6ca47-126">名称</span><span class="sxs-lookup"><span data-stu-id="6ca47-126">Name</span></span>           | <span data-ttu-id="6ca47-127">类型</span><span class="sxs-lookup"><span data-stu-id="6ca47-127">Type</span></span>    | <span data-ttu-id="6ca47-128">说明</span><span class="sxs-lookup"><span data-stu-id="6ca47-128">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="6ca47-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ca47-129">Authorization</span></span>  | <span data-ttu-id="6ca47-130">string</span><span class="sxs-lookup"><span data-stu-id="6ca47-130">string</span></span>  | <span data-ttu-id="6ca47-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ca47-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ca47-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ca47-133">Request body</span></span>

<span data-ttu-id="6ca47-134">在请求正文中，提供要替换与现有的架构的[synchronizationSchema](../resources/synchronization-synchronizationschema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6ca47-134">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="6ca47-135">响应</span><span class="sxs-lookup"><span data-stu-id="6ca47-135">Response</span></span>

<span data-ttu-id="6ca47-136">如果成功，返回`204 No Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="6ca47-136">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="6ca47-137">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="6ca47-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ca47-138">示例</span><span class="sxs-lookup"><span data-stu-id="6ca47-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6ca47-139">请求</span><span class="sxs-lookup"><span data-stu-id="6ca47-139">Request</span></span>
<span data-ttu-id="6ca47-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ca47-140">The following is an example of a request.</span></span>

><span data-ttu-id="6ca47-141">**注意：** 为便于阅读将被截如下所示的请求对象。</span><span class="sxs-lookup"><span data-stu-id="6ca47-141">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="6ca47-142">提供实际呼叫中的所有属性。</span><span class="sxs-lookup"><span data-stu-id="6ca47-142">Supply all the properties in an actual call.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6ca47-143">响应</span><span class="sxs-lookup"><span data-stu-id="6ca47-143">Response</span></span>
<span data-ttu-id="6ca47-144">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="6ca47-144">The following is an example of a response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update synchronizationschema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
