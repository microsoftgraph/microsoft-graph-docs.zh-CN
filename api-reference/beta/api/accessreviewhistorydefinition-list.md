---
title: 列出 accessReviewHistoryDefinitions
description: 获取 accessReviewHistoryDefinition 对象的列表。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0977ab297ec7b5d828ff11cf5090d8427bd3d695
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232907"
---
# <a name="list-accessreviewhistorydefinitions"></a><span data-ttu-id="f08e5-103">列出 accessReviewHistoryDefinitions</span><span class="sxs-lookup"><span data-stu-id="f08e5-103">List accessReviewHistoryDefinitions</span></span>
<span data-ttu-id="f08e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f08e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f08e5-105">检索最近 30 天内创建的 [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象，包括所有嵌套属性。</span><span class="sxs-lookup"><span data-stu-id="f08e5-105">Retrieve the [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) objects created in the last 30 days, including all nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="f08e5-106">此 API 的默认页面大小为 100 **accessReviewHistoryDefinitions** 对象。</span><span class="sxs-lookup"><span data-stu-id="f08e5-106">The default page size for this API is 100 **accessReviewHistoryDefinitions** objects.</span></span> <span data-ttu-id="f08e5-107">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="f08e5-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="f08e5-108">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="f08e5-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
>
><span data-ttu-id="f08e5-109">如果未提供查询参数且结果超过 100 个，Microsoft Graph将按每页 100 个结果自动对结果分页。</span><span class="sxs-lookup"><span data-stu-id="f08e5-109">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="f08e5-110">权限</span><span class="sxs-lookup"><span data-stu-id="f08e5-110">Permissions</span></span>

<span data-ttu-id="f08e5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f08e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f08e5-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="f08e5-113">Permission type</span></span>|<span data-ttu-id="f08e5-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f08e5-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f08e5-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f08e5-115">Delegated (work or school account)</span></span>|<span data-ttu-id="f08e5-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f08e5-116">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="f08e5-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f08e5-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f08e5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f08e5-118">Not supported.</span></span>|
|<span data-ttu-id="f08e5-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="f08e5-119">Application</span></span>|<span data-ttu-id="f08e5-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f08e5-120">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="f08e5-121">如果登录用户不是全局管理员目录角色成员或全局读者目录角色成员，则仅返回已登录用户创建的定义。</span><span class="sxs-lookup"><span data-stu-id="f08e5-121">If the signed-in user is not a Global Admin directory role member or a Global Reader directory role member, only the definitions that the signed-in user created will be returned.</span></span>

## <a name="http-request"></a><span data-ttu-id="f08e5-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f08e5-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/historyDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f08e5-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f08e5-123">Optional query parameters</span></span>
<span data-ttu-id="f08e5-124">此方法支持使用 `$top` 、 `$filter` 和 `$skip` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f08e5-124">This method supports the `$top`, `$filter`, and `$skip` OData query parameters to help customize the response.</span></span> <span data-ttu-id="f08e5-125">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f08e5-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span> 

## <a name="request-headers"></a><span data-ttu-id="f08e5-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="f08e5-126">Request headers</span></span>
|<span data-ttu-id="f08e5-127">名称</span><span class="sxs-lookup"><span data-stu-id="f08e5-127">Name</span></span>|<span data-ttu-id="f08e5-128">说明</span><span class="sxs-lookup"><span data-stu-id="f08e5-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f08e5-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="f08e5-129">Authorization</span></span>|<span data-ttu-id="f08e5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f08e5-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f08e5-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="f08e5-132">Request body</span></span>
<span data-ttu-id="f08e5-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f08e5-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f08e5-134">响应</span><span class="sxs-lookup"><span data-stu-id="f08e5-134">Response</span></span>

<span data-ttu-id="f08e5-135">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f08e5-135">If successful, this method returns a `200 OK` response code and a collection of [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f08e5-136">示例</span><span class="sxs-lookup"><span data-stu-id="f08e5-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f08e5-137">请求</span><span class="sxs-lookup"><span data-stu-id="f08e5-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_accessreviewhistorydefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions
```


### <a name="response"></a><span data-ttu-id="f08e5-138">响应</span><span class="sxs-lookup"><span data-stu-id="f08e5-138">Response</span></span>
><span data-ttu-id="f08e5-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f08e5-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition",
  "isCollection": "true"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.count": 1,
  "value": [
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
  ]
}
```
