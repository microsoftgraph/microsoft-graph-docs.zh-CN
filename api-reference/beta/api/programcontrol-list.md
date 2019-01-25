---
title: 列表 programControls
description: 在 Azure AD 中访问审阅功能，在租户中的所有程序列出所有 programControl 对象。
localization_priority: Normal
ms.openlocfilehash: 52361e3878445d4f739fd0cd33817d5b254ddc03
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525057"
---
# <a name="list-programcontrols"></a><span data-ttu-id="c1999-103">列表 programControls</span><span class="sxs-lookup"><span data-stu-id="c1999-103">List programControls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1999-104">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，在租户中的所有程序列出所有[programControl](../resources/programcontrol.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c1999-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="c1999-105">权限</span><span class="sxs-lookup"><span data-stu-id="c1999-105">Permissions</span></span>
<span data-ttu-id="c1999-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1999-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1999-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1999-108">Permission type</span></span>                        | <span data-ttu-id="c1999-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1999-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1999-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1999-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1999-111">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="c1999-111"></span></span>  <span data-ttu-id="c1999-112">登录的用户还必须在目录角色中允许他们阅读程序。</span><span class="sxs-lookup"><span data-stu-id="c1999-112">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="c1999-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1999-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1999-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1999-114">Not supported.</span></span> |
|<span data-ttu-id="c1999-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1999-115">Application</span></span>                            | <span data-ttu-id="c1999-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1999-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1999-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1999-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="c1999-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1999-118">Request headers</span></span>
| <span data-ttu-id="c1999-119">名称</span><span class="sxs-lookup"><span data-stu-id="c1999-119">Name</span></span>         | <span data-ttu-id="c1999-120">类型</span><span class="sxs-lookup"><span data-stu-id="c1999-120">Type</span></span>        | <span data-ttu-id="c1999-121">说明</span><span class="sxs-lookup"><span data-stu-id="c1999-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c1999-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1999-122">Authorization</span></span> | <span data-ttu-id="c1999-123">string</span><span class="sxs-lookup"><span data-stu-id="c1999-123">string</span></span> | <span data-ttu-id="c1999-124">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="c1999-124">Bearer \{token\}.</span></span> <span data-ttu-id="c1999-125">必需。</span><span class="sxs-lookup"><span data-stu-id="c1999-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1999-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1999-126">Request body</span></span>
<span data-ttu-id="c1999-127">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1999-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="c1999-128">响应</span><span class="sxs-lookup"><span data-stu-id="c1999-128">Response</span></span>
<span data-ttu-id="c1999-129">如果成功，此方法返回`200, OK`响应代码和响应正文中的[programControl](../resources/programcontrol.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="c1999-129">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1999-130">示例</span><span class="sxs-lookup"><span data-stu-id="c1999-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1999-131">请求</span><span class="sxs-lookup"><span data-stu-id="c1999-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```http
GET https://graph.microsoft.com/beta/programControls
```

##### <a name="response"></a><span data-ttu-id="c1999-132">响应</span><span class="sxs-lookup"><span data-stu-id="c1999-132">Response</span></span>
><span data-ttu-id="c1999-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c1999-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="c1999-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c1999-135">See also</span></span>

| <span data-ttu-id="c1999-136">方法</span><span class="sxs-lookup"><span data-stu-id="c1999-136">Method</span></span>           | <span data-ttu-id="c1999-137">返回类型</span><span class="sxs-lookup"><span data-stu-id="c1999-137">Return Type</span></span>    |<span data-ttu-id="c1999-138">说明</span><span class="sxs-lookup"><span data-stu-id="c1999-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c1999-139">对程序的列表 programControls</span><span class="sxs-lookup"><span data-stu-id="c1999-139">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="c1999-140">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="c1999-140">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="c1999-141">获取一个程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="c1999-141">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
