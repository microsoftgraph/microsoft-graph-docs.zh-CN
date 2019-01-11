---
title: 列表程序
description: 在 Azure AD 中访问审阅功能，列出程序的所有对象。
localization_priority: Normal
ms.openlocfilehash: 9ea71e5377b7dcfe7ca6de7cfaf221e2c6dfcd98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876291"
---
# <a name="list-programs"></a><span data-ttu-id="9ceda-103">列表程序</span><span class="sxs-lookup"><span data-stu-id="9ceda-103">List programs</span></span>

> <span data-ttu-id="9ceda-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9ceda-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ceda-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ceda-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ceda-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，列出[程序](../resources/program.md)的所有对象。</span><span class="sxs-lookup"><span data-stu-id="9ceda-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ceda-107">权限</span><span class="sxs-lookup"><span data-stu-id="9ceda-107">Permissions</span></span>
<span data-ttu-id="9ceda-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ceda-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ceda-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ceda-110">Permission type</span></span>                        | <span data-ttu-id="9ceda-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ceda-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ceda-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ceda-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ceda-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="9ceda-113"></span></span>  <span data-ttu-id="9ceda-114">登录的用户还必须在目录角色中允许他们阅读程序。</span><span class="sxs-lookup"><span data-stu-id="9ceda-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="9ceda-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ceda-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ceda-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ceda-116">Not supported.</span></span> |
|<span data-ttu-id="9ceda-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ceda-117">Application</span></span>                            | <span data-ttu-id="9ceda-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ceda-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ceda-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ceda-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="9ceda-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ceda-120">Request headers</span></span>
| <span data-ttu-id="9ceda-121">名称</span><span class="sxs-lookup"><span data-stu-id="9ceda-121">Name</span></span>         | <span data-ttu-id="9ceda-122">类型</span><span class="sxs-lookup"><span data-stu-id="9ceda-122">Type</span></span>        | <span data-ttu-id="9ceda-123">说明</span><span class="sxs-lookup"><span data-stu-id="9ceda-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9ceda-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ceda-124">Authorization</span></span> | <span data-ttu-id="9ceda-125">string</span><span class="sxs-lookup"><span data-stu-id="9ceda-125">string</span></span> | <span data-ttu-id="9ceda-126">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="9ceda-126">Bearer \{token\}.</span></span> <span data-ttu-id="9ceda-127">必填。</span><span class="sxs-lookup"><span data-stu-id="9ceda-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ceda-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ceda-128">Request body</span></span>
<span data-ttu-id="9ceda-129">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="9ceda-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="9ceda-130">响应</span><span class="sxs-lookup"><span data-stu-id="9ceda-130">Response</span></span>
<span data-ttu-id="9ceda-131">如果成功，此方法返回`200, OK`响应代码和响应正文中的[程序](../resources/program.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="9ceda-131">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ceda-132">示例</span><span class="sxs-lookup"><span data-stu-id="9ceda-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ceda-133">请求</span><span class="sxs-lookup"><span data-stu-id="9ceda-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="9ceda-134">响应</span><span class="sxs-lookup"><span data-stu-id="9ceda-134">Response</span></span>
><span data-ttu-id="9ceda-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9ceda-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
            "displayName": "testprogram3",
            "description": "test description"
        },
        {
            "id": "b4afdd74-b6cf-4239-9b08-dde9a91d18d2",
            "displayName": "Default Program",
            "description": "Built-in program to start managing access reviews"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="9ceda-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9ceda-137">See also</span></span>

| <span data-ttu-id="9ceda-138">方法</span><span class="sxs-lookup"><span data-stu-id="9ceda-138">Method</span></span>           | <span data-ttu-id="9ceda-139">返回类型</span><span class="sxs-lookup"><span data-stu-id="9ceda-139">Return Type</span></span>    |<span data-ttu-id="9ceda-140">说明</span><span class="sxs-lookup"><span data-stu-id="9ceda-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9ceda-141">对程序的列表 programControls</span><span class="sxs-lookup"><span data-stu-id="9ceda-141">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="9ceda-142">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="9ceda-142">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="9ceda-143">获取一个程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="9ceda-143">Get a collection of the controls of a program.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
