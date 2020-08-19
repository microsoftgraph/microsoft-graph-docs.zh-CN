---
title: 列出 secureScoreControlProfiles
description: 检索 secureScoreControlProfiles 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: b66f17fb7752ab129f2e1f78e25df590b5a9e79e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812568"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="1f73b-103">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="1f73b-103">List secureScoreControlProfiles</span></span>

<span data-ttu-id="1f73b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f73b-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f73b-105">检索租户的 [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="1f73b-105">Retrieves a list of [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) objects for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f73b-106">权限</span><span class="sxs-lookup"><span data-stu-id="1f73b-106">Permissions</span></span>

<span data-ttu-id="1f73b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f73b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f73b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f73b-109">Permission type</span></span>      | <span data-ttu-id="1f73b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f73b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f73b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f73b-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="1f73b-112">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="1f73b-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="1f73b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f73b-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1f73b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f73b-114">Not supported.</span></span>  |
|<span data-ttu-id="1f73b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f73b-115">Application</span></span> | <span data-ttu-id="1f73b-116">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="1f73b-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f73b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f73b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="1f73b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f73b-118">Request headers</span></span>

| <span data-ttu-id="1f73b-119">名称</span><span class="sxs-lookup"><span data-stu-id="1f73b-119">Name</span></span>      |<span data-ttu-id="1f73b-120">说明</span><span class="sxs-lookup"><span data-stu-id="1f73b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1f73b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f73b-121">Authorization</span></span>  | <span data-ttu-id="1f73b-122">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="1f73b-122">Bearer {code}.</span></span> <span data-ttu-id="1f73b-123">必需。</span><span class="sxs-lookup"><span data-stu-id="1f73b-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f73b-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f73b-124">Request body</span></span>

<span data-ttu-id="1f73b-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1f73b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f73b-126">响应</span><span class="sxs-lookup"><span data-stu-id="1f73b-126">Response</span></span>

<span data-ttu-id="1f73b-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 **secureScoreControlProfile** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1f73b-127">If successful, this method returns a `200 OK` response code and a collection of **secureScoreControlProfile** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f73b-128">示例</span><span class="sxs-lookup"><span data-stu-id="1f73b-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f73b-129">请求</span><span class="sxs-lookup"><span data-stu-id="1f73b-129">Request</span></span>

<span data-ttu-id="1f73b-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1f73b-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f73b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f73b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```
# <a name="c"></a>[<span data-ttu-id="1f73b-132">C#</span><span class="sxs-lookup"><span data-stu-id="1f73b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f73b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f73b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f73b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f73b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f73b-135">响应</span><span class="sxs-lookup"><span data-stu-id="1f73b-135">Response</span></span>

<span data-ttu-id="1f73b-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1f73b-136">The following is an example of the response.</span></span>
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
