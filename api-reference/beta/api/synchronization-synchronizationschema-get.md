---
title: 获取 synchronizationSchema
description: 检索给定的同步作业或模板的架构。
localization_priority: Normal
ms.openlocfilehash: 768a35940593231bbc4fbd4c3f5498c7eb3243fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863467"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="36ac0-103">获取 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="36ac0-103">Get synchronizationSchema</span></span>

> <span data-ttu-id="36ac0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="36ac0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36ac0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="36ac0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="36ac0-106">检索给定的同步作业或模板的架构。</span><span class="sxs-lookup"><span data-stu-id="36ac0-106">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="36ac0-107">权限</span><span class="sxs-lookup"><span data-stu-id="36ac0-107">Permissions</span></span>
<span data-ttu-id="36ac0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36ac0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36ac0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="36ac0-110">Permission type</span></span>                        | <span data-ttu-id="36ac0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36ac0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="36ac0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36ac0-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="36ac0-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36ac0-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="36ac0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36ac0-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="36ac0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="36ac0-115">Not supported.</span></span> |
|<span data-ttu-id="36ac0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="36ac0-116">Application</span></span>                            |<span data-ttu-id="36ac0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="36ac0-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="36ac0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36ac0-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="36ac0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="36ac0-119">Request headers</span></span>

| <span data-ttu-id="36ac0-120">名称</span><span class="sxs-lookup"><span data-stu-id="36ac0-120">Name</span></span>           | <span data-ttu-id="36ac0-121">类型</span><span class="sxs-lookup"><span data-stu-id="36ac0-121">Type</span></span>    | <span data-ttu-id="36ac0-122">说明</span><span class="sxs-lookup"><span data-stu-id="36ac0-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="36ac0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36ac0-123">Authorization</span></span>  | <span data-ttu-id="36ac0-124">string</span><span class="sxs-lookup"><span data-stu-id="36ac0-124">string</span></span>  | <span data-ttu-id="36ac0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36ac0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36ac0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="36ac0-127">Request body</span></span>

<span data-ttu-id="36ac0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36ac0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36ac0-129">响应</span><span class="sxs-lookup"><span data-stu-id="36ac0-129">Response</span></span>

<span data-ttu-id="36ac0-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[synchronizationSchema](../resources/synchronization-synchronizationschema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="36ac0-130">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36ac0-131">示例</span><span class="sxs-lookup"><span data-stu-id="36ac0-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="36ac0-132">请求</span><span class="sxs-lookup"><span data-stu-id="36ac0-132">Request</span></span>
<span data-ttu-id="36ac0-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36ac0-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="36ac0-134">响应</span><span class="sxs-lookup"><span data-stu-id="36ac0-134">Response</span></span>
<span data-ttu-id="36ac0-135">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="36ac0-135">The following is an example of a response.</span></span>

><span data-ttu-id="36ac0-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="36ac0-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="36ac0-137">将返回实际呼叫中的所有属性。</span><span class="sxs-lookup"><span data-stu-id="36ac0-137">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK

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
                }
            ]
        },
        {
            "name": "Salesforce",
            "objects": [{}]
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
                        {}
                    ]
                },
                {}
            ]
        },
        {}
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
