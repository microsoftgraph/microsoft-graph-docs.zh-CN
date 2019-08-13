---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: 文件活动
description: 列出在某个项上或某个层次结构下发生的最近活动。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: f794f13e4410cdef7c32c4fd444f31cf66131032
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319046"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="5041f-103">枚举活动（预览）</span><span class="sxs-lookup"><span data-stu-id="5041f-103">Enumerate activities (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5041f-104">列出在某个项上或某个层次结构下发生的最近[活动](../resources/itemactivity.md)。</span><span class="sxs-lookup"><span data-stu-id="5041f-104">List the recent [activities](../resources/itemactivity.md) that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="5041f-105">**注意：** 活动处于限定预览阶段，尚未对所有租户可用。</span><span class="sxs-lookup"><span data-stu-id="5041f-105">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="5041f-106">权限</span><span class="sxs-lookup"><span data-stu-id="5041f-106">Permissions</span></span>

<span data-ttu-id="5041f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5041f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5041f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5041f-109">Permission type</span></span>                        | <span data-ttu-id="5041f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5041f-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="5041f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5041f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5041f-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5041f-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="5041f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5041f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5041f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5041f-114">Not supported.</span></span>
|<span data-ttu-id="5041f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5041f-115">Application</span></span>                            | <span data-ttu-id="5041f-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5041f-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="5041f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5041f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="5041f-118">示例</span><span class="sxs-lookup"><span data-stu-id="5041f-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5041f-119">请求</span><span class="sxs-lookup"><span data-stu-id="5041f-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5041f-120">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5041f-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-activities" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/activities
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5041f-121">C#</span><span class="sxs-lookup"><span data-stu-id="5041f-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-activities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5041f-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5041f-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-activities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5041f-123">目标-C</span><span class="sxs-lookup"><span data-stu-id="5041f-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-activities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5041f-124">Java</span><span class="sxs-lookup"><span data-stu-id="5041f-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-activities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5041f-125">响应</span><span class="sxs-lookup"><span data-stu-id="5041f-125">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
  ]
}
-->
