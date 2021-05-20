---
title: 获取 mobileAppManagementPolicy
description: 读取移动应用管理策略的属性和关系。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 062382f52f4efbd709a68f122a38a0ce0d4b5718
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547399"
---
# <a name="get-mobileappmanagementpolicy"></a><span data-ttu-id="200c7-103">获取 mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="200c7-103">Get mobileAppManagementPolicy</span></span>

<span data-ttu-id="200c7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="200c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="200c7-105">读取 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="200c7-105">Read the properties and relationships of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="200c7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="200c7-106">Permissions</span></span>

<span data-ttu-id="200c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="200c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="200c7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="200c7-109">Permission type</span></span>|<span data-ttu-id="200c7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="200c7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="200c7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="200c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="200c7-112">Policy.Read.All、Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="200c7-112">Policy.Read.All, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="200c7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="200c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="200c7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="200c7-114">Not supported.</span></span>|
|<span data-ttu-id="200c7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="200c7-115">Application</span></span> | <span data-ttu-id="200c7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="200c7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="200c7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="200c7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileAppManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="200c7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="200c7-118">Request headers</span></span>

|<span data-ttu-id="200c7-119">名称</span><span class="sxs-lookup"><span data-stu-id="200c7-119">Name</span></span>|<span data-ttu-id="200c7-120">说明</span><span class="sxs-lookup"><span data-stu-id="200c7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="200c7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="200c7-121">Authorization</span></span>|<span data-ttu-id="200c7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="200c7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="200c7-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="200c7-124">Request body</span></span>

<span data-ttu-id="200c7-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="200c7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="200c7-126">响应</span><span class="sxs-lookup"><span data-stu-id="200c7-126">Response</span></span>

<span data-ttu-id="200c7-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="200c7-127">If successful, this method returns a `200 OK` response code and a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="200c7-128">示例</span><span class="sxs-lookup"><span data-stu-id="200c7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="200c7-129">请求</span><span class="sxs-lookup"><span data-stu-id="200c7-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mobilitymanagementpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
```

### <a name="response"></a><span data-ttu-id="200c7-130">响应</span><span class="sxs-lookup"><span data-stu-id="200c7-130">Response</span></span>

><span data-ttu-id="200c7-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="200c7-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
