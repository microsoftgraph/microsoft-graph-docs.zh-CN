---
author: daspek
ms.author: dspektor
ms.date: 09/10/2017
title: 文件活动
localization_priority: Normal
ms.openlocfilehash: 75849fc67febe8c0f22d4dbd057da98aea5e8854
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459481"
---
# <a name="enumerate-activities-preview"></a><span data-ttu-id="4fab9-102">枚举活动（预览）</span><span class="sxs-lookup"><span data-stu-id="4fab9-102">Enumerate activities (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fab9-103">列出在某个项上或某个层次结构下发生的最近[活动][]。</span><span class="sxs-lookup"><span data-stu-id="4fab9-103">List the recent [activities][] that took place on an item or under a hierarchy.</span></span>

<span data-ttu-id="4fab9-104">**注意：** 活动处于限定预览阶段，尚未对所有租户可用。</span><span class="sxs-lookup"><span data-stu-id="4fab9-104">**Note:** Activities is in a limited Preview and not yet available to all tenants.</span></span>

[活动]: ../resources/itemactivity.md
[activities]: ../resources/itemactivity.md

## <a name="permissions"></a><span data-ttu-id="4fab9-106">权限</span><span class="sxs-lookup"><span data-stu-id="4fab9-106">Permissions</span></span>

<span data-ttu-id="4fab9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fab9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fab9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fab9-109">Permission type</span></span>                        | <span data-ttu-id="4fab9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4fab9-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="4fab9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fab9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4fab9-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fab9-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="4fab9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fab9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fab9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fab9-114">Not supported.</span></span>
|<span data-ttu-id="4fab9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4fab9-115">Application</span></span>                            | <span data-ttu-id="4fab9-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fab9-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="4fab9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fab9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/activities
GET /drives/{drive-id}/items/{item-id}/activities
GET /sites/{site-id}/lists/{list-id}/activities
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/activities
```

## <a name="example"></a><span data-ttu-id="4fab9-118">示例</span><span class="sxs-lookup"><span data-stu-id="4fab9-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4fab9-119">请求</span><span class="sxs-lookup"><span data-stu-id="4fab9-119">Request</span></span>

<!-- { "blockType": "request", "name": "list-activities" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/activities
```

#### <a name="response"></a><span data-ttu-id="4fab9-120">响应</span><span class="sxs-lookup"><span data-stu-id="4fab9-120">Response</span></span>

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
    "Error: /api-reference/beta/api/activities-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
