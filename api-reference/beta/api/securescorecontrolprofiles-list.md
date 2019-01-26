---
title: 列出 secureScoreControlProfiles
description: 检索的属性和 secureScoreControlProfiles 对象的关系。
localization_priority: Normal
ms.openlocfilehash: 6177af7da65d268af7c089aee3772109fb182959
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571091"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="3271f-103">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="3271f-103">List secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3271f-104">检索的属性和[secureScoreControlProfiles](../resources/securescorecontrolprofiles.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="3271f-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3271f-105">权限</span><span class="sxs-lookup"><span data-stu-id="3271f-105">Permissions</span></span>

<span data-ttu-id="3271f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3271f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3271f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3271f-108">Permission type</span></span>      | <span data-ttu-id="3271f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3271f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3271f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3271f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3271f-111">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="3271f-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="3271f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3271f-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3271f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3271f-113">Not supported.</span></span>  |
|<span data-ttu-id="3271f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3271f-114">Application</span></span> | <span data-ttu-id="3271f-115">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="3271f-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3271f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3271f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="3271f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3271f-117">Request headers</span></span>

| <span data-ttu-id="3271f-118">名称</span><span class="sxs-lookup"><span data-stu-id="3271f-118">Name</span></span>      |<span data-ttu-id="3271f-119">说明</span><span class="sxs-lookup"><span data-stu-id="3271f-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3271f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3271f-120">Authorization</span></span>  | <span data-ttu-id="3271f-p102">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="3271f-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3271f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3271f-123">Request body</span></span>

<span data-ttu-id="3271f-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3271f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3271f-125">响应</span><span class="sxs-lookup"><span data-stu-id="3271f-125">Response</span></span>

<span data-ttu-id="3271f-126">如果成功，此方法返回`200 OK`响应代码和响应正文中的**secureScoreControlProfiles**对象。</span><span class="sxs-lookup"><span data-stu-id="3271f-126">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfiles** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3271f-127">示例</span><span class="sxs-lookup"><span data-stu-id="3271f-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="3271f-128">请求</span><span class="sxs-lookup"><span data-stu-id="3271f-128">Request</span></span>

<span data-ttu-id="3271f-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3271f-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="3271f-130">响应</span><span class="sxs-lookup"><span data-stu-id="3271f-130">Response</span></span>

<span data-ttu-id="3271f-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3271f-131">The following is an example of the response.</span></span>
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
