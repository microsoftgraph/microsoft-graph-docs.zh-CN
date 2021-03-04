---
title: 列出 programControls
description: 在 Azure AD 访问评审功能中，列出租户中所有程序的所有 programControl 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 7e689be520d337916774e28d8204e99ca412b65d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442192"
---
# <a name="list-programcontrols"></a><span data-ttu-id="971de-103">列出 programControls</span><span class="sxs-lookup"><span data-stu-id="971de-103">List programControls</span></span>

<span data-ttu-id="971de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="971de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="971de-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，列出租户中所有程序的所有 [programControl](../resources/programcontrol.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="971de-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="971de-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="971de-106">Permissions</span></span>
<span data-ttu-id="971de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="971de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="971de-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="971de-109">Permission type</span></span>                        | <span data-ttu-id="971de-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="971de-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="971de-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="971de-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="971de-112">ProgramControl.Read.All、ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="971de-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="971de-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="971de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="971de-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="971de-114">Not supported.</span></span> |
|<span data-ttu-id="971de-115">Application</span><span class="sxs-lookup"><span data-stu-id="971de-115">Application</span></span>                            | <span data-ttu-id="971de-116">ProgramControl.Read.All、ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="971de-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="971de-117">登录用户还必须是允许其读取程序的目录角色。</span><span class="sxs-lookup"><span data-stu-id="971de-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="971de-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="971de-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="971de-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="971de-119">Request headers</span></span>
| <span data-ttu-id="971de-120">名称</span><span class="sxs-lookup"><span data-stu-id="971de-120">Name</span></span>         | <span data-ttu-id="971de-121">类型</span><span class="sxs-lookup"><span data-stu-id="971de-121">Type</span></span>        | <span data-ttu-id="971de-122">说明</span><span class="sxs-lookup"><span data-stu-id="971de-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="971de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="971de-123">Authorization</span></span> | <span data-ttu-id="971de-124">string</span><span class="sxs-lookup"><span data-stu-id="971de-124">string</span></span> | <span data-ttu-id="971de-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="971de-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="971de-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="971de-127">Request body</span></span>
<span data-ttu-id="971de-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="971de-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="971de-129">响应</span><span class="sxs-lookup"><span data-stu-id="971de-129">Response</span></span>
<span data-ttu-id="971de-130">如果成功，此方法在响应正文中返回响应代码和 `200, OK` [programControl](../resources/programcontrol.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="971de-130">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="971de-131">示例</span><span class="sxs-lookup"><span data-stu-id="971de-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="971de-132">请求</span><span class="sxs-lookup"><span data-stu-id="971de-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="971de-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="971de-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programControls
```
# <a name="c"></a>[<span data-ttu-id="971de-134">C#</span><span class="sxs-lookup"><span data-stu-id="971de-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontrol-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="971de-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="971de-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontrol-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="971de-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="971de-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontrol-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="971de-137">Java</span><span class="sxs-lookup"><span data-stu-id="971de-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-programcontrol-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="971de-138">响应</span><span class="sxs-lookup"><span data-stu-id="971de-138">Response</span></span>
><span data-ttu-id="971de-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="971de-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "id": "f6abf8ef-a05e-4788-adc9-5af909c400af",
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

## <a name="see-also"></a><span data-ttu-id="971de-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="971de-141">See also</span></span>

| <span data-ttu-id="971de-142">方法</span><span class="sxs-lookup"><span data-stu-id="971de-142">Method</span></span>           | <span data-ttu-id="971de-143">返回类型</span><span class="sxs-lookup"><span data-stu-id="971de-143">Return Type</span></span>    |<span data-ttu-id="971de-144">说明</span><span class="sxs-lookup"><span data-stu-id="971de-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="971de-145">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="971de-145">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="971de-146">[programControl](../resources/programcontrol.md) 集合</span><span class="sxs-lookup"><span data-stu-id="971de-146">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="971de-147">获取程序控件的集合。</span><span class="sxs-lookup"><span data-stu-id="971de-147">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


