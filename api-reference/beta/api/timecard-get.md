---
title: 获取 timeCard
description: 按 ID 获取 timeCard。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3ffeb7f57769cc84500b9c0dbb913c214ba6e144
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869516"
---
# <a name="get-timecard"></a><span data-ttu-id="821a2-103">获取 timeCard</span><span class="sxs-lookup"><span data-stu-id="821a2-103">Get timeCard</span></span>

<span data-ttu-id="821a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="821a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="821a2-105">按 ID 检索 [timeCard](../resources/timeCard.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="821a2-105">Retrieve the properties and relationships of a [timeCard](../resources/timeCard.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="821a2-106">权限</span><span class="sxs-lookup"><span data-stu-id="821a2-106">Permissions</span></span>

<span data-ttu-id="821a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="821a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="821a2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="821a2-109">Permission type</span></span>      | <span data-ttu-id="821a2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="821a2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="821a2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="821a2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="821a2-112">Schedule.Read.All、Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="821a2-112">Schedule.Read.All, Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="821a2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="821a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="821a2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="821a2-114">Not supported.</span></span>    |
|<span data-ttu-id="821a2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="821a2-115">Application</span></span> | <span data-ttu-id="821a2-116">Schedule.Read.All *、Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="821a2-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="821a2-117">\***重要提示：** 使用应用程序权限时，必须在请求 `MS-APP-ACTS-AS` 中包括 标头。</span><span class="sxs-lookup"><span data-stu-id="821a2-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="821a2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="821a2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timecards/{timecardID}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="821a2-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="821a2-119">Optional query parameters</span></span>
<span data-ttu-id="821a2-120">此方法不支持使用 OData 查询参数自定义响应。</span><span class="sxs-lookup"><span data-stu-id="821a2-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="821a2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="821a2-121">Request headers</span></span>

| <span data-ttu-id="821a2-122">标头</span><span class="sxs-lookup"><span data-stu-id="821a2-122">Header</span></span>       | <span data-ttu-id="821a2-123">值</span><span class="sxs-lookup"><span data-stu-id="821a2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="821a2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="821a2-124">Authorization</span></span>  | <span data-ttu-id="821a2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="821a2-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="821a2-127">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="821a2-127">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="821a2-128">应用代表其操作的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="821a2-128">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="821a2-129">使用应用程序权限范围时是必需的。</span><span class="sxs-lookup"><span data-stu-id="821a2-129">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="821a2-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="821a2-130">Request body</span></span>
<span data-ttu-id="821a2-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="821a2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="821a2-132">响应</span><span class="sxs-lookup"><span data-stu-id="821a2-132">Response</span></span>

<span data-ttu-id="821a2-133">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [timeCard](../resources/timeCard.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="821a2-133">If successful, this method returns a `200 OK` response code and a [timeCard](../resources/timeCard.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="821a2-134">示例</span><span class="sxs-lookup"><span data-stu-id="821a2-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="821a2-135">请求</span><span class="sxs-lookup"><span data-stu-id="821a2-135">Request</span></span>
<span data-ttu-id="821a2-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="821a2-136">The following is an example of the request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="821a2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="821a2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-get"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972
```
# <a name="c"></a>[<span data-ttu-id="821a2-138">C#</span><span class="sxs-lookup"><span data-stu-id="821a2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timecard-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="821a2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="821a2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="821a2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="821a2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="821a2-141">Java</span><span class="sxs-lookup"><span data-stu-id="821a2-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timecard-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="821a2-142">响应</span><span class="sxs-lookup"><span data-stu-id="821a2-142">Response</span></span>

<span data-ttu-id="821a2-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="821a2-143">The following is an example of the response.</span></span> 

><span data-ttu-id="821a2-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="821a2-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
