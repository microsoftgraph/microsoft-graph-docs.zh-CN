---
title: 列表 programControlTypes
description: 在 Azure AD 中访问审阅功能，列出所有 programControlType 对象。
localization_priority: Normal
ms.openlocfilehash: 00983cadf4bd1e0cf136c594f06ac3ee6fbb1de5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515690"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="33a6b-103">列表 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="33a6b-103">List programControlTypes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33a6b-104">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，列出所有[programControlType](../resources/programcontroltype.md)对象。</span><span class="sxs-lookup"><span data-stu-id="33a6b-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="33a6b-105">权限</span><span class="sxs-lookup"><span data-stu-id="33a6b-105">Permissions</span></span>
<span data-ttu-id="33a6b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="33a6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33a6b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="33a6b-108">Permission type</span></span>                        | <span data-ttu-id="33a6b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="33a6b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="33a6b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33a6b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="33a6b-111">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="33a6b-111"></span></span>  <span data-ttu-id="33a6b-112">登录的用户还必须在目录角色中允许他们阅读程序。</span><span class="sxs-lookup"><span data-stu-id="33a6b-112">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="33a6b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33a6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33a6b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="33a6b-114">Not supported.</span></span> |
|<span data-ttu-id="33a6b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="33a6b-115">Application</span></span>                            | <span data-ttu-id="33a6b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="33a6b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="33a6b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33a6b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="33a6b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="33a6b-118">Request headers</span></span>
| <span data-ttu-id="33a6b-119">名称</span><span class="sxs-lookup"><span data-stu-id="33a6b-119">Name</span></span>         | <span data-ttu-id="33a6b-120">类型</span><span class="sxs-lookup"><span data-stu-id="33a6b-120">Type</span></span>        | <span data-ttu-id="33a6b-121">说明</span><span class="sxs-lookup"><span data-stu-id="33a6b-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="33a6b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="33a6b-122">Authorization</span></span> | <span data-ttu-id="33a6b-123">string</span><span class="sxs-lookup"><span data-stu-id="33a6b-123">string</span></span> | <span data-ttu-id="33a6b-124">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="33a6b-124">Bearer \{token\}.</span></span> <span data-ttu-id="33a6b-125">必需。</span><span class="sxs-lookup"><span data-stu-id="33a6b-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33a6b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="33a6b-126">Request body</span></span>
<span data-ttu-id="33a6b-127">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="33a6b-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="33a6b-128">响应</span><span class="sxs-lookup"><span data-stu-id="33a6b-128">Response</span></span>
<span data-ttu-id="33a6b-129">如果成功，此方法返回`200, OK`响应代码和响应正文中的[programControlType](../resources/programcontroltype.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="33a6b-129">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33a6b-130">示例</span><span class="sxs-lookup"><span data-stu-id="33a6b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33a6b-131">请求</span><span class="sxs-lookup"><span data-stu-id="33a6b-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```http
GET https://graph.microsoft.com/beta/programControlTypes
```

##### <a name="response"></a><span data-ttu-id="33a6b-132">响应</span><span class="sxs-lookup"><span data-stu-id="33a6b-132">Response</span></span>
><span data-ttu-id="33a6b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="33a6b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="33a6b-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="33a6b-135">See also</span></span>

| <span data-ttu-id="33a6b-136">方法</span><span class="sxs-lookup"><span data-stu-id="33a6b-136">Method</span></span>           | <span data-ttu-id="33a6b-137">返回类型</span><span class="sxs-lookup"><span data-stu-id="33a6b-137">Return Type</span></span>    |<span data-ttu-id="33a6b-138">说明</span><span class="sxs-lookup"><span data-stu-id="33a6b-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="33a6b-139">对程序的列表 programControls</span><span class="sxs-lookup"><span data-stu-id="33a6b-139">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="33a6b-140">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="33a6b-140">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="33a6b-141">获取一个程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="33a6b-141">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
