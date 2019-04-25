---
title: 删除 programControl
description: 在 "Azure AD access 评论" 功能中, 删除 programControl 对象。  这会断开某个程序的访问评审。
localization_priority: Normal
ms.openlocfilehash: 7510dfe80f758a75f190402d3ae426138e60bbed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538552"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="b726b-104">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="b726b-104">Delete programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b726b-105">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 删除[programControl](../resources/programcontrol.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b726b-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="b726b-106">这会断开某个程序的访问评审。</span><span class="sxs-lookup"><span data-stu-id="b726b-106">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="b726b-107">权限</span><span class="sxs-lookup"><span data-stu-id="b726b-107">Permissions</span></span>
<span data-ttu-id="b726b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b726b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b726b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b726b-110">Permission type</span></span>                        | <span data-ttu-id="b726b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b726b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b726b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b726b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b726b-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="b726b-113"></span></span>  <span data-ttu-id="b726b-114">登录用户还必须位于允许他们删除 programControl 的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="b726b-114">The signed in user must also be in a directory role which permits them to delete a programControl.</span></span> |
|<span data-ttu-id="b726b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b726b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b726b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b726b-116">Not supported.</span></span> |
|<span data-ttu-id="b726b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b726b-117">Application</span></span>                            | <span data-ttu-id="b726b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b726b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b726b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b726b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="b726b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b726b-120">Request headers</span></span>
| <span data-ttu-id="b726b-121">名称</span><span class="sxs-lookup"><span data-stu-id="b726b-121">Name</span></span>         | <span data-ttu-id="b726b-122">类型</span><span class="sxs-lookup"><span data-stu-id="b726b-122">Type</span></span>        | <span data-ttu-id="b726b-123">说明</span><span class="sxs-lookup"><span data-stu-id="b726b-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b726b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b726b-124">Authorization</span></span> | <span data-ttu-id="b726b-125">string</span><span class="sxs-lookup"><span data-stu-id="b726b-125">string</span></span> | <span data-ttu-id="b726b-p105">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="b726b-p105">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b726b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b726b-128">Request body</span></span>
<span data-ttu-id="b726b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b726b-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b726b-130">响应</span><span class="sxs-lookup"><span data-stu-id="b726b-130">Response</span></span>
<span data-ttu-id="b726b-p106">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b726b-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b726b-133">示例</span><span class="sxs-lookup"><span data-stu-id="b726b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b726b-134">请求</span><span class="sxs-lookup"><span data-stu-id="b726b-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="b726b-135">响应</span><span class="sxs-lookup"><span data-stu-id="b726b-135">Response</span></span>
><span data-ttu-id="b726b-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b726b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
