---
title: 更新 adminConsentRequestPolicy
description: 更新 adminConsentRequestPolicy 对象的属性。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3fcd6bb895a4f1cb36f099269c8414669dc98620
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201455"
---
# <a name="update-adminconsentrequestpolicy"></a><span data-ttu-id="06681-103">更新 adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="06681-103">Update adminConsentRequestPolicy</span></span>
<span data-ttu-id="06681-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06681-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06681-105">更新 [adminConsentRequestPolicy 对象](../resources/adminconsentrequestpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="06681-105">Update the properties of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="06681-106">权限</span><span class="sxs-lookup"><span data-stu-id="06681-106">Permissions</span></span>
<span data-ttu-id="06681-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06681-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06681-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="06681-109">Permission type</span></span>|<span data-ttu-id="06681-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06681-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06681-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06681-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06681-112">Policy.ReadWrite.ConsentRequest</span><span class="sxs-lookup"><span data-stu-id="06681-112">Policy.ReadWrite.ConsentRequest</span></span>|
|<span data-ttu-id="06681-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06681-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06681-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="06681-114">Not supported.</span></span>|
|<span data-ttu-id="06681-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="06681-115">Application</span></span>|<span data-ttu-id="06681-116">Policy.ReadWrite.ConsentRequest</span><span class="sxs-lookup"><span data-stu-id="06681-116">Policy.ReadWrite.ConsentRequest</span></span>|

<span data-ttu-id="06681-117">代表用户进行呼叫时，用户需要属于全局 [管理员](/azure/active-directory/roles/permissions-reference) 目录角色。</span><span class="sxs-lookup"><span data-stu-id="06681-117">When calling on behalf of a user, the user needs to belong to the [Global Administrator](/azure/active-directory/roles/permissions-reference) directory role.</span></span>

## <a name="http-request"></a><span data-ttu-id="06681-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06681-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /policies/adminConsentRequestPolicy 
```

## <a name="request-headers"></a><span data-ttu-id="06681-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="06681-119">Request headers</span></span>
|<span data-ttu-id="06681-120">名称</span><span class="sxs-lookup"><span data-stu-id="06681-120">Name</span></span>|<span data-ttu-id="06681-121">说明</span><span class="sxs-lookup"><span data-stu-id="06681-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="06681-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="06681-122">Authorization</span></span>|<span data-ttu-id="06681-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="06681-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="06681-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06681-125">Content-Type</span></span>|<span data-ttu-id="06681-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="06681-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="06681-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="06681-128">Request body</span></span>
<span data-ttu-id="06681-129">在请求正文中，提供 [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06681-129">In the request body, supply a JSON representation of the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

<span data-ttu-id="06681-130">下表显示更新 [adminConsentRequestPolicy 时所需的属性](../resources/adminconsentrequestpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="06681-130">The following table shows the properties that are required when you update the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md).</span></span>

|<span data-ttu-id="06681-131">属性</span><span class="sxs-lookup"><span data-stu-id="06681-131">Property</span></span>|<span data-ttu-id="06681-132">类型</span><span class="sxs-lookup"><span data-stu-id="06681-132">Type</span></span>|<span data-ttu-id="06681-133">说明</span><span class="sxs-lookup"><span data-stu-id="06681-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06681-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="06681-134">isEnabled</span></span>|<span data-ttu-id="06681-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="06681-135">Boolean</span></span>|<span data-ttu-id="06681-136">指定是启用还是禁用管理员同意请求功能。</span><span class="sxs-lookup"><span data-stu-id="06681-136">Specifies whether the admin consent request feature is enabled or disabled.</span></span>|
|<span data-ttu-id="06681-137">notifyReviewers</span><span class="sxs-lookup"><span data-stu-id="06681-137">notifyReviewers</span></span>|<span data-ttu-id="06681-138">布尔值</span><span class="sxs-lookup"><span data-stu-id="06681-138">Boolean</span></span>|<span data-ttu-id="06681-139">指定审阅者是否将收到通知。</span><span class="sxs-lookup"><span data-stu-id="06681-139">Specifies whether reviewers will receive notifications.</span></span>|
|<span data-ttu-id="06681-140">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="06681-140">remindersEnabled</span></span>|<span data-ttu-id="06681-141">布尔值</span><span class="sxs-lookup"><span data-stu-id="06681-141">Boolean</span></span>|<span data-ttu-id="06681-142">指定审阅者是否将收到提醒电子邮件。</span><span class="sxs-lookup"><span data-stu-id="06681-142">Specifies whether reviewers will receive reminder emails.</span></span>|
|<span data-ttu-id="06681-143">requestDurationInDays</span><span class="sxs-lookup"><span data-stu-id="06681-143">requestDurationInDays</span></span>|<span data-ttu-id="06681-144">Int32</span><span class="sxs-lookup"><span data-stu-id="06681-144">Int32</span></span>|<span data-ttu-id="06681-145">指定请求在未应用决策时自动过期之前处于活动状态的持续时间。</span><span class="sxs-lookup"><span data-stu-id="06681-145">Specifies the duration the request is active before it automatically expires if no decision is applied.</span></span>|
|<span data-ttu-id="06681-146">reviewers</span><span class="sxs-lookup"><span data-stu-id="06681-146">reviewers</span></span>|<span data-ttu-id="06681-147">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06681-147">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="06681-148">管理员同意的审阅者列表。</span><span class="sxs-lookup"><span data-stu-id="06681-148">The list of reviewers for the admin consent.</span></span>|



## <a name="response"></a><span data-ttu-id="06681-149">响应</span><span class="sxs-lookup"><span data-stu-id="06681-149">Response</span></span>

<span data-ttu-id="06681-150">如果成功，此方法返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="06681-150">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="06681-151">示例</span><span class="sxs-lookup"><span data-stu-id="06681-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06681-152">请求</span><span class="sxs-lookup"><span data-stu-id="06681-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="06681-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="06681-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_adminconsentrequestpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/beta/policies/adminConsentRequestPolicy 
Content-Type: application/json

{
  "isEnabled": true,
  "notifyReviewers": true,
  "remindersEnabled": true,
  "requestDurationInDays": 5,
  "reviewers": [
    {
      "query": "/users/b6879be8-fb87-4482-a72e-18445d2b5c54",
      "queryType": "MicrosoftGraph"
    },
    {
      "query": "/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9",
      "queryType": "MicrosoftGraph"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="06681-154">C#</span><span class="sxs-lookup"><span data-stu-id="06681-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-adminconsentrequestpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06681-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06681-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-adminconsentrequestpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06681-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06681-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-adminconsentrequestpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06681-157">Java</span><span class="sxs-lookup"><span data-stu-id="06681-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-adminconsentrequestpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="06681-158">响应</span><span class="sxs-lookup"><span data-stu-id="06681-158">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: text/plain
```
