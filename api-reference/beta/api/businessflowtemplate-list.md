---
title: 列表 businessFlowTemplates
description: 在 Azure AD 中访问审阅功能，列出所有 businessFlowTemplate 对象。
localization_priority: Normal
ms.openlocfilehash: 021a3c939c6642caf5200b5e9cc4e47b390019b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829496"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="89502-103">列表 businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="89502-103">List businessFlowTemplates</span></span>

> <span data-ttu-id="89502-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="89502-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89502-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="89502-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89502-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，列出所有[businessFlowTemplate](../resources/businessflowtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="89502-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="89502-107">权限</span><span class="sxs-lookup"><span data-stu-id="89502-107">Permissions</span></span>
<span data-ttu-id="89502-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89502-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89502-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="89502-110">Permission type</span></span>                        | <span data-ttu-id="89502-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89502-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="89502-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89502-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="89502-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="89502-113"></span></span>  <span data-ttu-id="89502-114">登录的用户还必须在目录角色中允许他们阅读访问审阅。</span><span class="sxs-lookup"><span data-stu-id="89502-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="89502-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89502-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89502-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="89502-116">Not supported.</span></span> |
|<span data-ttu-id="89502-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="89502-117">Application</span></span>                            | <span data-ttu-id="89502-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="89502-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89502-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89502-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="89502-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="89502-120">Request headers</span></span>
| <span data-ttu-id="89502-121">Name</span><span class="sxs-lookup"><span data-stu-id="89502-121">Name</span></span>         | <span data-ttu-id="89502-122">类型</span><span class="sxs-lookup"><span data-stu-id="89502-122">Type</span></span>        | <span data-ttu-id="89502-123">说明</span><span class="sxs-lookup"><span data-stu-id="89502-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="89502-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="89502-124">Authorization</span></span> | <span data-ttu-id="89502-125">字符串</span><span class="sxs-lookup"><span data-stu-id="89502-125">string</span></span> | <span data-ttu-id="89502-126">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="89502-126">Bearer \{token\}.</span></span> <span data-ttu-id="89502-127">必需。</span><span class="sxs-lookup"><span data-stu-id="89502-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89502-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="89502-128">Request body</span></span>
<span data-ttu-id="89502-129">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="89502-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="89502-130">响应</span><span class="sxs-lookup"><span data-stu-id="89502-130">Response</span></span>
<span data-ttu-id="89502-131">如果成功，此方法返回`200, OK`响应代码和响应正文中的[businessFlowTemplate](../resources/businessflowtemplate.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="89502-131">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89502-132">示例</span><span class="sxs-lookup"><span data-stu-id="89502-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89502-133">请求</span><span class="sxs-lookup"><span data-stu-id="89502-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businesFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businesFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="89502-134">响应</span><span class="sxs-lookup"><span data-stu-id="89502-134">Response</span></span>
><span data-ttu-id="89502-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="89502-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.businessFlowTemplate",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "842169fe-e1b7-4ce9-98b6-6a9db02eec6b",
            "displayName": "Access Reviews for External Users' access to groups"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access Reviews for External Users' access to applications"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access Reviews for All Users' assignment to applications"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access Reviews for Office 365 Groups' membership"
        } 
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="89502-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="89502-137">See also</span></span>

| <span data-ttu-id="89502-138">方法</span><span class="sxs-lookup"><span data-stu-id="89502-138">Method</span></span>           | <span data-ttu-id="89502-139">返回类型</span><span class="sxs-lookup"><span data-stu-id="89502-139">Return Type</span></span>    |<span data-ttu-id="89502-140">说明</span><span class="sxs-lookup"><span data-stu-id="89502-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="89502-141">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="89502-141">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="89502-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="89502-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="89502-143">创建新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="89502-143">Create a new accessReview.</span></span> |




<!-- {
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
