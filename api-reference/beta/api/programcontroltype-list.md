---
title: 列表 programControlTypes
description: 在 Azure AD 中访问审阅功能，列出所有 programControlType 对象。
ms.openlocfilehash: 9e3b8efccd8d8be96ef1295dfba1a5c2e329c756
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049443"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="70523-103">列表 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="70523-103">List programControlTypes</span></span>

> <span data-ttu-id="70523-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="70523-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70523-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="70523-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70523-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，列出所有[programControlType](../resources/programcontroltype.md)对象。</span><span class="sxs-lookup"><span data-stu-id="70523-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="70523-107">权限</span><span class="sxs-lookup"><span data-stu-id="70523-107">Permissions</span></span>
<span data-ttu-id="70523-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70523-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70523-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="70523-110">Permission type</span></span>                        | <span data-ttu-id="70523-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70523-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="70523-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70523-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="70523-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="70523-113"></span></span>  <span data-ttu-id="70523-114">登录的用户还必须在目录角色中允许他们阅读程序。</span><span class="sxs-lookup"><span data-stu-id="70523-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="70523-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70523-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70523-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="70523-116">Not supported.</span></span> |
|<span data-ttu-id="70523-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="70523-117">Application</span></span>                            | <span data-ttu-id="70523-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="70523-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70523-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70523-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="70523-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="70523-120">Request headers</span></span>
| <span data-ttu-id="70523-121">名称</span><span class="sxs-lookup"><span data-stu-id="70523-121">Name</span></span>         | <span data-ttu-id="70523-122">类型</span><span class="sxs-lookup"><span data-stu-id="70523-122">Type</span></span>        | <span data-ttu-id="70523-123">说明</span><span class="sxs-lookup"><span data-stu-id="70523-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="70523-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="70523-124">Authorization</span></span> | <span data-ttu-id="70523-125">string</span><span class="sxs-lookup"><span data-stu-id="70523-125">string</span></span> | <span data-ttu-id="70523-126">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="70523-126">Bearer \{token\}.</span></span> <span data-ttu-id="70523-127">必需。</span><span class="sxs-lookup"><span data-stu-id="70523-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70523-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="70523-128">Request body</span></span>
<span data-ttu-id="70523-129">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="70523-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="70523-130">响应</span><span class="sxs-lookup"><span data-stu-id="70523-130">Response</span></span>
<span data-ttu-id="70523-131">如果成功，此方法返回`200, OK`响应代码和响应正文中的[programControlType](../resources/programcontroltype.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="70523-131">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70523-132">示例</span><span class="sxs-lookup"><span data-stu-id="70523-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70523-133">请求</span><span class="sxs-lookup"><span data-stu-id="70523-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```http
GET https://graph.microsoft.com/beta/programControlTypes
```

##### <a name="response"></a><span data-ttu-id="70523-134">响应</span><span class="sxs-lookup"><span data-stu-id="70523-134">Response</span></span>
><span data-ttu-id="70523-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="70523-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControlType",
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

## <a name="see-also"></a><span data-ttu-id="70523-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="70523-137">See also</span></span>

| <span data-ttu-id="70523-138">方法</span><span class="sxs-lookup"><span data-stu-id="70523-138">Method</span></span>           | <span data-ttu-id="70523-139">返回类型</span><span class="sxs-lookup"><span data-stu-id="70523-139">Return Type</span></span>    |<span data-ttu-id="70523-140">说明</span><span class="sxs-lookup"><span data-stu-id="70523-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70523-141">对程序的列表 programControls</span><span class="sxs-lookup"><span data-stu-id="70523-141">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="70523-142">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="70523-142">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="70523-143">获取一个程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="70523-143">Get a collection of the controls of a program.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
