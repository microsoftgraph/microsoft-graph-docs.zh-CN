---
title: 列出 secureScoreControlProfiles
description: 检索 secureScoreControlProfiles 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: 94f94feb5f540d3a830b97ec3defe7972b345557
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638814"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="f41c9-103">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="f41c9-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f41c9-104">检索租户的[secureScoreControlProfile](../resources/securescorecontrolprofiles.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="f41c9-104">Retrieves a list of [secureScoreControlProfile](../resources/securescorecontrolprofiles.md) objects for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="f41c9-105">权限</span><span class="sxs-lookup"><span data-stu-id="f41c9-105">Permissions</span></span>

<span data-ttu-id="f41c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f41c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f41c9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f41c9-108">Permission type</span></span>      | <span data-ttu-id="f41c9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f41c9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f41c9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f41c9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f41c9-111">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="f41c9-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="f41c9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f41c9-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f41c9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f41c9-113">Not supported.</span></span>  |
|<span data-ttu-id="f41c9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f41c9-114">Application</span></span> | <span data-ttu-id="f41c9-115">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="f41c9-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f41c9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f41c9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="f41c9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f41c9-117">Request headers</span></span>

| <span data-ttu-id="f41c9-118">名称</span><span class="sxs-lookup"><span data-stu-id="f41c9-118">Name</span></span>      |<span data-ttu-id="f41c9-119">说明</span><span class="sxs-lookup"><span data-stu-id="f41c9-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f41c9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f41c9-120">Authorization</span></span>  | <span data-ttu-id="f41c9-121">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="f41c9-121">Bearer {code}.</span></span> <span data-ttu-id="f41c9-122">必需。</span><span class="sxs-lookup"><span data-stu-id="f41c9-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f41c9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f41c9-123">Request body</span></span>

<span data-ttu-id="f41c9-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f41c9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f41c9-125">响应</span><span class="sxs-lookup"><span data-stu-id="f41c9-125">Response</span></span>

<span data-ttu-id="f41c9-126">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScoreControlProfile**对象集合。</span><span class="sxs-lookup"><span data-stu-id="f41c9-126">If successful, this method returns a `200 OK` response code and a collection of **secureScoreControlProfile** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f41c9-127">示例</span><span class="sxs-lookup"><span data-stu-id="f41c9-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="f41c9-128">请求</span><span class="sxs-lookup"><span data-stu-id="f41c9-128">Request</span></span>

<span data-ttu-id="f41c9-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f41c9-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="f41c9-130">响应</span><span class="sxs-lookup"><span data-stu-id="f41c9-130">Response</span></span>

<span data-ttu-id="f41c9-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f41c9-131">The following is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f41c9-132">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f41c9-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f41c9-133">语言</span><span class="sxs-lookup"><span data-stu-id="f41c9-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/securescorecontrolprofiles_list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f41c9-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="f41c9-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/securescorecontrolprofiles_list-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
