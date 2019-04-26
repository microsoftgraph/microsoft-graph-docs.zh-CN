---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: 文件活动
localization_priority: Normal
ms.openlocfilehash: 9131146bc627f1f611e817d66dcb86a084fef26f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323014"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="f689c-102">枚举活动（预览）</span><span class="sxs-lookup"><span data-stu-id="f689c-102">Enumerate activities (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f689c-103">列出在某个项上或某个层次结构下发生的最近[活动](../resources/itemactivity.md)。</span><span class="sxs-lookup"><span data-stu-id="f689c-103">List the recent [activities](../resources/itemactivity.md) that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="f689c-104">**注意：** 活动处于限定预览阶段，尚未对所有租户可用。</span><span class="sxs-lookup"><span data-stu-id="f689c-104">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="f689c-105">权限</span><span class="sxs-lookup"><span data-stu-id="f689c-105">Permissions</span></span>

<span data-ttu-id="f689c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f689c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f689c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f689c-108">Permission type</span></span>                        | <span data-ttu-id="f689c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f689c-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="f689c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f689c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f689c-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f689c-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="f689c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f689c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f689c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f689c-113">Not supported.</span></span>
|<span data-ttu-id="f689c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f689c-114">Application</span></span>                            | <span data-ttu-id="f689c-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f689c-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f689c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f689c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="f689c-117">示例</span><span class="sxs-lookup"><span data-stu-id="f689c-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f689c-118">请求</span><span class="sxs-lookup"><span data-stu-id="f689c-118">Request</span></span>

<!-- { "blockType": "request", "name": "list-activities" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/activities
```

#### <a name="response"></a><span data-ttu-id="f689c-119">响应</span><span class="sxs-lookup"><span data-stu-id="f689c-119">Response</span></span>

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
  "suppressions": []
}
-->
