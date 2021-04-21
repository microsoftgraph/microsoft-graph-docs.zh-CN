---
title: 获取 userFlowLanguageConfiguration
description: 读取 userFlowLanguageConfiguration 对象的属性和关系。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a2f17c309e104738a1bae4fd7e599fd8efa28355
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920571"
---
# <a name="get-userflowlanguageconfiguration"></a><span data-ttu-id="b9700-103">获取 userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9700-103">Get userFlowLanguageConfiguration</span></span>

<span data-ttu-id="b9700-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9700-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9700-105">读取 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b9700-105">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="b9700-106">这些对象表示用户流中可用的语言。</span><span class="sxs-lookup"><span data-stu-id="b9700-106">These objects represent a language available in a user flow.</span></span>

<span data-ttu-id="b9700-107">**注意：** 默认情况下，在 Azure Active Directory 用户流 [中启用语言自定义](../resources/b2xidentityuserflow.md)。</span><span class="sxs-lookup"><span data-stu-id="b9700-107">**Note:** Language customization is enabled by default in [Azure Active Directory user flows](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b9700-108">权限</span><span class="sxs-lookup"><span data-stu-id="b9700-108">Permissions</span></span>

<span data-ttu-id="b9700-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9700-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9700-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9700-111">Permission type</span></span>      | <span data-ttu-id="b9700-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9700-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9700-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9700-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9700-114">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9700-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="b9700-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9700-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b9700-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9700-116">Not supported.</span></span>|
|<span data-ttu-id="b9700-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9700-117">Application</span></span>|<span data-ttu-id="b9700-118">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9700-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="b9700-119">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="b9700-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="b9700-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="b9700-120">Global administrator</span></span>
* <span data-ttu-id="b9700-121">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="b9700-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="b9700-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9700-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2xUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b9700-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9700-123">Request headers</span></span>

|<span data-ttu-id="b9700-124">名称</span><span class="sxs-lookup"><span data-stu-id="b9700-124">Name</span></span>|<span data-ttu-id="b9700-125">说明</span><span class="sxs-lookup"><span data-stu-id="b9700-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b9700-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9700-126">Authorization</span></span>|<span data-ttu-id="b9700-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9700-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9700-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9700-129">Request body</span></span>

<span data-ttu-id="b9700-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b9700-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9700-131">响应</span><span class="sxs-lookup"><span data-stu-id="b9700-131">Response</span></span>

<span data-ttu-id="b9700-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9700-132">If successful, this method returns a `200 OK` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9700-133">示例</span><span class="sxs-lookup"><span data-stu-id="b9700-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9700-134">请求</span><span class="sxs-lookup"><span data-stu-id="b9700-134">Request</span></span>

<span data-ttu-id="b9700-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b9700-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b9700-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9700-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/languages/en
```
# <a name="c"></a>[<span data-ttu-id="b9700-137">C#</span><span class="sxs-lookup"><span data-stu-id="b9700-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9700-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9700-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9700-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9700-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9700-140">Java</span><span class="sxs-lookup"><span data-stu-id="b9700-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b9700-141">响应</span><span class="sxs-lookup"><span data-stu-id="b9700-141">Response</span></span>

<span data-ttu-id="b9700-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b9700-142">The following is an example of the response.</span></span>

<span data-ttu-id="b9700-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b9700-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_Partner')/languages/$entity",
    "id": "en",
    "isEnabled": true,
    "displayName": "English"
  }
}
```
