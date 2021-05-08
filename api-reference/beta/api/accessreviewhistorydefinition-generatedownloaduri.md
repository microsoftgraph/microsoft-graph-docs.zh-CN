---
title: accessReviewHistoryDefinition： generateDownloadUri
description: 生成可用于检索审阅历史记录数据的 URI。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e45af13a74c31c09dd3733a5a2c0fbec9645b2cf
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232906"
---
# <a name="accessreviewhistorydefinition-generatedownloaduri"></a><span data-ttu-id="6a32c-103">accessReviewHistoryDefinition： generateDownloadUri</span><span class="sxs-lookup"><span data-stu-id="6a32c-103">accessReviewHistoryDefinition: generateDownloadUri</span></span>

<span data-ttu-id="6a32c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a32c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a32c-105">生成可用于检索关联 [accessReviewHistoryDefinition](../resources/accessReviewHistoryDefinition.md)的审阅历史记录数据的 URI。</span><span class="sxs-lookup"><span data-stu-id="6a32c-105">Generate a URI that can be used to retrieve review history data for the associated [accessReviewHistoryDefinition](../resources/accessReviewHistoryDefinition.md).</span></span> <span data-ttu-id="6a32c-106">此 URI 的有效期为一天，可通过从关联的 [accessReviewHistoryDefinition](../resources/accessReviewHistoryDefinition.md)对象提取 **downloadUri** 属性来检索。</span><span class="sxs-lookup"><span data-stu-id="6a32c-106">This URI is valid for one day and can be retrieved by fetching the **downloadUri** property from the associated [accessReviewHistoryDefinition](../resources/accessReviewHistoryDefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a32c-107">权限</span><span class="sxs-lookup"><span data-stu-id="6a32c-107">Permissions</span></span>

<span data-ttu-id="6a32c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a32c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a32c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a32c-110">Permission type</span></span>|<span data-ttu-id="6a32c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a32c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a32c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a32c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a32c-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a32c-113">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="6a32c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a32c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a32c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a32c-115">Not supported.</span></span>|
|<span data-ttu-id="6a32c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a32c-116">Application</span></span>|<span data-ttu-id="6a32c-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a32c-117">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="6a32c-118">登录用户还必须是关联的审阅历史记录定义的创建者、全局管理员目录角色成员或全局读取者目录角色成员才能生成链接。</span><span class="sxs-lookup"><span data-stu-id="6a32c-118">The signed-in user must also be the creator of the associated review history definition, a Global Admin directory role member, or a Global Reader directory role member to generate the link.</span></span>

## <a name="http-request"></a><span data-ttu-id="6a32c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a32c-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/historyDefinitions/{definition-id}/generateDownloadUri()
```

## <a name="request-headers"></a><span data-ttu-id="6a32c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a32c-120">Request headers</span></span>
|<span data-ttu-id="6a32c-121">名称</span><span class="sxs-lookup"><span data-stu-id="6a32c-121">Name</span></span>|<span data-ttu-id="6a32c-122">说明</span><span class="sxs-lookup"><span data-stu-id="6a32c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6a32c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a32c-123">Authorization</span></span>|<span data-ttu-id="6a32c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6a32c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a32c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a32c-126">Request body</span></span>
<span data-ttu-id="6a32c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6a32c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a32c-128">响应</span><span class="sxs-lookup"><span data-stu-id="6a32c-128">Response</span></span>

<span data-ttu-id="6a32c-129">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [accessReviewHistoryDefinition。](../resources/accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6a32c-129">If successful, this action returns a `200 OK` response code and an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a32c-130">示例</span><span class="sxs-lookup"><span data-stu-id="6a32c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a32c-131">请求</span><span class="sxs-lookup"><span data-stu-id="6a32c-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewhistorydefinition_generatedownloaduri"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions/b2cb022f-b7e1-40f3-9854-c65a40861c38/generateDownloadUri
```


### <a name="response"></a><span data-ttu-id="6a32c-132">响应</span><span class="sxs-lookup"><span data-stu-id="6a32c-132">Response</span></span>
><span data-ttu-id="6a32c-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6a32c-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
  "displayName": "Last quarter's group reviews April 2021",
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "status": "done",
  "createdDateTime": "2021-04-14T00:22:48.9392594Z",
  "fulfilledDateTime": "2021-04-14T00:22:58.5276552Z",
  "downloadUri": "https://contoso.com/df-erm-reports/Last quarter's group reviews April 2021-22be232e-a93d-42a3-8ac5-313cfd29a0eb.csv?sv=2015-04-05&ss=b&srt=o&sp=rl&st=2021-04-15T00:22:58.5276552Z&se=2021-03-23T19:41:38.0000000Z&spr=https&sig=84rlGCIgU4ToMn%2FFLncBXq95O8a8RsFlwQY1Knl%2Fo%2FI%3D",
  "createdBy": {
      "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
      "displayName": "MOD Administrator",
      "userPrincipalName": "admin@contoso.com"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```
