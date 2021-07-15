---
title: 列出 includedGroups
description: 获取包含在移动设备管理策略中的组列表。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9cdb9724c19fbf8af2fa15e86c29fee11632ec72
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441028"
---
# <a name="list-includedgroups"></a><span data-ttu-id="89e9c-103">列出 includedGroups</span><span class="sxs-lookup"><span data-stu-id="89e9c-103">List includedGroups</span></span>

<span data-ttu-id="89e9c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89e9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89e9c-105">获取包含在移动设备管理策略中的组列表。</span><span class="sxs-lookup"><span data-stu-id="89e9c-105">Get the list of groups that are included in a mobile device management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="89e9c-106">权限</span><span class="sxs-lookup"><span data-stu-id="89e9c-106">Permissions</span></span>

<span data-ttu-id="89e9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89e9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89e9c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="89e9c-109">Permission type</span></span>|<span data-ttu-id="89e9c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89e9c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89e9c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89e9c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89e9c-112">Policy.Read.All、Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="89e9c-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="89e9c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89e9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89e9c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="89e9c-114">Not supported.</span></span>|
|<span data-ttu-id="89e9c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="89e9c-115">Application</span></span> | <span data-ttu-id="89e9c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="89e9c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89e9c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89e9c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileDeviceManagementPolicies/{id}/includedGroups
```

## <a name="request-headers"></a><span data-ttu-id="89e9c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="89e9c-118">Request headers</span></span>

|<span data-ttu-id="89e9c-119">名称</span><span class="sxs-lookup"><span data-stu-id="89e9c-119">Name</span></span>|<span data-ttu-id="89e9c-120">说明</span><span class="sxs-lookup"><span data-stu-id="89e9c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="89e9c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="89e9c-121">Authorization</span></span>|<span data-ttu-id="89e9c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89e9c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89e9c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="89e9c-124">Request body</span></span>

<span data-ttu-id="89e9c-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="89e9c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89e9c-126">响应</span><span class="sxs-lookup"><span data-stu-id="89e9c-126">Response</span></span>

<span data-ttu-id="89e9c-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="89e9c-127">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89e9c-128">示例</span><span class="sxs-lookup"><span data-stu-id="89e9c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89e9c-129">请求</span><span class="sxs-lookup"><span data-stu-id="89e9c-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="89e9c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="89e9c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups
```
# <a name="c"></a>[<span data-ttu-id="89e9c-131">C#</span><span class="sxs-lookup"><span data-stu-id="89e9c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89e9c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89e9c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89e9c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89e9c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89e9c-134">Java</span><span class="sxs-lookup"><span data-stu-id="89e9c-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89e9c-135">响应</span><span class="sxs-lookup"><span data-stu-id="89e9c-135">Response</span></span>

><span data-ttu-id="89e9c-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="89e9c-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.group)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef",
      "displayName": "Test MDM Group"
    }
  ]
}
```
