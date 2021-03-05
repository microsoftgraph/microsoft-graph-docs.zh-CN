---
author: daspek
ms.date: 09/10/2017
title: 文件活动
description: 列出在某个项上或某个层次结构下发生的最近活动。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: f345551f4685023581eea58fa2615e9c723303f5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472256"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="cb113-103">枚举活动（预览）</span><span class="sxs-lookup"><span data-stu-id="cb113-103">Enumerate activities (preview)</span></span>

<span data-ttu-id="cb113-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb113-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb113-105">列出在某个项上或某个层次结构下发生的最近[活动](../resources/itemactivity.md)。</span><span class="sxs-lookup"><span data-stu-id="cb113-105">List the recent [activities](../resources/itemactivity.md) that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="cb113-106">**注意：** 活动处于限定预览阶段，尚未对所有租户可用。</span><span class="sxs-lookup"><span data-stu-id="cb113-106">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="cb113-107">权限</span><span class="sxs-lookup"><span data-stu-id="cb113-107">Permissions</span></span>

<span data-ttu-id="cb113-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb113-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb113-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb113-110">Permission type</span></span>                        | <span data-ttu-id="cb113-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb113-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="cb113-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb113-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb113-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb113-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="cb113-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb113-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb113-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb113-115">Not supported.</span></span>
|<span data-ttu-id="cb113-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb113-116">Application</span></span>                            | <span data-ttu-id="cb113-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb113-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="cb113-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb113-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="cb113-119">示例</span><span class="sxs-lookup"><span data-stu-id="cb113-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cb113-120">请求</span><span class="sxs-lookup"><span data-stu-id="cb113-120">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cb113-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb113-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-activities" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/activities
```
# <a name="c"></a>[<span data-ttu-id="cb113-122">C#</span><span class="sxs-lookup"><span data-stu-id="cb113-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-activities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb113-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb113-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-activities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb113-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb113-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-activities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb113-125">Java</span><span class="sxs-lookup"><span data-stu-id="cb113-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-activities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cb113-126">响应</span><span class="sxs-lookup"><span data-stu-id="cb113-126">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivity)", "truncated": true } -->

```http
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


