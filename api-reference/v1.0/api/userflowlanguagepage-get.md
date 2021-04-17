---
title: 获取 userFlowLanguagePage
description: 读取用户流中某种语言的 userFlowLanguagePage 对象中的值。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5b1edf34635e94a3bb45500df34309c7ba1fac59
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882978"
---
# <a name="get-userflowlanguagepage"></a><span data-ttu-id="5e4dc-103">获取 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="5e4dc-103">Get userFlowLanguagePage</span></span>

<span data-ttu-id="5e4dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e4dc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5e4dc-105">读取用户流中某种语言的 [userFlowLanguagePage](../resources/userflowlanguagepage.md) 对象中的值。</span><span class="sxs-lookup"><span data-stu-id="5e4dc-105">Read the values in a [userFlowLanguagePage](../resources/userflowlanguagepage.md) object for a language in a user flow.</span></span> <span data-ttu-id="5e4dc-106">这些值在用户流定义的用户旅程中向用户显示。</span><span class="sxs-lookup"><span data-stu-id="5e4dc-106">These values are shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e4dc-107">权限</span><span class="sxs-lookup"><span data-stu-id="5e4dc-107">Permissions</span></span>

<span data-ttu-id="5e4dc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e4dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e4dc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e4dc-110">Permission type</span></span>      | <span data-ttu-id="5e4dc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e4dc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e4dc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e4dc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e4dc-113">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e4dc-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="5e4dc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e4dc-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5e4dc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e4dc-115">Not supported.</span></span>|
|<span data-ttu-id="5e4dc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e4dc-116">Application</span></span>|<span data-ttu-id="5e4dc-117">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e4dc-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="5e4dc-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="5e4dc-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="5e4dc-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="5e4dc-119">Global administrator</span></span>
* <span data-ttu-id="5e4dc-120">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="5e4dc-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="5e4dc-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e4dc-121">HTTP request</span></span>

<span data-ttu-id="5e4dc-122">若要引用对象中的内容，必须使用 `$value` 。</span><span class="sxs-lookup"><span data-stu-id="5e4dc-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="5e4dc-123">这将返回 对象中的内容，并允许你直接引用它。</span><span class="sxs-lookup"><span data-stu-id="5e4dc-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages/{id}/defaultPages/{id}/$value
GET /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="5e4dc-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e4dc-124">Request headers</span></span>

|<span data-ttu-id="5e4dc-125">名称</span><span class="sxs-lookup"><span data-stu-id="5e4dc-125">Name</span></span>|<span data-ttu-id="5e4dc-126">说明</span><span class="sxs-lookup"><span data-stu-id="5e4dc-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5e4dc-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e4dc-127">Authorization</span></span>|<span data-ttu-id="5e4dc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e4dc-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e4dc-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e4dc-130">Request body</span></span>

<span data-ttu-id="5e4dc-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5e4dc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e4dc-132">响应</span><span class="sxs-lookup"><span data-stu-id="5e4dc-132">Response</span></span>

<span data-ttu-id="5e4dc-133">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [userFlowLanguagePage](../resources/userflowlanguagepage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5e4dc-133">If successful, this method returns a `200 OK` response code and a [userFlowLanguagePage](../resources/userflowlanguagepage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5e4dc-134">示例</span><span class="sxs-lookup"><span data-stu-id="5e4dc-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5e4dc-135">请求</span><span class="sxs-lookup"><span data-stu-id="5e4dc-135">Request</span></span>

<span data-ttu-id="5e4dc-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5e4dc-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/languages/en/defaultPages/idpselections/$value
```

### <a name="response"></a><span data-ttu-id="5e4dc-137">响应</span><span class="sxs-lookup"><span data-stu-id="5e4dc-137">Response</span></span>

<span data-ttu-id="5e4dc-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5e4dc-138">The following is an example of the response.</span></span>

<span data-ttu-id="5e4dc-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5e4dc-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguagePage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "LocalizedStrings": [
      {
        "ElementType": "ErrorMessage",
        "ElementId": null,
        "StringId": "ServiceThrottled",
        "Override": false,
        "Value": "There are too many requests at this moment. Please wait for some time and try again."
      }
   ]
}
```
