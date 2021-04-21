---
title: 更新 userFlowLanguagePage
description: 更新 userFlowLanguagePage 对象中的值。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4f38a29a7471eb48d039ded52f7ac4f24a3d17bf
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920445"
---
# <a name="update-userflowlanguagepage"></a><span data-ttu-id="bbee1-103">更新 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="bbee1-103">Update userFlowLanguagePage</span></span>

<span data-ttu-id="bbee1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbee1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bbee1-105">更新 userFlowLanguagePage 对象中的值。</span><span class="sxs-lookup"><span data-stu-id="bbee1-105">Update the values in an userFlowLanguagePage object.</span></span> <span data-ttu-id="bbee1-106">只能更新 overridesPage 中的值，用于自定义在用户流定义的用户旅程期间向用户显示的值。</span><span class="sxs-lookup"><span data-stu-id="bbee1-106">You may only update the values in an overridesPage, which is used to customize the values shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbee1-107">权限</span><span class="sxs-lookup"><span data-stu-id="bbee1-107">Permissions</span></span>

<span data-ttu-id="bbee1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bbee1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbee1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbee1-110">Permission type</span></span>      | <span data-ttu-id="bbee1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bbee1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbee1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbee1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bbee1-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbee1-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="bbee1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbee1-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="bbee1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbee1-115">Not supported.</span></span>|
|<span data-ttu-id="bbee1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbee1-116">Application</span></span>|<span data-ttu-id="bbee1-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbee1-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="bbee1-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="bbee1-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="bbee1-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="bbee1-119">Global administrator</span></span>
* <span data-ttu-id="bbee1-120">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="bbee1-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="bbee1-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbee1-121">HTTP request</span></span>

<span data-ttu-id="bbee1-122">若要引用对象中的内容，必须使用 `$value` 。</span><span class="sxs-lookup"><span data-stu-id="bbee1-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="bbee1-123">这将返回 对象中的内容，并允许你直接引用它。</span><span class="sxs-lookup"><span data-stu-id="bbee1-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="bbee1-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbee1-124">Request headers</span></span>

|<span data-ttu-id="bbee1-125">名称</span><span class="sxs-lookup"><span data-stu-id="bbee1-125">Name</span></span>|<span data-ttu-id="bbee1-126">说明</span><span class="sxs-lookup"><span data-stu-id="bbee1-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bbee1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbee1-127">Authorization</span></span>|<span data-ttu-id="bbee1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bbee1-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bbee1-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bbee1-130">Content-Type</span></span>|<span data-ttu-id="bbee1-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bbee1-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbee1-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbee1-133">Request body</span></span>

<span data-ttu-id="bbee1-134">在请求正文中，提供 [userFlowLanguagePage](../resources/userflowlanguagepage.md)中包含的值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bbee1-134">In the request body, supply a JSON representation for the values contained within a [userFlowLanguagePage](../resources/userflowlanguagepage.md).</span></span>

## <a name="response"></a><span data-ttu-id="bbee1-135">响应</span><span class="sxs-lookup"><span data-stu-id="bbee1-135">Response</span></span>

<span data-ttu-id="bbee1-136">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bbee1-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bbee1-137">示例</span><span class="sxs-lookup"><span data-stu-id="bbee1-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bbee1-138">请求</span><span class="sxs-lookup"><span data-stu-id="bbee1-138">Request</span></span>

<span data-ttu-id="bbee1-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bbee1-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bbee1-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbee1-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_overridespages"
}
-->

``` http
PUT https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/languages/en/overridesPages/selfasserted1_1/$value
Content-Type: application/json

{
"LocalizedStrings": [
      {
          "ElementType": "UxElement",
          "ElementId": null,
          "StringId": "alert_message",
          "Override": true,
          "Value": "Are you sure that you want to cancel entering your information?"
      }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="bbee1-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbee1-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-overridespages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bbee1-142">响应</span><span class="sxs-lookup"><span data-stu-id="bbee1-142">Response</span></span>

<span data-ttu-id="bbee1-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bbee1-143">The following is an example of the response.</span></span>

<span data-ttu-id="bbee1-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bbee1-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
