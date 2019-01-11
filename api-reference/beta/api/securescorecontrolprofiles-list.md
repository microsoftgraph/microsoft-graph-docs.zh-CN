---
title: 列出 secureScoreControlProfiles
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: cd13e4349119202f5f9e026973f3a90ee99f1019
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884551"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="73df1-104">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="73df1-104">List secureScoreControlProfiles</span></span>

 > <span data-ttu-id="73df1-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="73df1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73df1-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="73df1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73df1-107">检索的属性和[secureScoreControlProfiles](../resources/securescorecontrolprofiles.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="73df1-107">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="73df1-108">权限</span><span class="sxs-lookup"><span data-stu-id="73df1-108">Permissions</span></span>

<span data-ttu-id="73df1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73df1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73df1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="73df1-111">Permission type</span></span>      | <span data-ttu-id="73df1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73df1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73df1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73df1-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="73df1-114">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="73df1-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="73df1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73df1-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="73df1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="73df1-116">Not supported.</span></span>  |
|<span data-ttu-id="73df1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="73df1-117">Application</span></span> | <span data-ttu-id="73df1-118">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="73df1-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73df1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73df1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
```

## <a name="request-headers"></a><span data-ttu-id="73df1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="73df1-120">Request headers</span></span>

| <span data-ttu-id="73df1-121">名称</span><span class="sxs-lookup"><span data-stu-id="73df1-121">Name</span></span>      |<span data-ttu-id="73df1-122">说明</span><span class="sxs-lookup"><span data-stu-id="73df1-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="73df1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="73df1-123">Authorization</span></span>  | <span data-ttu-id="73df1-p104">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="73df1-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73df1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="73df1-126">Request body</span></span>

<span data-ttu-id="73df1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73df1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73df1-128">响应</span><span class="sxs-lookup"><span data-stu-id="73df1-128">Response</span></span>

<span data-ttu-id="73df1-129">如果成功，此方法返回`200 OK`响应代码和响应正文中的**secureScoreControlProfiles**对象。</span><span class="sxs-lookup"><span data-stu-id="73df1-129">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfiles** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73df1-130">示例</span><span class="sxs-lookup"><span data-stu-id="73df1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="73df1-131">请求</span><span class="sxs-lookup"><span data-stu-id="73df1-131">Request</span></span>

<span data-ttu-id="73df1-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="73df1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="73df1-133">响应</span><span class="sxs-lookup"><span data-stu-id="73df1-133">Response</span></span>

<span data-ttu-id="73df1-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="73df1-134">The following is an example of the response.</span></span>
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
