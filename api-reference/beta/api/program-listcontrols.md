---
title: 列出程序的 programControls
description: 在 "Azure AD access 评论" 功能中，列出链接到特定程序的所有 programControl 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 5299861843a6af0e3a41a8903d1d85af645672bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087942"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="abb65-103">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="abb65-103">List programControls of a program</span></span>

<span data-ttu-id="abb65-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abb65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abb65-105">在 "Azure AD [access 评论](../resources/accessreviews-root.md) " 功能中，列出链接到特定程序的所有 [programControl](../resources/programcontrol.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="abb65-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="abb65-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="abb65-106">Permissions</span></span>
<span data-ttu-id="abb65-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="abb65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abb65-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="abb65-109">Permission type</span></span>                        | <span data-ttu-id="abb65-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="abb65-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="abb65-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="abb65-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="abb65-112">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="abb65-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="abb65-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="abb65-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abb65-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="abb65-114">Not supported.</span></span> |
|<span data-ttu-id="abb65-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="abb65-115">Application</span></span>                            | <span data-ttu-id="abb65-116">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="abb65-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="abb65-117">登录用户还必须位于允许他们读取程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="abb65-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="abb65-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="abb65-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a><span data-ttu-id="abb65-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="abb65-119">Request headers</span></span>
| <span data-ttu-id="abb65-120">名称</span><span class="sxs-lookup"><span data-stu-id="abb65-120">Name</span></span>         | <span data-ttu-id="abb65-121">类型</span><span class="sxs-lookup"><span data-stu-id="abb65-121">Type</span></span>        | <span data-ttu-id="abb65-122">说明</span><span class="sxs-lookup"><span data-stu-id="abb65-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="abb65-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="abb65-123">Authorization</span></span> | <span data-ttu-id="abb65-124">string</span><span class="sxs-lookup"><span data-stu-id="abb65-124">string</span></span> | <span data-ttu-id="abb65-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="abb65-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="abb65-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="abb65-127">Request body</span></span>
<span data-ttu-id="abb65-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="abb65-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="abb65-129">响应</span><span class="sxs-lookup"><span data-stu-id="abb65-129">Response</span></span>
<span data-ttu-id="abb65-130">如果成功，此方法 `200, OK` 在响应正文中返回响应代码和 [programControl](../resources/programcontrol.md) 对象的数组。</span><span class="sxs-lookup"><span data-stu-id="abb65-130">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abb65-131">示例</span><span class="sxs-lookup"><span data-stu-id="abb65-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="abb65-132">请求</span><span class="sxs-lookup"><span data-stu-id="abb65-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="abb65-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="abb65-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programs/673a7379-9c38-4f01-bd9d-4fda7260b807/controls
```
# <a name="c"></a>[<span data-ttu-id="abb65-134">C#</span><span class="sxs-lookup"><span data-stu-id="abb65-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontrol-from-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="abb65-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abb65-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontrol-from-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="abb65-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abb65-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontrol-from-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="abb65-137">响应</span><span class="sxs-lookup"><span data-stu-id="abb65-137">Response</span></span>
><span data-ttu-id="abb65-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="abb65-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{

    "value": [
        {
            "id": "bd68f301-e44b-4ad1-ba6d-a07314ed2e79",
            "controlId": "bc81d51d-be53-4606-a8c2-f90a2beb5f40",
            "programId": "673a7379-9c38-4f01-bd9d-4fda7260b807",
            "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "guest user review",
            "status": "Completed",
            "createdDateTime": "2017-09-20T20:18:05.1318394Z"
        }
    ]
}

```


<!--
{
  "type": "#page.annotation",
  "description": "List programControls of a program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


