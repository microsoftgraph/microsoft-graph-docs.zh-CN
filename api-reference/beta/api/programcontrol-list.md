---
title: 列表 programControls
description: 在 Azure AD 中访问审阅功能，在租户中的所有程序列出所有 programControl 对象。
localization_priority: Normal
ms.openlocfilehash: bc56fd5013bcf0013007b9d4264ab89eca02d43b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843951"
---
# <a name="list-programcontrols"></a><span data-ttu-id="b710f-103">列表 programControls</span><span class="sxs-lookup"><span data-stu-id="b710f-103">List programControls</span></span>

> <span data-ttu-id="b710f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b710f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b710f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b710f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b710f-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，在租户中的所有程序列出所有[programControl](../resources/programcontrol.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b710f-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="b710f-107">权限</span><span class="sxs-lookup"><span data-stu-id="b710f-107">Permissions</span></span>
<span data-ttu-id="b710f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b710f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b710f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b710f-110">Permission type</span></span>                        | <span data-ttu-id="b710f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b710f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b710f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b710f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b710f-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="b710f-113"></span></span>  <span data-ttu-id="b710f-114">登录的用户还必须在目录角色中允许他们阅读程序。</span><span class="sxs-lookup"><span data-stu-id="b710f-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="b710f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b710f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b710f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b710f-116">Not supported.</span></span> |
|<span data-ttu-id="b710f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b710f-117">Application</span></span>                            | <span data-ttu-id="b710f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b710f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b710f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b710f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="b710f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b710f-120">Request headers</span></span>
| <span data-ttu-id="b710f-121">名称</span><span class="sxs-lookup"><span data-stu-id="b710f-121">Name</span></span>         | <span data-ttu-id="b710f-122">类型</span><span class="sxs-lookup"><span data-stu-id="b710f-122">Type</span></span>        | <span data-ttu-id="b710f-123">说明</span><span class="sxs-lookup"><span data-stu-id="b710f-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b710f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b710f-124">Authorization</span></span> | <span data-ttu-id="b710f-125">string</span><span class="sxs-lookup"><span data-stu-id="b710f-125">string</span></span> | <span data-ttu-id="b710f-126">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="b710f-126">Bearer \{token\}.</span></span> <span data-ttu-id="b710f-127">必填。</span><span class="sxs-lookup"><span data-stu-id="b710f-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b710f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b710f-128">Request body</span></span>
<span data-ttu-id="b710f-129">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="b710f-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="b710f-130">响应</span><span class="sxs-lookup"><span data-stu-id="b710f-130">Response</span></span>
<span data-ttu-id="b710f-131">如果成功，此方法返回`200, OK`响应代码和响应正文中的[programControl](../resources/programcontrol.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="b710f-131">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b710f-132">示例</span><span class="sxs-lookup"><span data-stu-id="b710f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b710f-133">请求</span><span class="sxs-lookup"><span data-stu-id="b710f-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```http
GET https://graph.microsoft.com/beta/programControls
```

##### <a name="response"></a><span data-ttu-id="b710f-134">响应</span><span class="sxs-lookup"><span data-stu-id="b710f-134">Response</span></span>
><span data-ttu-id="b710f-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b710f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="b710f-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b710f-137">See also</span></span>

| <span data-ttu-id="b710f-138">方法</span><span class="sxs-lookup"><span data-stu-id="b710f-138">Method</span></span>           | <span data-ttu-id="b710f-139">返回类型</span><span class="sxs-lookup"><span data-stu-id="b710f-139">Return Type</span></span>    |<span data-ttu-id="b710f-140">说明</span><span class="sxs-lookup"><span data-stu-id="b710f-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b710f-141">对程序的列表 programControls</span><span class="sxs-lookup"><span data-stu-id="b710f-141">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="b710f-142">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="b710f-142">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="b710f-143">获取一个程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="b710f-143">Get a collection of the controls of a program.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
