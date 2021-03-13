---
title: identityUserFlowAttributeAssignment： getOrder
description: 获取在用户流中收集的 identityUserFlowAttributeAssignments 的顺序。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 93308846ecf1549efd70ebe8fc4b2915626d7b81
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759956"
---
# <a name="identityuserflowattributeassignment-getorder"></a><span data-ttu-id="5f9ec-103">identityUserFlowAttributeAssignment： getOrder</span><span class="sxs-lookup"><span data-stu-id="5f9ec-103">identityUserFlowAttributeAssignment: getOrder</span></span>

<span data-ttu-id="5f9ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f9ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f9ec-105">获取在用户流中收集的 identityUserFlowAttributeAssignments 的顺序。</span><span class="sxs-lookup"><span data-stu-id="5f9ec-105">Get the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f9ec-106">权限</span><span class="sxs-lookup"><span data-stu-id="5f9ec-106">Permissions</span></span>

<span data-ttu-id="5f9ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f9ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f9ec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f9ec-109">Permission type</span></span>|<span data-ttu-id="5f9ec-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f9ec-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f9ec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f9ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5f9ec-112">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f9ec-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="5f9ec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f9ec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f9ec-114">不支持</span><span class="sxs-lookup"><span data-stu-id="5f9ec-114">Not supported</span></span>|
|<span data-ttu-id="5f9ec-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f9ec-115">Application</span></span>|<span data-ttu-id="5f9ec-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f9ec-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f9ec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f9ec-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/getOrder
GET /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/getOrder
```

## <a name="request-headers"></a><span data-ttu-id="5f9ec-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f9ec-118">Request headers</span></span>

|<span data-ttu-id="5f9ec-119">名称</span><span class="sxs-lookup"><span data-stu-id="5f9ec-119">Name</span></span>|<span data-ttu-id="5f9ec-120">说明</span><span class="sxs-lookup"><span data-stu-id="5f9ec-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5f9ec-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f9ec-121">Authorization</span></span>|<span data-ttu-id="5f9ec-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f9ec-p102">Bearer {token}. Required.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="5f9ec-124">函数参数</span><span class="sxs-lookup"><span data-stu-id="5f9ec-124">Function parameters</span></span>

<span data-ttu-id="5f9ec-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5f9ec-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f9ec-126">响应</span><span class="sxs-lookup"><span data-stu-id="5f9ec-126">Response</span></span>

<span data-ttu-id="5f9ec-127">如果成功，此函数在响应 `200 OK` 正文中返回 响应代码和[assignmentOrder。](../resources/assignmentorder.md)</span><span class="sxs-lookup"><span data-stu-id="5f9ec-127">If successful, this function returns a `200 OK` response code and a [assignmentOrder](../resources/assignmentorder.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f9ec-128">示例</span><span class="sxs-lookup"><span data-stu-id="5f9ec-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f9ec-129">请求</span><span class="sxs-lookup"><span data-stu-id="5f9ec-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5f9ec-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f9ec-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_getorder"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/getOrder
```
# <a name="c"></a>[<span data-ttu-id="5f9ec-131">C#</span><span class="sxs-lookup"><span data-stu-id="5f9ec-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityuserflowattributeassignment-getorder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f9ec-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f9ec-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityuserflowattributeassignment-getorder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f9ec-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f9ec-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityuserflowattributeassignment-getorder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f9ec-134">Java</span><span class="sxs-lookup"><span data-stu-id="5f9ec-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityuserflowattributeassignment-getorder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5f9ec-135">响应</span><span class="sxs-lookup"><span data-stu-id="5f9ec-135">Response</span></span>

<span data-ttu-id="5f9ec-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5f9ec-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.assignmentOrder"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta$metadata#microsoft.graph.assignmentOrder",
    "order": [
        "extension_GUID_ShoeSize",
        "City"
    ]
}
```
