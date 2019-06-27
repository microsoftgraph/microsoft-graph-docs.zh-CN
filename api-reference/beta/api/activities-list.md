---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: 文件活动
localization_priority: Normal
ms.openlocfilehash: db1edeb786cfaf7d0257b0097b4403c95d281eb2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258777"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="b7e32-102">枚举活动（预览）</span><span class="sxs-lookup"><span data-stu-id="b7e32-102">Enumerate activities (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7e32-103">列出在某个项上或某个层次结构下发生的最近[活动](../resources/itemactivity.md)。</span><span class="sxs-lookup"><span data-stu-id="b7e32-103">List the recent [activities](../resources/itemactivity.md) that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="b7e32-104">**注意：** 活动处于限定预览阶段，尚未对所有租户可用。</span><span class="sxs-lookup"><span data-stu-id="b7e32-104">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="b7e32-105">权限</span><span class="sxs-lookup"><span data-stu-id="b7e32-105">Permissions</span></span>

<span data-ttu-id="b7e32-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7e32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7e32-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7e32-108">Permission type</span></span>                        | <span data-ttu-id="b7e32-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7e32-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="b7e32-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7e32-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7e32-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7e32-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="b7e32-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7e32-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7e32-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7e32-113">Not supported.</span></span>
|<span data-ttu-id="b7e32-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7e32-114">Application</span></span>                            | <span data-ttu-id="b7e32-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7e32-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="b7e32-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7e32-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="b7e32-117">示例</span><span class="sxs-lookup"><span data-stu-id="b7e32-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b7e32-118">请求</span><span class="sxs-lookup"><span data-stu-id="b7e32-118">Request</span></span>

<!-- { "blockType": "request", "name": "list-activities" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/activities
```

#### <a name="response"></a><span data-ttu-id="b7e32-119">响应</span><span class="sxs-lookup"><span data-stu-id="b7e32-119">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivity)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "action": {
                "comment": {}
            },
            "actor": {
                "user": {
                    "displayName": "Xavier Wilke"
                }
            },
            "id": "EJalEvjV1EgIYFQAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-29T18:34:40Z"
            }
        },
        {
            "action": {
                "edit": {},
                "version": {
                    "newVersion": "2.0"
                }
            },
            "actor": {
                "user": {
                    "displayName": "Judith Clemons"
                }
            },
            "id": "cInT6/fV1EgFYFQAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-29T16:23:35Z"
            }
        },
        {
            "action": {
                "mention": {
                    "mentionees": [
                        {
                            "user": {
                                "displayName": "Judith Clemons"
                            }
                        }
                    ]
                }
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "EBJa0vPV1EjFX1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:14:14Z"
            }
        },
        {
            "action": {
                "rename": {
                    "oldName": "Document2.docx"
                }
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "QFJFlfPV1Ei/X1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:12:32Z"
            }
        },
        {
            "action": {
                "create": {}
            },
            "actor": {
                "user": {
                    "displayName": "Misty Suarez"
                }
            },
            "id": "IJydkPPV1Ei9X1QAAAAAAA==",
            "times": {
                "recordedTime": "2017-07-28T20:02:24Z"
            }
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b7e32-120">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b7e32-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b7e32-121">C#</span><span class="sxs-lookup"><span data-stu-id="b7e32-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list-activities-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7e32-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="b7e32-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-activities-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b7e32-123">目标-C</span><span class="sxs-lookup"><span data-stu-id="b7e32-123">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/list-activities-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
    "Error: /api-reference/beta/api/activities-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/activities-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/activities-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
