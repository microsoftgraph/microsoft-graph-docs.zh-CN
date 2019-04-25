---
title: 列出 secureScoreControlProfiles
description: 检索 secureScoreControlProfiles 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: 6627111633f54eb7bc2584af826b69fd5bd6cf49
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545593"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="178fa-103">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="178fa-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="178fa-104">检索[secureScoreControlProfiles](../resources/securescorecontrolprofiles.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="178fa-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="178fa-105">权限</span><span class="sxs-lookup"><span data-stu-id="178fa-105">Permissions</span></span>

<span data-ttu-id="178fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="178fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="178fa-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="178fa-108">Permission type</span></span>      | <span data-ttu-id="178fa-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="178fa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="178fa-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="178fa-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="178fa-111">securityevents.readwrite.all、securityevents.readwrite.all、all。</span><span class="sxs-lookup"><span data-stu-id="178fa-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="178fa-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="178fa-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="178fa-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="178fa-113">Not supported.</span></span>  |
|<span data-ttu-id="178fa-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="178fa-114">Application</span></span> | <span data-ttu-id="178fa-115">securityevents.readwrite.all、securityevents.readwrite.all、all。</span><span class="sxs-lookup"><span data-stu-id="178fa-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="178fa-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="178fa-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="178fa-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="178fa-117">Request headers</span></span>

| <span data-ttu-id="178fa-118">名称</span><span class="sxs-lookup"><span data-stu-id="178fa-118">Name</span></span>      |<span data-ttu-id="178fa-119">说明</span><span class="sxs-lookup"><span data-stu-id="178fa-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="178fa-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="178fa-120">Authorization</span></span>  | <span data-ttu-id="178fa-121">持有者 {代码}。</span><span class="sxs-lookup"><span data-stu-id="178fa-121">Bearer {code}.</span></span> <span data-ttu-id="178fa-122">必需。</span><span class="sxs-lookup"><span data-stu-id="178fa-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="178fa-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="178fa-123">Request body</span></span>

<span data-ttu-id="178fa-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="178fa-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="178fa-125">响应</span><span class="sxs-lookup"><span data-stu-id="178fa-125">Response</span></span>

<span data-ttu-id="178fa-126">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScoreControlProfiles**对象。</span><span class="sxs-lookup"><span data-stu-id="178fa-126">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfiles** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="178fa-127">示例</span><span class="sxs-lookup"><span data-stu-id="178fa-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="178fa-128">请求</span><span class="sxs-lookup"><span data-stu-id="178fa-128">Request</span></span>

<span data-ttu-id="178fa-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="178fa-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="178fa-130">响应</span><span class="sxs-lookup"><span data-stu-id="178fa-130">Response</span></span>

<span data-ttu-id="178fa-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="178fa-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
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
            "deprecated": "deprecated.value",
            "implementationCost": "implementationCost.value",
            "lastModifiedDateTime": "lastModifiedDateTime.value",
            "maxScore": "maxScore.value",
            "rank": "rank.value",
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
    "Error: /api-reference/beta/api/securescorecontrolprofiles-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
