---
title: 列出程序的 programControls
description: 在 Azure AD 访问评审功能中，列出链接到特定程序的所有 programControl 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 06eeeed15e6f46c8bbe802e504a1d7b15a83d867
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721774"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="ef8d0-103">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="ef8d0-103">List programControls of a program</span></span>

<span data-ttu-id="ef8d0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef8d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef8d0-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，列出链接到特定程序的所有 [programControl](../resources/programcontrol.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ef8d0-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef8d0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ef8d0-106">Permissions</span></span>
<span data-ttu-id="ef8d0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef8d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef8d0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef8d0-109">Permission type</span></span>                        | <span data-ttu-id="ef8d0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ef8d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef8d0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef8d0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef8d0-112">ProgramControl.Read.All、ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef8d0-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="ef8d0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef8d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef8d0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef8d0-114">Not supported.</span></span> |
|<span data-ttu-id="ef8d0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef8d0-115">Application</span></span>                            | <span data-ttu-id="ef8d0-116">ProgramControl.Read.All、ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef8d0-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="ef8d0-117">登录用户还必须具有允许其读取程序的目录角色。</span><span class="sxs-lookup"><span data-stu-id="ef8d0-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="ef8d0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef8d0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs/{programId}/controls
```
## <a name="request-headers"></a><span data-ttu-id="ef8d0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef8d0-119">Request headers</span></span>
| <span data-ttu-id="ef8d0-120">名称</span><span class="sxs-lookup"><span data-stu-id="ef8d0-120">Name</span></span>         | <span data-ttu-id="ef8d0-121">类型</span><span class="sxs-lookup"><span data-stu-id="ef8d0-121">Type</span></span>        | <span data-ttu-id="ef8d0-122">说明</span><span class="sxs-lookup"><span data-stu-id="ef8d0-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ef8d0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef8d0-123">Authorization</span></span> | <span data-ttu-id="ef8d0-124">string</span><span class="sxs-lookup"><span data-stu-id="ef8d0-124">string</span></span> | <span data-ttu-id="ef8d0-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="ef8d0-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef8d0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef8d0-127">Request body</span></span>
<span data-ttu-id="ef8d0-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="ef8d0-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="ef8d0-129">响应</span><span class="sxs-lookup"><span data-stu-id="ef8d0-129">Response</span></span>
<span data-ttu-id="ef8d0-130">如果成功，此方法在响应正文中返回响应代码和 `200, OK` [programControl](../resources/programcontrol.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="ef8d0-130">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef8d0-131">示例</span><span class="sxs-lookup"><span data-stu-id="ef8d0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef8d0-132">请求</span><span class="sxs-lookup"><span data-stu-id="ef8d0-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ef8d0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef8d0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programs/673a7379-9c38-4f01-bd9d-4fda7260b807/controls
```
# <a name="c"></a>[<span data-ttu-id="ef8d0-134">C#</span><span class="sxs-lookup"><span data-stu-id="ef8d0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontrol-from-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef8d0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef8d0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontrol-from-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef8d0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef8d0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontrol-from-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef8d0-137">Java</span><span class="sxs-lookup"><span data-stu-id="ef8d0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-programcontrol-from-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ef8d0-138">响应</span><span class="sxs-lookup"><span data-stu-id="ef8d0-138">Response</span></span>
><span data-ttu-id="ef8d0-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ef8d0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


