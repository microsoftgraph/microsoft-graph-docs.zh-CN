---
title: 'identityUserFlowAttributeAssignment: getOrder'
description: 获取在用户流中收集的 identityUserFlowAttributeAssignments 的顺序。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 653a1e83ee96418dc70129790f62ea764e6326f9
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581328"
---
# <a name="identityuserflowattributeassignment-getorder"></a><span data-ttu-id="1696c-103">identityUserFlowAttributeAssignment: getOrder</span><span class="sxs-lookup"><span data-stu-id="1696c-103">identityUserFlowAttributeAssignment: getOrder</span></span>

<span data-ttu-id="1696c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1696c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1696c-105">获取在用户流中收集的 identityUserFlowAttributeAssignments 的顺序。</span><span class="sxs-lookup"><span data-stu-id="1696c-105">Get the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="1696c-106">权限</span><span class="sxs-lookup"><span data-stu-id="1696c-106">Permissions</span></span>

<span data-ttu-id="1696c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1696c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1696c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1696c-109">Permission type</span></span>|<span data-ttu-id="1696c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1696c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1696c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1696c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1696c-112">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="1696c-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="1696c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1696c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1696c-114">不支持</span><span class="sxs-lookup"><span data-stu-id="1696c-114">Not supported</span></span>|
|<span data-ttu-id="1696c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1696c-115">Application</span></span>|<span data-ttu-id="1696c-116">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="1696c-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1696c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1696c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/getOrder
GET /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/getOrder
```

## <a name="request-headers"></a><span data-ttu-id="1696c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1696c-118">Request headers</span></span>

|<span data-ttu-id="1696c-119">名称</span><span class="sxs-lookup"><span data-stu-id="1696c-119">Name</span></span>|<span data-ttu-id="1696c-120">说明</span><span class="sxs-lookup"><span data-stu-id="1696c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1696c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1696c-121">Authorization</span></span>|<span data-ttu-id="1696c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1696c-p102">Bearer {token}. Required.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="1696c-124">函数参数</span><span class="sxs-lookup"><span data-stu-id="1696c-124">Function parameters</span></span>

<span data-ttu-id="1696c-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1696c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1696c-126">响应</span><span class="sxs-lookup"><span data-stu-id="1696c-126">Response</span></span>

<span data-ttu-id="1696c-127">如果成功，此函数会 `200 OK` 在响应正文中返回响应代码和 [assignmentOrder](../resources/assignmentorder.md) 。</span><span class="sxs-lookup"><span data-stu-id="1696c-127">If successful, this function returns a `200 OK` response code and a [assignmentOrder](../resources/assignmentorder.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1696c-128">示例</span><span class="sxs-lookup"><span data-stu-id="1696c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1696c-129">请求</span><span class="sxs-lookup"><span data-stu-id="1696c-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_getorder"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/getOrder
```

### <a name="response"></a><span data-ttu-id="1696c-130">响应</span><span class="sxs-lookup"><span data-stu-id="1696c-130">Response</span></span>

<span data-ttu-id="1696c-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1696c-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
