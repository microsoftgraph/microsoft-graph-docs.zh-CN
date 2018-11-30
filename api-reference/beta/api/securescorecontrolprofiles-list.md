---
title: 列表 secureScoreControlProfiles
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: 33d0f6059d66350c9fa763097277f83c041e96ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044666"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="6092e-104">列表 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="6092e-104">List secureScoreControlProfiles</span></span>

 > <span data-ttu-id="6092e-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6092e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6092e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6092e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6092e-107">检索的属性和[secureScoreControlProfiles](../resources/securescorecontrolprofiles.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="6092e-107">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6092e-108">权限</span><span class="sxs-lookup"><span data-stu-id="6092e-108">Permissions</span></span>

<span data-ttu-id="6092e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6092e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6092e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6092e-111">Permission type</span></span>      | <span data-ttu-id="6092e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6092e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6092e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6092e-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="6092e-114">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="6092e-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="6092e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6092e-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6092e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6092e-116">Not supported.</span></span>  |
|<span data-ttu-id="6092e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6092e-117">Application</span></span> | <span data-ttu-id="6092e-118">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="6092e-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6092e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6092e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="6092e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6092e-120">Request headers</span></span>

| <span data-ttu-id="6092e-121">名称</span><span class="sxs-lookup"><span data-stu-id="6092e-121">Name</span></span>      |<span data-ttu-id="6092e-122">说明</span><span class="sxs-lookup"><span data-stu-id="6092e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6092e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6092e-123">Authorization</span></span>  | <span data-ttu-id="6092e-p104">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="6092e-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6092e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6092e-126">Request body</span></span>

<span data-ttu-id="6092e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6092e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6092e-128">响应</span><span class="sxs-lookup"><span data-stu-id="6092e-128">Response</span></span>

<span data-ttu-id="6092e-129">如果成功，此方法返回`200 OK`响应代码和响应正文中的**secureScoreControlProfiles**对象。</span><span class="sxs-lookup"><span data-stu-id="6092e-129">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfiles** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6092e-130">示例</span><span class="sxs-lookup"><span data-stu-id="6092e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6092e-131">请求</span><span class="sxs-lookup"><span data-stu-id="6092e-131">Request</span></span>

<span data-ttu-id="6092e-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6092e-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="6092e-133">响应</span><span class="sxs-lookup"><span data-stu-id="6092e-133">Response</span></span>

<span data-ttu-id="6092e-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6092e-134">The following is an example of the response.</span></span>
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


<!-- {
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
