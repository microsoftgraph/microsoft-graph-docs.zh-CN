---
title: 更新 adminConsentRequestPolicy
description: 更新 adminConsentRequestPolicy 对象的属性。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1c0769262cc17e79448ca856e26334d4c03d92a1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952213"
---
# <a name="update-adminconsentrequestpolicy"></a><span data-ttu-id="7dde2-103">更新 adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="7dde2-103">Update adminConsentRequestPolicy</span></span>
<span data-ttu-id="7dde2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dde2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dde2-105">更新 [adminConsentRequestPolicy 对象](../resources/adminconsentrequestpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="7dde2-105">Update the properties of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dde2-106">权限</span><span class="sxs-lookup"><span data-stu-id="7dde2-106">Permissions</span></span>
<span data-ttu-id="7dde2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7dde2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dde2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7dde2-109">Permission type</span></span>|<span data-ttu-id="7dde2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7dde2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dde2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7dde2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7dde2-112">Policy.ReadWrite.ConsentRequest</span><span class="sxs-lookup"><span data-stu-id="7dde2-112">Policy.ReadWrite.ConsentRequest</span></span>|
|<span data-ttu-id="7dde2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7dde2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dde2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dde2-114">Not supported.</span></span>|
|<span data-ttu-id="7dde2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7dde2-115">Application</span></span>|<span data-ttu-id="7dde2-116">Policy.ReadWrite.ConsentRequest</span><span class="sxs-lookup"><span data-stu-id="7dde2-116">Policy.ReadWrite.ConsentRequest</span></span>|

<span data-ttu-id="7dde2-117">代表用户进行呼叫时，用户需要属于全局 [管理员](/azure/active-directory/roles/permissions-reference) 目录角色。</span><span class="sxs-lookup"><span data-stu-id="7dde2-117">When calling on behalf of a user, the user needs to belong to the [Global Administrator](/azure/active-directory/roles/permissions-reference) directory role.</span></span>

## <a name="http-request"></a><span data-ttu-id="7dde2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7dde2-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /policies/adminConsentRequestPolicy 
```

## <a name="request-headers"></a><span data-ttu-id="7dde2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7dde2-119">Request headers</span></span>
|<span data-ttu-id="7dde2-120">名称</span><span class="sxs-lookup"><span data-stu-id="7dde2-120">Name</span></span>|<span data-ttu-id="7dde2-121">说明</span><span class="sxs-lookup"><span data-stu-id="7dde2-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7dde2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dde2-122">Authorization</span></span>|<span data-ttu-id="7dde2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7dde2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7dde2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7dde2-125">Content-Type</span></span>|<span data-ttu-id="7dde2-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7dde2-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dde2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7dde2-128">Request body</span></span>
<span data-ttu-id="7dde2-129">在请求正文中，提供 [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7dde2-129">In the request body, supply a JSON representation of the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

<span data-ttu-id="7dde2-130">下表显示更新 [adminConsentRequestPolicy 时所需的属性](../resources/adminconsentrequestpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="7dde2-130">The following table shows the properties that are required when you update the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md).</span></span>

|<span data-ttu-id="7dde2-131">属性</span><span class="sxs-lookup"><span data-stu-id="7dde2-131">Property</span></span>|<span data-ttu-id="7dde2-132">类型</span><span class="sxs-lookup"><span data-stu-id="7dde2-132">Type</span></span>|<span data-ttu-id="7dde2-133">说明</span><span class="sxs-lookup"><span data-stu-id="7dde2-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dde2-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7dde2-134">isEnabled</span></span>|<span data-ttu-id="7dde2-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dde2-135">Boolean</span></span>|<span data-ttu-id="7dde2-136">指定是启用还是禁用管理员同意请求功能。</span><span class="sxs-lookup"><span data-stu-id="7dde2-136">Specifies whether the admin consent request feature is enabled or disabled.</span></span>|
|<span data-ttu-id="7dde2-137">notifyReviewers</span><span class="sxs-lookup"><span data-stu-id="7dde2-137">notifyReviewers</span></span>|<span data-ttu-id="7dde2-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dde2-138">Boolean</span></span>|<span data-ttu-id="7dde2-139">指定审阅者是否将收到通知。</span><span class="sxs-lookup"><span data-stu-id="7dde2-139">Specifies whether reviewers will receive notifications.</span></span>|
|<span data-ttu-id="7dde2-140">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="7dde2-140">remindersEnabled</span></span>|<span data-ttu-id="7dde2-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dde2-141">Boolean</span></span>|<span data-ttu-id="7dde2-142">指定审阅者是否将收到提醒电子邮件。</span><span class="sxs-lookup"><span data-stu-id="7dde2-142">Specifies whether reviewers will receive reminder emails.</span></span>|
|<span data-ttu-id="7dde2-143">requestDurationInDays</span><span class="sxs-lookup"><span data-stu-id="7dde2-143">requestDurationInDays</span></span>|<span data-ttu-id="7dde2-144">Int32</span><span class="sxs-lookup"><span data-stu-id="7dde2-144">Int32</span></span>|<span data-ttu-id="7dde2-145">指定请求在未应用决策时自动过期之前处于活动状态的持续时间。</span><span class="sxs-lookup"><span data-stu-id="7dde2-145">Specifies the duration the request is active before it automatically expires if no decision is applied.</span></span>|
|<span data-ttu-id="7dde2-146">reviewers</span><span class="sxs-lookup"><span data-stu-id="7dde2-146">reviewers</span></span>|<span data-ttu-id="7dde2-147">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7dde2-147">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="7dde2-148">管理员同意的审阅者列表。</span><span class="sxs-lookup"><span data-stu-id="7dde2-148">The list of reviewers for the admin consent.</span></span>|



## <a name="response"></a><span data-ttu-id="7dde2-149">响应</span><span class="sxs-lookup"><span data-stu-id="7dde2-149">Response</span></span>

<span data-ttu-id="7dde2-150">如果成功，此方法返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7dde2-150">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7dde2-151">示例</span><span class="sxs-lookup"><span data-stu-id="7dde2-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7dde2-152">请求</span><span class="sxs-lookup"><span data-stu-id="7dde2-152">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="7dde2-153">响应</span><span class="sxs-lookup"><span data-stu-id="7dde2-153">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: text/plain
```
