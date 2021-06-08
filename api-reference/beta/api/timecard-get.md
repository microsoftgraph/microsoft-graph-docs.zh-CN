---
title: 获取 timeCard
description: 按 ID 获取 timeCard。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f1e2424a9303caa69aa2f64798f9c61388418723
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787850"
---
# <a name="get-timecard"></a><span data-ttu-id="328a4-103">获取 timeCard</span><span class="sxs-lookup"><span data-stu-id="328a4-103">Get timeCard</span></span>

<span data-ttu-id="328a4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="328a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="328a4-105">按 ID 检索 [timeCard](../resources/timeCard.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="328a4-105">Retrieve the properties and relationships of a [timeCard](../resources/timeCard.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="328a4-106">权限</span><span class="sxs-lookup"><span data-stu-id="328a4-106">Permissions</span></span>

<span data-ttu-id="328a4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="328a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="328a4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="328a4-109">Permission type</span></span>      | <span data-ttu-id="328a4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="328a4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="328a4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="328a4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="328a4-112">Schedule.Read.All、Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="328a4-112">Schedule.Read.All, Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="328a4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="328a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="328a4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="328a4-114">Not supported.</span></span>    |
|<span data-ttu-id="328a4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="328a4-115">Application</span></span> | <span data-ttu-id="328a4-116">Schedule.Read.All *、Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="328a4-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="328a4-117">\***重要提示：** 使用应用程序权限时，必须在请求 `MS-APP-ACTS-AS` 中包括 标头。</span><span class="sxs-lookup"><span data-stu-id="328a4-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="328a4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="328a4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timecards/{timecardID}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="328a4-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="328a4-119">Optional query parameters</span></span>
<span data-ttu-id="328a4-120">此方法不支持使用 OData 查询参数自定义响应。</span><span class="sxs-lookup"><span data-stu-id="328a4-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="328a4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="328a4-121">Request headers</span></span>

| <span data-ttu-id="328a4-122">标头</span><span class="sxs-lookup"><span data-stu-id="328a4-122">Header</span></span>       | <span data-ttu-id="328a4-123">值</span><span class="sxs-lookup"><span data-stu-id="328a4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="328a4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="328a4-124">Authorization</span></span>  | <span data-ttu-id="328a4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="328a4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="328a4-127">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="328a4-127">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="328a4-128">应用代表其操作的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="328a4-128">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="328a4-129">使用应用程序权限范围时是必需的。</span><span class="sxs-lookup"><span data-stu-id="328a4-129">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="328a4-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="328a4-130">Request body</span></span>
<span data-ttu-id="328a4-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="328a4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="328a4-132">响应</span><span class="sxs-lookup"><span data-stu-id="328a4-132">Response</span></span>

<span data-ttu-id="328a4-133">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [timeCard](../resources/timeCard.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="328a4-133">If successful, this method returns a `200 OK` response code and a [timeCard](../resources/timeCard.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="328a4-134">示例</span><span class="sxs-lookup"><span data-stu-id="328a4-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="328a4-135">请求</span><span class="sxs-lookup"><span data-stu-id="328a4-135">Request</span></span>
<span data-ttu-id="328a4-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="328a4-136">The following is an example of the request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="328a4-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="328a4-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-get"
}-->

```http
GET https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972
```

### <a name="response"></a><span data-ttu-id="328a4-138">响应</span><span class="sxs-lookup"><span data-stu-id="328a4-138">Response</span></span>

<span data-ttu-id="328a4-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="328a4-139">The following is an example of the response.</span></span> 

><span data-ttu-id="328a4-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="328a4-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972",
    "createdDateTime": "2021-05-27T22:58:41.327Z",
    "lastModifiedDateTime": "2021-05-27T23:02:04.187Z",
    "userId": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    "state": "clockedOut",
    "confirmedBy": "user,manager",
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
        "dateTime": "2021-05-27T22:58:41.327Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "clock in notes"
        }
    },
    "clockOutEvent": {
        "dateTime": "2021-05-27T23:01:46.205Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "clock out smaple notes"
        }
    },
    "breaks": [
        {
            "breakId": "BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f",
            "notes": null,
            "start": {
                "dateTime": "2021-05-27T22:59:59.328Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "start break smaple notes"
                }
            },
            "end": {
                "dateTime": "2021-05-27T23:01:10.205Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "end break smaple notes"
                }
            }
        }
    ],
    "originalEntry": {
        "clockInEvent": {
            "dateTime": "2021-05-27T22:58:41.327Z",
            "atApprovedLocation": null,
            "notes": {
                "contentType": "text",
                "content": "clock in notes"
            }
        },
        "clockOutEvent": {
            "dateTime": "2021-05-27T23:01:46.205Z",
            "atApprovedLocation": null,
            "notes": {
                "contentType": "text",
                "content": "clock out smaple notes"
            }
        },
        "breaks": [
            {
                "breakId": "BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f",
                "notes": null,
                "start": {
                    "dateTime": "2021-05-27T22:59:59.328Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "start break smaple notes"
                    }
                },
                "end": {
                    "dateTime": "2021-05-27T23:01:10.205Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "end break smaple notes"
                    }
                }
            }
        ]
    },
    "createdBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a timeCard by ID",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
