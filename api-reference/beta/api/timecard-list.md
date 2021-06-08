---
title: 列出 timeCard
description: 检索计划中的 timeCard 条目列表。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1635e8c524b25b3795bf90f03449eddf259ff208
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787849"
---
# <a name="list-timecard"></a><span data-ttu-id="289a7-103">列出 timeCard</span><span class="sxs-lookup"><span data-stu-id="289a7-103">List timeCard</span></span>

<span data-ttu-id="289a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="289a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="289a7-105">检索计划 [中的 timeCard](../resources/timecard.md) 条目 [列表](../resources/schedule.md)。</span><span class="sxs-lookup"><span data-stu-id="289a7-105">Retrieve a list of [timeCard](../resources/timecard.md) entries in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="289a7-106">权限</span><span class="sxs-lookup"><span data-stu-id="289a7-106">Permissions</span></span>

<span data-ttu-id="289a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="289a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="289a7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="289a7-109">Permission type</span></span>      | <span data-ttu-id="289a7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="289a7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="289a7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="289a7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="289a7-112">Schedule.Read.All、Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="289a7-112">Schedule.Read.All, Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="289a7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="289a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="289a7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="289a7-114">Not supported.</span></span>    |
|<span data-ttu-id="289a7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="289a7-115">Application</span></span> | <span data-ttu-id="289a7-116">Schedule.Read.All *、Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="289a7-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="289a7-117">\***重要提示：** 使用应用程序权限时，必须在请求 `MS-APP-ACTS-AS` 中包括 标头。</span><span class="sxs-lookup"><span data-stu-id="289a7-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="289a7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="289a7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timecards
```

## <a name="optional-query-parameters"></a><span data-ttu-id="289a7-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="289a7-119">Optional query parameters</span></span>

<span data-ttu-id="289a7-120">此方法支持 `$filter` 、 `$orderBy` 、 、 OData 查询 `$top` `$skipToken` 参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="289a7-120">This method supports the `$filter`, `$orderBy`, `$top`, `$skipToken` OData query parameters to help customize the response.</span></span> <span data-ttu-id="289a7-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="289a7-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="289a7-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="289a7-122">Request headers</span></span>

| <span data-ttu-id="289a7-123">标头</span><span class="sxs-lookup"><span data-stu-id="289a7-123">Header</span></span>       | <span data-ttu-id="289a7-124">值</span><span class="sxs-lookup"><span data-stu-id="289a7-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="289a7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="289a7-125">Authorization</span></span>  | <span data-ttu-id="289a7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="289a7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="289a7-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="289a7-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="289a7-129">应用代表其操作的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="289a7-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="289a7-130">使用应用程序权限范围时是必需的。</span><span class="sxs-lookup"><span data-stu-id="289a7-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="289a7-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="289a7-131">Request body</span></span>
<span data-ttu-id="289a7-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="289a7-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="289a7-133">响应</span><span class="sxs-lookup"><span data-stu-id="289a7-133">Response</span></span>

<span data-ttu-id="289a7-134">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [timeCard](../resources/timeCard.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="289a7-134">If successful, this method returns a `200 OK` response code and a list of [timeCard](../resources/timeCard.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="289a7-135">示例</span><span class="sxs-lookup"><span data-stu-id="289a7-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="289a7-136">请求</span><span class="sxs-lookup"><span data-stu-id="289a7-136">Request</span></span>
<span data-ttu-id="289a7-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="289a7-137">The following is an example of the request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="289a7-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="289a7-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-list"
}-->

```http
GET https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards?$top=2&$filter=state eq 'clockedOut'

```

### <a name="response"></a><span data-ttu-id="289a7-139">响应</span><span class="sxs-lookup"><span data-stu-id="289a7-139">Response</span></span>

<span data-ttu-id="289a7-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="289a7-140">The following is an example of the response.</span></span> 

><span data-ttu-id="289a7-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="289a7-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "@odata.etag": "\"3400c313-0000-0d00-0000-60afe1940000\"",
            "id": "TCK_d1e0f245-9996-4125-b128-d3eb5c4b0164",
            "createdDateTime": "2020-09-21T18:01:29.302Z",
            "lastModifiedDateTime": "2021-05-27T18:14:44.503Z",
            "userId": "66b4f2a4-425d-4dec-8172-7e889950885e",
            "state": "clockedOut",
            "confirmedBy": "none",
            "notes": null,
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
                    "displayName": "Jing Jing GuTwo"
                }
            },
            "clockInEvent": {
                "dateTime": "2020-09-21T18:01:29.302Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "ClockIn-OBO Shorbani"
                }
            },
            "clockOutEvent": {
                "dateTime": "2021-05-27T18:14:44.503Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "clock out notes"
                }
            },
            "breaks": [],
            "originalEntry": {
                "clockInEvent": {
                    "dateTime": "2020-09-21T18:01:29.302Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "ClockIn-OBO Shorbani"
                    }
                },
                "clockOutEvent": {
                    "dateTime": "2021-05-27T18:14:44.503Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "clock out notes"
                    }
                },
                "breaks": []
            },
            "createdBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "66b4f2a4-425d-4dec-8172-7e889950885e",
                    "displayName": "Janani Varadharajan"
                }
            }
        },
        {
            "@odata.etag": "\"3400d914-0000-0d00-0000-60afe1ee0000\"",
            "id": "TCK_aa73c610-dd75-4021-bb5c-6b071c7aa835",
            "createdDateTime": "2020-09-21T18:02:48.688Z",
            "lastModifiedDateTime": "2021-05-27T18:16:14.766Z",
            "userId": "3041ccde-7544-4ae0-b44f-3618b08ba1ce",
            "state": "clockedOut",
            "confirmedBy": "none",
            "notes": null,
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
                    "displayName": "Jing Jing GuTwo"
                }
            },
            "clockInEvent": {
                "dateTime": "2020-09-21T18:02:48.688Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "ClockIn-OBO Shorbani"
                }
            },
            "clockOutEvent": {
                "dateTime": "2021-05-27T18:16:14.766Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "clock out notes"
                }
            },
            "breaks": [],
            "originalEntry": {
                "clockInEvent": {
                    "dateTime": "2020-09-21T18:02:48.688Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "ClockIn-OBO Shorbani"
                    }
                },
                "clockOutEvent": {
                    "dateTime": "2021-05-27T18:16:14.766Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "clock out notes"
                    }
                },
                "breaks": []
            },
            "createdBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "66b4f2a4-425d-4dec-8172-7e889950885e",
                    "displayName": "Janani Varadharajan"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Retrieve a list of timeCard entries in the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
