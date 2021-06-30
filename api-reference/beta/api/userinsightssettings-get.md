---
title: 获取 userInsightsSettings
description: 检索 userInsightsSettings 对象的属性。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: d3d9f370318f74f3c25b8737de4cecc7dbb37d6d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210343"
---
# <a name="get-userinsightssettings"></a><span data-ttu-id="deac0-103">获取 userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="deac0-103">Get userInsightsSettings</span></span>

<span data-ttu-id="deac0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deac0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deac0-105">获取 [itemInsights](../resources/iteminsights.md) 和会议时间见解 [的用户可自定义的隐私设置](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)。</span><span class="sxs-lookup"><span data-stu-id="deac0-105">Get the user-customizable privacy settings for [itemInsights](../resources/iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1).</span></span>

## <a name="permissions"></a><span data-ttu-id="deac0-106">权限</span><span class="sxs-lookup"><span data-stu-id="deac0-106">Permissions</span></span>

<span data-ttu-id="deac0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="deac0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="deac0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="deac0-109">Permission type</span></span>      | <span data-ttu-id="deac0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="deac0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="deac0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="deac0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="deac0-112">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deac0-112">User.Read, User.ReadWrite</span></span> |
|<span data-ttu-id="deac0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="deac0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="deac0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="deac0-114">Not supported.</span></span>    |
|<span data-ttu-id="deac0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="deac0-115">Application</span></span> | <span data-ttu-id="deac0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="deac0-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="deac0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="deac0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/settings/itemInsights
GET /user/{userId}/settings/itemInsights
```

><span data-ttu-id="deac0-118">**注意：** 具有 或 的请求仅可供用户或具有 `userId` `userPrincipalName` User.ReadWrite.All 权限的用户访问。</span><span class="sxs-lookup"><span data-stu-id="deac0-118">**Note:** Requests with a `userId` or `userPrincipalName` are only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="deac0-119">若要了解详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="deac0-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

## <a name="request-headers"></a><span data-ttu-id="deac0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="deac0-120">Request headers</span></span>

| <span data-ttu-id="deac0-121">名称</span><span class="sxs-lookup"><span data-stu-id="deac0-121">Name</span></span>       | <span data-ttu-id="deac0-122">说明</span><span class="sxs-lookup"><span data-stu-id="deac0-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="deac0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="deac0-123">Authorization</span></span>  | <span data-ttu-id="deac0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="deac0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="deac0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="deac0-126">Request body</span></span>

<span data-ttu-id="deac0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="deac0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="deac0-128">响应</span><span class="sxs-lookup"><span data-stu-id="deac0-128">Response</span></span>

<span data-ttu-id="deac0-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userInsightsSettings](../resources/userinsightssettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="deac0-129">If successful, this method returns a `200 OK` response code and a [userInsightsSettings](../resources/userinsightssettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="deac0-130">示例</span><span class="sxs-lookup"><span data-stu-id="deac0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="deac0-131">请求</span><span class="sxs-lookup"><span data-stu-id="deac0-131">Request</span></span>

<span data-ttu-id="deac0-132">下面是请求获取用户项目见解和会议时间见解设置的示例。</span><span class="sxs-lookup"><span data-stu-id="deac0-132">The following is an example of the request to get user item insights and meeting hours insights settings.</span></span>


# <a name="http"></a>[<span data-ttu-id="deac0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="deac0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userInsightsSettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/settings/itemInsights
```
# <a name="c"></a>[<span data-ttu-id="deac0-134">C#</span><span class="sxs-lookup"><span data-stu-id="deac0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userinsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="deac0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="deac0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userinsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="deac0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="deac0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userinsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="deac0-137">Java</span><span class="sxs-lookup"><span data-stu-id="deac0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userinsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="deac0-138">响应</span><span class="sxs-lookup"><span data-stu-id="deac0-138">Response</span></span>

<span data-ttu-id="deac0-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="deac0-139">The following is an example of the response.</span></span> 
> <span data-ttu-id="deac0-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="deac0-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userInsightsSettings",
  "name": "get_userInsightsSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabled": true
}
```


