---
title: 创建 authenticationListener
description: 为 onSignUpStart 事件创建新的 authenticationListener 对象。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 098a8679f09c7f766b361146abddc0d01a5aa20e
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872357"
---
# <a name="create-authenticationlistener"></a><span data-ttu-id="e638a-103">创建 authenticationListener</span><span class="sxs-lookup"><span data-stu-id="e638a-103">Create authenticationListener</span></span>

<span data-ttu-id="e638a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e638a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e638a-105">为 onSignUpStart 事件创建新的 authenticationListener 对象。</span><span class="sxs-lookup"><span data-stu-id="e638a-105">Create a new authenticationListener object for the onSignUpStart event.</span></span>

## <a name="permissions"></a><span data-ttu-id="e638a-106">权限</span><span class="sxs-lookup"><span data-stu-id="e638a-106">Permissions</span></span>

<span data-ttu-id="e638a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e638a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e638a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e638a-109">Permission type</span></span>|<span data-ttu-id="e638a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e638a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e638a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e638a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e638a-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="e638a-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="e638a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e638a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e638a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e638a-114">Not supported.</span></span>|
|<span data-ttu-id="e638a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e638a-115">Application</span></span>|<span data-ttu-id="e638a-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="e638a-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="e638a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e638a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/events/onSignupStart
```

## <a name="request-headers"></a><span data-ttu-id="e638a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e638a-118">Request headers</span></span>

|<span data-ttu-id="e638a-119">名称</span><span class="sxs-lookup"><span data-stu-id="e638a-119">Name</span></span>|<span data-ttu-id="e638a-120">说明</span><span class="sxs-lookup"><span data-stu-id="e638a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e638a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e638a-121">Authorization</span></span>|<span data-ttu-id="e638a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e638a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e638a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e638a-124">Content-Type</span></span>|<span data-ttu-id="e638a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e638a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e638a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e638a-127">Request body</span></span>

<span data-ttu-id="e638a-128">在请求正文中，提供 [authenticationListener](../resources/authenticationlistener.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e638a-128">In the request body, supply a JSON representation of the [authenticationListener](../resources/authenticationlistener.md) object.</span></span>

<span data-ttu-id="e638a-129">下表显示创建 [invokeUserFlowListener authenticationListener](../resources/invokeuserflowlistener.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e638a-129">The following table shows the properties that are required when you create the [invokeUserFlowListener](../resources/invokeuserflowlistener.md) authenticationListener.</span></span>

|<span data-ttu-id="e638a-130">属性</span><span class="sxs-lookup"><span data-stu-id="e638a-130">Property</span></span>|<span data-ttu-id="e638a-131">类型</span><span class="sxs-lookup"><span data-stu-id="e638a-131">Type</span></span>|<span data-ttu-id="e638a-132">Description</span><span class="sxs-lookup"><span data-stu-id="e638a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e638a-133">priority</span><span class="sxs-lookup"><span data-stu-id="e638a-133">priority</span></span>|<span data-ttu-id="e638a-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e638a-134">Int32</span></span>|<span data-ttu-id="e638a-135">侦听器的优先级。</span><span class="sxs-lookup"><span data-stu-id="e638a-135">The priority of the listener.</span></span> <span data-ttu-id="e638a-136">确定事件具有多个侦听器时的评估顺序。</span><span class="sxs-lookup"><span data-stu-id="e638a-136">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="e638a-137">优先级从低到高计算。</span><span class="sxs-lookup"><span data-stu-id="e638a-137">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="e638a-138">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="e638a-138">sourceFilter</span></span>|[<span data-ttu-id="e638a-139">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="e638a-139">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="e638a-140">基于用于确定是否评估侦听器的身份验证源进行筛选。</span><span class="sxs-lookup"><span data-stu-id="e638a-140">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="e638a-141">当前仅限于基于用户进行身份验证的应用程序的评估。</span><span class="sxs-lookup"><span data-stu-id="e638a-141">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|
|<span data-ttu-id="e638a-142">userFlow</span><span class="sxs-lookup"><span data-stu-id="e638a-142">userFlow</span></span>|[<span data-ttu-id="e638a-143">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="e638a-143">b2xIdentityUserFlow</span></span>](../resources/b2xidentityuserflow.md)|<span data-ttu-id="e638a-144">计算此操作时将调用的 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e638a-144">The [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object that will be invoked when this action is evaluated.</span></span>|

## <a name="response"></a><span data-ttu-id="e638a-145">响应</span><span class="sxs-lookup"><span data-stu-id="e638a-145">Response</span></span>

<span data-ttu-id="e638a-146">如果成功，此方法在响应正文中返回响应 `201 Created` 代码和 [authenticationListener](../resources/authenticationlistener.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e638a-146">If successful, this method returns a `201 Created` response code and an [authenticationListener](../resources/authenticationlistener.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e638a-147">示例</span><span class="sxs-lookup"><span data-stu-id="e638a-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e638a-148">请求</span><span class="sxs-lookup"><span data-stu-id="e638a-148">Request</span></span>

<span data-ttu-id="e638a-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e638a-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_authenticationlistener_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/events/onSignupStart
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.invokeUserFlowListener",
    "priority": 101,
    "sourceFilter": {
        "includeApplications": [
            "1fc41a76-3050-4529-8095-9af8897cf63d"
        ]
    },
    "userFlow": {
        "id": "B2X_1_Partner"
    }
}
```

### <a name="response"></a><span data-ttu-id="e638a-150">响应</span><span class="sxs-lookup"><span data-stu-id="e638a-150">Response</span></span>

<span data-ttu-id="e638a-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e638a-151">The following is an example of the response.</span></span>

<span data-ttu-id="e638a-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e638a-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationListener"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/events/onSignupStart/Microsoft.Graph.InvokeUserFlowListener/$entity",
    "@odata.type": "#microsoft.graph.invokeUserFlowListener",
    "id": "2be3336b-e3b4-44f3-9128-b6fd9ad39bb8",
    "priority": 101,
    "sourceFilter": {
        "includeApplications": [
            "1fc41a76-3050-4529-8095-9af8897cf63d"
        ]
    }
}
```
