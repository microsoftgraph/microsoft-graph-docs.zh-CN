---
title: 获取 mobileAppManagementPolicy
description: 读取移动应用管理策略的属性和关系。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1e1e9bbd73ce8ac255673bc111e19fde3c69eb39
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442421"
---
# <a name="get-mobileappmanagementpolicy"></a><span data-ttu-id="8ad65-103">获取 mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8ad65-103">Get mobileAppManagementPolicy</span></span>

<span data-ttu-id="8ad65-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ad65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ad65-105">读取 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8ad65-105">Read the properties and relationships of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ad65-106">权限</span><span class="sxs-lookup"><span data-stu-id="8ad65-106">Permissions</span></span>

<span data-ttu-id="8ad65-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ad65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ad65-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ad65-109">Permission type</span></span>|<span data-ttu-id="8ad65-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ad65-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ad65-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ad65-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8ad65-112">Policy.Read.All、Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="8ad65-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="8ad65-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ad65-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ad65-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ad65-114">Not supported.</span></span>|
|<span data-ttu-id="8ad65-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ad65-115">Application</span></span> | <span data-ttu-id="8ad65-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ad65-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ad65-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ad65-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileAppManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8ad65-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ad65-118">Request headers</span></span>

|<span data-ttu-id="8ad65-119">名称</span><span class="sxs-lookup"><span data-stu-id="8ad65-119">Name</span></span>|<span data-ttu-id="8ad65-120">说明</span><span class="sxs-lookup"><span data-stu-id="8ad65-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8ad65-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ad65-121">Authorization</span></span>|<span data-ttu-id="8ad65-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ad65-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ad65-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ad65-124">Request body</span></span>

<span data-ttu-id="8ad65-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8ad65-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ad65-126">响应</span><span class="sxs-lookup"><span data-stu-id="8ad65-126">Response</span></span>

<span data-ttu-id="8ad65-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ad65-127">If successful, this method returns a `200 OK` response code and a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ad65-128">示例</span><span class="sxs-lookup"><span data-stu-id="8ad65-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8ad65-129">请求</span><span class="sxs-lookup"><span data-stu-id="8ad65-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8ad65-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ad65-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mobilitymanagementpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
```
# <a name="c"></a>[<span data-ttu-id="8ad65-131">C#</span><span class="sxs-lookup"><span data-stu-id="8ad65-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mobilitymanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ad65-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ad65-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mobilitymanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ad65-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ad65-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mobilitymanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8ad65-134">Java</span><span class="sxs-lookup"><span data-stu-id="8ad65-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mobilitymanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8ad65-135">响应</span><span class="sxs-lookup"><span data-stu-id="8ad65-135">Response</span></span>

><span data-ttu-id="8ad65-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8ad65-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobilityManagementPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "ab90bacf-55a3-4a3e-839a-aa4b74e4f020",
    "appliesTo": "selected",
    "complianceUrl": "https://portal.mam.contoso.com/?portalAction=Compliance",
    "description": "Contoso mobilty app is a cloud-based  Endpoint Management solution for managing Windows.",
    "discoveryUrl": "https://enrollment.mam.contoso.com/enrollmentserver/discovery.svc",
    "displayName": "Contoso mobilty app",
    "termsOfUseUrl": "https://portal.mam.contoso.com/TermsofUse.aspx",
    "includedGroups": [
      {
        "id": "800c583d-cc3d-4361-8e4a-3fbf668f27f4",
        "displayName": "Test Group"
      }
    ]
  }
}
```
