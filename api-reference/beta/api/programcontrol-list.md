---
title: 列出 programControls
description: 在 Azure AD access 评论功能中, 列出租户中的所有程序中的所有 programControl 对象。
localization_priority: Normal
ms.openlocfilehash: bfc224c0897b9e9edba2114bac4d88e06ca0720d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332069"
---
# <a name="list-programcontrols"></a><span data-ttu-id="c7b9d-103">列出 programControls</span><span class="sxs-lookup"><span data-stu-id="c7b9d-103">List programControls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7b9d-104">在 Azure AD [access 评论](../resources/accessreviews-root.md)功能中, 列出租户中的所有程序中的所有[programControl](../resources/programcontrol.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c7b9d-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7b9d-105">权限</span><span class="sxs-lookup"><span data-stu-id="c7b9d-105">Permissions</span></span>
<span data-ttu-id="c7b9d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7b9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7b9d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7b9d-108">Permission type</span></span>                        | <span data-ttu-id="c7b9d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7b9d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7b9d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7b9d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7b9d-111">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="c7b9d-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="c7b9d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7b9d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7b9d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7b9d-113">Not supported.</span></span> |
|<span data-ttu-id="c7b9d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7b9d-114">Application</span></span>                            | <span data-ttu-id="c7b9d-115">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="c7b9d-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="c7b9d-116">登录用户还必须位于允许他们读取程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="c7b9d-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="c7b9d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7b9d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="c7b9d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7b9d-118">Request headers</span></span>
| <span data-ttu-id="c7b9d-119">名称</span><span class="sxs-lookup"><span data-stu-id="c7b9d-119">Name</span></span>         | <span data-ttu-id="c7b9d-120">类型</span><span class="sxs-lookup"><span data-stu-id="c7b9d-120">Type</span></span>        | <span data-ttu-id="c7b9d-121">说明</span><span class="sxs-lookup"><span data-stu-id="c7b9d-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c7b9d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7b9d-122">Authorization</span></span> | <span data-ttu-id="c7b9d-123">string</span><span class="sxs-lookup"><span data-stu-id="c7b9d-123">string</span></span> | <span data-ttu-id="c7b9d-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7b9d-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7b9d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7b9d-126">Request body</span></span>
<span data-ttu-id="c7b9d-127">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7b9d-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="c7b9d-128">响应</span><span class="sxs-lookup"><span data-stu-id="c7b9d-128">Response</span></span>
<span data-ttu-id="c7b9d-129">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[programControl](../resources/programcontrol.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="c7b9d-129">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7b9d-130">示例</span><span class="sxs-lookup"><span data-stu-id="c7b9d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7b9d-131">请求</span><span class="sxs-lookup"><span data-stu-id="c7b9d-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```http
GET https://graph.microsoft.com/beta/programControls
```

##### <a name="response"></a><span data-ttu-id="c7b9d-132">响应</span><span class="sxs-lookup"><span data-stu-id="c7b9d-132">Response</span></span>
><span data-ttu-id="c7b9d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c7b9d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="c7b9d-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c7b9d-135">See also</span></span>

| <span data-ttu-id="c7b9d-136">方法</span><span class="sxs-lookup"><span data-stu-id="c7b9d-136">Method</span></span>           | <span data-ttu-id="c7b9d-137">返回类型</span><span class="sxs-lookup"><span data-stu-id="c7b9d-137">Return Type</span></span>    |<span data-ttu-id="c7b9d-138">说明</span><span class="sxs-lookup"><span data-stu-id="c7b9d-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c7b9d-139">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="c7b9d-139">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="c7b9d-140">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="c7b9d-140">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="c7b9d-141">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="c7b9d-141">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
