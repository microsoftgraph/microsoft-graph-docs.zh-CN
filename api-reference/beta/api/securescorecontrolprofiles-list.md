---
title: 列出 secureScoreControlProfiles
description: 检索 secureScoreControlProfiles 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5df74d2d9d90839e2caa83039fa82a6eeb71b2ab
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410435"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="d004a-103">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="d004a-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d004a-104">检索租户的[secureScoreControlProfile](../resources/securescorecontrolprofiles.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d004a-104">Retrieves a list of [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) objects for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="d004a-105">权限</span><span class="sxs-lookup"><span data-stu-id="d004a-105">Permissions</span></span>

<span data-ttu-id="d004a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d004a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d004a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d004a-108">Permission type</span></span>      | <span data-ttu-id="d004a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d004a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d004a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d004a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d004a-111">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="d004a-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="d004a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d004a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d004a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d004a-113">Not supported.</span></span>  |
|<span data-ttu-id="d004a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d004a-114">Application</span></span> | <span data-ttu-id="d004a-115">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="d004a-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d004a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d004a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="d004a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d004a-117">Request headers</span></span>

| <span data-ttu-id="d004a-118">名称</span><span class="sxs-lookup"><span data-stu-id="d004a-118">Name</span></span>      |<span data-ttu-id="d004a-119">说明</span><span class="sxs-lookup"><span data-stu-id="d004a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d004a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d004a-120">Authorization</span></span>  | <span data-ttu-id="d004a-121">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="d004a-121">Bearer {code}.</span></span> <span data-ttu-id="d004a-122">必需。</span><span class="sxs-lookup"><span data-stu-id="d004a-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d004a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d004a-123">Request body</span></span>

<span data-ttu-id="d004a-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d004a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d004a-125">响应</span><span class="sxs-lookup"><span data-stu-id="d004a-125">Response</span></span>

<span data-ttu-id="d004a-126">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScoreControlProfile**对象集合。</span><span class="sxs-lookup"><span data-stu-id="d004a-126">If successful, this method returns a `200 OK` response code and a collection of **secureScoreControlProfile** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d004a-127">示例</span><span class="sxs-lookup"><span data-stu-id="d004a-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="d004a-128">请求</span><span class="sxs-lookup"><span data-stu-id="d004a-128">Request</span></span>

<span data-ttu-id="d004a-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d004a-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d004a-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d004a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d004a-131">C#</span><span class="sxs-lookup"><span data-stu-id="d004a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d004a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d004a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d004a-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="d004a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d004a-134">响应</span><span class="sxs-lookup"><span data-stu-id="d004a-134">Response</span></span>

<span data-ttu-id="d004a-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d004a-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "value": [
        {
            "actionType": "actionType.value",
            "actionUrl": "actionUrl.value",
            "controlCategory": "controlCategory.value",
            "title": "title.value",
            "deprecated": true,
            "implementationCost": "implementationCost.value",
            "lastModifiedDateTime": "lastModifiedDateTime.value",
            "maxScore": 1020.13,
            "rank": 100,
            "remediation": "remediation.value",
            "remediationImpact": "remediationImpact.value",
            "service": "service.value",
            "threats": [
                "threats.value"
            ],
            "tier": "tier.value",
            "userImpact": "userImpact.value",
            "id": "id.value",
            "azureTenantId": "azureTenantId.value",
            "controlStateUpdates": [
                {
                    "assignedTo": "assignedTo.value",
                    "comment": "comment.value",
                    "state": "state.value",
                    "updatedBy": "updatedBy.value",
                    "updatedDateTime": "updatedDateTime.value"
                }
            ],
            "vendorInformation": {
                "provider": "SecureScore",
                "providerVersion": null,
                "subProvider": null,
                "vendor": "Microsoft"
            }
         }
     ]
}
```


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
