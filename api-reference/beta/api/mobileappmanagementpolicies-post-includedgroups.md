---
title: 添加 includedGroups
description: 添加要包含在移动应用管理策略中的组。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 23612a1aaa10c1a51af54dd184f6a7ea8497dd2d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440470"
---
# <a name="add-includedgroups"></a><span data-ttu-id="45614-103">添加 includedGroups</span><span class="sxs-lookup"><span data-stu-id="45614-103">Add includedGroups</span></span>

<span data-ttu-id="45614-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45614-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45614-105">添加要包含在移动应用管理策略中的组。</span><span class="sxs-lookup"><span data-stu-id="45614-105">Add groups to be included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="45614-106">权限</span><span class="sxs-lookup"><span data-stu-id="45614-106">Permissions</span></span>
<span data-ttu-id="45614-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45614-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45614-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="45614-109">Permission type</span></span>|<span data-ttu-id="45614-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45614-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45614-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45614-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45614-112">Policy.Read.All、Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="45614-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="45614-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45614-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45614-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="45614-114">Not supported.</span></span>|
|<span data-ttu-id="45614-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="45614-115">Application</span></span> | <span data-ttu-id="45614-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="45614-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45614-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45614-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /policies/mobileAppManagementPolicies/{id}/includedGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="45614-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="45614-118">Request headers</span></span>
|<span data-ttu-id="45614-119">名称</span><span class="sxs-lookup"><span data-stu-id="45614-119">Name</span></span>|<span data-ttu-id="45614-120">说明</span><span class="sxs-lookup"><span data-stu-id="45614-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="45614-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="45614-121">Authorization</span></span>|<span data-ttu-id="45614-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="45614-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="45614-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="45614-124">Content-Type</span></span>|<span data-ttu-id="45614-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="45614-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45614-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="45614-127">Request body</span></span>
<span data-ttu-id="45614-128">在请求正文中，提供 group 对象的 JSON [表示](../resources/group.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="45614-128">In the request body, supply a JSON representation of the [group](../resources/group.md) object.</span></span>

<span data-ttu-id="45614-129">下表显示添加组 时所需的 [属性](../resources/group.md)。</span><span class="sxs-lookup"><span data-stu-id="45614-129">The following table shows the properties that are required when you add the [group](../resources/group.md).</span></span>

|<span data-ttu-id="45614-130">属性</span><span class="sxs-lookup"><span data-stu-id="45614-130">Property</span></span>|<span data-ttu-id="45614-131">类型</span><span class="sxs-lookup"><span data-stu-id="45614-131">Type</span></span>|<span data-ttu-id="45614-132">说明</span><span class="sxs-lookup"><span data-stu-id="45614-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45614-133">id</span><span class="sxs-lookup"><span data-stu-id="45614-133">id</span></span>|<span data-ttu-id="45614-134">String</span><span class="sxs-lookup"><span data-stu-id="45614-134">String</span></span>|<span data-ttu-id="45614-135">组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="45614-135">The unique identifier for the group.</span></span>|

## <a name="response"></a><span data-ttu-id="45614-136">响应</span><span class="sxs-lookup"><span data-stu-id="45614-136">Response</span></span>

<span data-ttu-id="45614-137">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45614-137">If successful, this method returns a `204 No Content` response code and a [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45614-138">示例</span><span class="sxs-lookup"><span data-stu-id="45614-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45614-139">请求</span><span class="sxs-lookup"><span data-stu-id="45614-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="45614-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="45614-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
}
-->

``` http
POST https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/$ref
Content-Type: application/json

{
  "@odata.id": "https://graph.microsoft.com/odata/groups('1a9db3ab-0acf-4808-99ae-e8ed581cb2e0')"
}
```
# <a name="c"></a>[<span data-ttu-id="45614-141">C#</span><span class="sxs-lookup"><span data-stu-id="45614-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-from-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45614-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45614-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-from-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45614-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45614-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-from-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45614-144">Java</span><span class="sxs-lookup"><span data-stu-id="45614-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-from-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="45614-145">响应</span><span class="sxs-lookup"><span data-stu-id="45614-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
