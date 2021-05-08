---
title: 获取 accessReviewHistoryDefinition
description: 检索 accessReviewHistoryDefinition 对象。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d5a512124bdd6496e2c86f03a39a5a2bd706b7e6
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232905"
---
# <a name="get-accessreviewhistorydefinition"></a><span data-ttu-id="5fc0f-103">获取 accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="5fc0f-103">Get accessReviewHistoryDefinition</span></span>

<span data-ttu-id="5fc0f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fc0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fc0f-105">按其 [标识符检索 accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5fc0f-105">Retrieve an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object by its identifier.</span></span> <span data-ttu-id="5fc0f-106">返回访问评审历史记录定义对象的所有属性。</span><span class="sxs-lookup"><span data-stu-id="5fc0f-106">All of the properties of the access review history definition object are returned.</span></span> <span data-ttu-id="5fc0f-107">如果下载链接仍然有效，它将与定义一起返回。</span><span class="sxs-lookup"><span data-stu-id="5fc0f-107">If the download link is still valid, it is returned along with the definition.</span></span> <span data-ttu-id="5fc0f-108">如果定义是 30 天或更久，则返回 404 错误。</span><span class="sxs-lookup"><span data-stu-id="5fc0f-108">If the definition is 30 days or older, a 404 error is returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="5fc0f-109">权限</span><span class="sxs-lookup"><span data-stu-id="5fc0f-109">Permissions</span></span>

<span data-ttu-id="5fc0f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5fc0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fc0f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5fc0f-112">Permission type</span></span>|<span data-ttu-id="5fc0f-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5fc0f-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fc0f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5fc0f-114">Delegated (work or school account)</span></span>|<span data-ttu-id="5fc0f-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fc0f-115">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="5fc0f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5fc0f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fc0f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fc0f-117">Not supported.</span></span>|
|<span data-ttu-id="5fc0f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5fc0f-118">Application</span></span>|<span data-ttu-id="5fc0f-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fc0f-119">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="5fc0f-120">登录用户还必须是关联的审阅历史记录定义的创建者、全局管理员目录角色成员或全局读取者目录角色成员才能检索定义。</span><span class="sxs-lookup"><span data-stu-id="5fc0f-120">The signed-in user must also be the creator of the associated review history definition, a Global Admin directory role member, or a Global Reader directory role member to retrieve the definition.</span></span>

## <a name="http-request"></a><span data-ttu-id="5fc0f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5fc0f-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/historyDefinitions/{definition-id}
```

## <a name="request-headers"></a><span data-ttu-id="5fc0f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5fc0f-122">Request headers</span></span>
|<span data-ttu-id="5fc0f-123">名称</span><span class="sxs-lookup"><span data-stu-id="5fc0f-123">Name</span></span>|<span data-ttu-id="5fc0f-124">说明</span><span class="sxs-lookup"><span data-stu-id="5fc0f-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5fc0f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fc0f-125">Authorization</span></span>|<span data-ttu-id="5fc0f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5fc0f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fc0f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5fc0f-128">Request body</span></span>
<span data-ttu-id="5fc0f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5fc0f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fc0f-130">响应</span><span class="sxs-lookup"><span data-stu-id="5fc0f-130">Response</span></span>

<span data-ttu-id="5fc0f-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5fc0f-131">If successful, this method returns a `200 OK` response code and an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5fc0f-132">示例</span><span class="sxs-lookup"><span data-stu-id="5fc0f-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5fc0f-133">请求</span><span class="sxs-lookup"><span data-stu-id="5fc0f-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accessreviewhistorydefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions/b2cb022f-b7e1-40f3-9854-c65a40861c38
```


### <a name="response"></a><span data-ttu-id="5fc0f-134">响应</span><span class="sxs-lookup"><span data-stu-id="5fc0f-134">Response</span></span>
><span data-ttu-id="5fc0f-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5fc0f-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
