---
title: 创建 timeCard
description: 在计划内创建 timeCard 实例。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e1a03dd2139070fa06156689bf332d0e7c1a3dcb
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870092"
---
# <a name="create-timecard"></a><span data-ttu-id="64bd2-103">创建 timeCard</span><span class="sxs-lookup"><span data-stu-id="64bd2-103">Create timeCard</span></span>

<span data-ttu-id="64bd2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64bd2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64bd2-105">在 [计划 创建 timeCard](../resources/timeCard.md) [实例](../resources/schedule.md)。</span><span class="sxs-lookup"><span data-stu-id="64bd2-105">Create a [timeCard](../resources/timeCard.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="64bd2-106">权限</span><span class="sxs-lookup"><span data-stu-id="64bd2-106">Permissions</span></span>

<span data-ttu-id="64bd2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64bd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64bd2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="64bd2-109">Permission type</span></span>      | <span data-ttu-id="64bd2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64bd2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64bd2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64bd2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="64bd2-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64bd2-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="64bd2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64bd2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64bd2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="64bd2-114">Not supported.</span></span>    |
|<span data-ttu-id="64bd2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="64bd2-115">Application</span></span> | <span data-ttu-id="64bd2-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="64bd2-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="64bd2-117">\***重要提示：** 使用应用程序权限时，必须在请求 `MS-APP-ACTS-AS` 中包括 标头。</span><span class="sxs-lookup"><span data-stu-id="64bd2-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="64bd2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64bd2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards
```

## <a name="request-headers"></a><span data-ttu-id="64bd2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="64bd2-119">Request headers</span></span>

| <span data-ttu-id="64bd2-120">标头</span><span class="sxs-lookup"><span data-stu-id="64bd2-120">Header</span></span>       | <span data-ttu-id="64bd2-121">值</span><span class="sxs-lookup"><span data-stu-id="64bd2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64bd2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="64bd2-122">Authorization</span></span>  | <span data-ttu-id="64bd2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64bd2-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="64bd2-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="64bd2-125">Content-type</span></span> | <span data-ttu-id="64bd2-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="64bd2-p103">application/json. Required.</span></span>|
| <span data-ttu-id="64bd2-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="64bd2-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="64bd2-129">应用代表其操作的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="64bd2-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="64bd2-130">使用应用程序权限范围时是必需的。</span><span class="sxs-lookup"><span data-stu-id="64bd2-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64bd2-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="64bd2-131">Request body</span></span>

<span data-ttu-id="64bd2-132">在此方法的请求正文中提供新的 [timeCard](../resources/timecard.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64bd2-132">Provide the new [timeCard](../resources/timecard.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64bd2-133">响应</span><span class="sxs-lookup"><span data-stu-id="64bd2-133">Response</span></span>

<span data-ttu-id="64bd2-134">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [timeCard](../resources/timeCard.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64bd2-134">If successful, this method returns a `201 Created` response code and a [timeCard](../resources/timeCard.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64bd2-135">示例</span><span class="sxs-lookup"><span data-stu-id="64bd2-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="64bd2-136">请求</span><span class="sxs-lookup"><span data-stu-id="64bd2-136">Request</span></span>
<span data-ttu-id="64bd2-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="64bd2-137">The following is an example of the request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="64bd2-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="64bd2-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-post"
}-->

```http
POST https://graph.microsoft.com/beta/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule/timecards
Content-type: application/json

{
  "onBehalfOfUserId":"a3601044-a1b5-438e-b742-f78d01d68a67",
  "clockInEvent":{
     "dateTime":"2019-03-18T00:00:00.000Z",
     "atApprovedLocation":true,
     "notes": {
        "content": "Started late due to traffic in CA 237",
        "contentType": "text"
     },
  },
  "notes":{
        "content": "8 To 5 Inventory management",
        "contentType": "text"
   },
  "breaks":[
     {
       "breakId": "string",
        "notes":{
             "content": "Lunch break",
             "contentType": "text"
        },
        "start":{
           "dateTime":"2019-03-18T02:00:00.000Z",
           "atApprovedLocation":true,
           "notes": {
                "content": "Reduced break to make up for lost time",
                "contentType": "text"
             },
        }
     }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="64bd2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64bd2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64bd2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64bd2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="64bd2-141">响应</span><span class="sxs-lookup"><span data-stu-id="64bd2-141">Response</span></span>

<span data-ttu-id="64bd2-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="64bd2-142">The following is an example of the response.</span></span> 

><span data-ttu-id="64bd2-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="64bd2-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "id":"3895809b-a618-4c0d-86a0-d42b25b7d74f",
   "userId":"a3601044-a1b5-438e-b742-f78d01d68a67",
   "createdDateTime":"2019-03-18T00:00:00.000Z",
   "createdBy":{
      "user":{
         "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
         "displayName":"Dwight Schrute"
      }
   },
   "lastModifiedDateTime":"2019-03-18T00:00:00.000Z",
   "lastModifiedBy":{
      "user":{
         "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
         "displayName":"Dwight Schrute"
      }
   },
   "state":"onBreak",
   "confirmationStatus":"notConfirmed",
   "originalEntry":{
      "clockInEvent":{
         "dateTime":"2019-03-18T00:00:00.000Z",
         "atApprovedLocation":true,
         "notes": {
            "content": "Started late due to traffic in CA 237",
           "contentType": "text"
         },
      },
      "clockOutEvent":null,
      "breaks":[
         {
            "breakId":"string",
            "notes":{
                "content": "Lunch break",
                "contentType": "text"
             },
            "start":{
               "dateTime":"2019-03-18T02:00:00.000Z",
               "atApprovedLocation":true,
               "notes": {
                  "content": "Reduced break to make up for lost time",
                  "contentType": "text"
               },
            },
            "end":null
         }
      ]
   },
   "clockInEvent":{
      "dateTime":"2019-03-18T00:00:00.000Z",
      "atApprovedLocation":true,
      "notes": {
        "content": "Started late due to traffic in CA 237",
        "contentType": "text"
     },
   },
   "clockOutEvent":null,
   "notes":{
        "content": "8 To 5 Inventory management",
        "contentType": "text"
   },
   "breaks":[
      {
         "breakId":"string",
         "notes":{
             "content": "Lunch break",
             "contentType": "text"
         },
         "start":{
            "dateTime":"2019-03-18T02:00:00.000Z",
            "atApprovedLocation":true,
            "notes": {
                "content": "Reduced break to make up for lost time",
                "contentType": "text"
             },
         },
         "end":null
      }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
