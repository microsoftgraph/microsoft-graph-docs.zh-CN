---
title: 获取 synchronizationSchema
description: 检索给定的同步作业或模板的架构。
localization_priority: Normal
ms.openlocfilehash: 050357c94997ca7a45d9ca09bf164638072d1354
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512491"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="92924-103">获取 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="92924-103">Get synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92924-104">检索给定的同步作业或模板的架构。</span><span class="sxs-lookup"><span data-stu-id="92924-104">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="92924-105">权限</span><span class="sxs-lookup"><span data-stu-id="92924-105">Permissions</span></span>
<span data-ttu-id="92924-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92924-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92924-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="92924-108">Permission type</span></span>                        | <span data-ttu-id="92924-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92924-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="92924-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92924-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="92924-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92924-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="92924-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92924-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="92924-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="92924-113">Not supported.</span></span> |
|<span data-ttu-id="92924-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="92924-114">Application</span></span>                            |<span data-ttu-id="92924-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="92924-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="92924-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92924-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="92924-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="92924-117">Request headers</span></span>

| <span data-ttu-id="92924-118">名称</span><span class="sxs-lookup"><span data-stu-id="92924-118">Name</span></span>           | <span data-ttu-id="92924-119">类型</span><span class="sxs-lookup"><span data-stu-id="92924-119">Type</span></span>    | <span data-ttu-id="92924-120">说明</span><span class="sxs-lookup"><span data-stu-id="92924-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="92924-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="92924-121">Authorization</span></span>  | <span data-ttu-id="92924-122">string</span><span class="sxs-lookup"><span data-stu-id="92924-122">string</span></span>  | <span data-ttu-id="92924-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="92924-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92924-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="92924-125">Request body</span></span>

<span data-ttu-id="92924-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="92924-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92924-127">响应</span><span class="sxs-lookup"><span data-stu-id="92924-127">Response</span></span>

<span data-ttu-id="92924-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[synchronizationSchema](../resources/synchronization-synchronizationschema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="92924-128">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92924-129">示例</span><span class="sxs-lookup"><span data-stu-id="92924-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="92924-130">请求</span><span class="sxs-lookup"><span data-stu-id="92924-130">Request</span></span>
<span data-ttu-id="92924-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92924-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="92924-132">响应</span><span class="sxs-lookup"><span data-stu-id="92924-132">Response</span></span>
<span data-ttu-id="92924-133">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="92924-133">The following is an example of a response.</span></span>

><span data-ttu-id="92924-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="92924-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="92924-135">将返回实际呼叫中的所有属性。</span><span class="sxs-lookup"><span data-stu-id="92924-135">All the properties will be returned in an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
