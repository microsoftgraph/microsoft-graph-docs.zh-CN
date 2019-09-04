---
title: 获取 administrativeUnit
description: 检索与此**educationSchool**相对应的简单目录**administrativeUnit** 。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6707717bf7cf3e98eabdb400d2d677c2e98b73fd
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720387"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="658b2-103">获取 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="658b2-103">Get administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="658b2-104">检索与此**educationSchool**相对应的简单目录**administrativeUnit** 。</span><span class="sxs-lookup"><span data-stu-id="658b2-104">Retrieve the simple directory **administrativeUnit** that corresponds to this **educationSchool**.</span></span>

><span data-ttu-id="658b2-105">**注意：** 如果使用委派令牌，成员只能看到有关自己学校的信息。</span><span class="sxs-lookup"><span data-stu-id="658b2-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="658b2-106">在这种情况下，使用 `...beta/education/me/schools` 资源。</span><span class="sxs-lookup"><span data-stu-id="658b2-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="658b2-107">权限</span><span class="sxs-lookup"><span data-stu-id="658b2-107">Permissions</span></span>
<span data-ttu-id="658b2-108">要调用此 API，需要一组权限。</span><span class="sxs-lookup"><span data-stu-id="658b2-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="658b2-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="658b2-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="658b2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="658b2-110">Permission type</span></span>      | <span data-ttu-id="658b2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="658b2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="658b2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="658b2-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="658b2-113">来自 EduRoster.ReadBasic、EduRoster.Read、EduRoster.Write 以及 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="658b2-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="658b2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="658b2-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="658b2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="658b2-115">Not supported.</span></span>  |
|<span data-ttu-id="658b2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="658b2-116">Application</span></span> | <span data-ttu-id="658b2-117">EduRoster.Read.All、EduRoster.ReadWrite.All 以及 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="658b2-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="658b2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="658b2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/administrativeUnit
```
## <a name="request-headers"></a><span data-ttu-id="658b2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="658b2-119">Request headers</span></span>
| <span data-ttu-id="658b2-120">标头</span><span class="sxs-lookup"><span data-stu-id="658b2-120">Header</span></span>       | <span data-ttu-id="658b2-121">值</span><span class="sxs-lookup"><span data-stu-id="658b2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="658b2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="658b2-122">Authorization</span></span>  | <span data-ttu-id="658b2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="658b2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="658b2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="658b2-125">Request body</span></span>
<span data-ttu-id="658b2-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="658b2-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="658b2-127">响应</span><span class="sxs-lookup"><span data-stu-id="658b2-127">Response</span></span>
<span data-ttu-id="658b2-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[administrativeUnit](../resources/administrativeunit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="658b2-128">If successful, this method returns a `200 OK` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="658b2-129">示例</span><span class="sxs-lookup"><span data-stu-id="658b2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="658b2-130">请求</span><span class="sxs-lookup"><span data-stu-id="658b2-130">Request</span></span>
<span data-ttu-id="658b2-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="658b2-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="658b2-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="658b2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_administrativeUnit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/2961761D-8094-4183-A9F6-8E36E966C7D9/administrativeUnit
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="658b2-133">C#</span><span class="sxs-lookup"><span data-stu-id="658b2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="658b2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="658b2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="658b2-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="658b2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="658b2-136">响应</span><span class="sxs-lookup"><span data-stu-id="658b2-136">Response</span></span>
<span data-ttu-id="658b2-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="658b2-137">The following is an example of the response.</span></span> 

><span data-ttu-id="658b2-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="658b2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

<!-- uuid: A681726F-B4A7-4BCF-9407-F87CB9A4771D
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
