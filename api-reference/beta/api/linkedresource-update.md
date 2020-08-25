---
title: 更新 linkedResource
description: 更新 linkedResource 对象的属性。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0ce6ff6c8fd519888682e53939238dab02215007
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872565"
---
# <a name="update-linkedresource"></a><span data-ttu-id="2ac0a-103">更新 linkedResource</span><span class="sxs-lookup"><span data-stu-id="2ac0a-103">Update linkedResource</span></span>
<span data-ttu-id="2ac0a-104">命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="2ac0a-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="2ac0a-105">更新 [linkedResource](../resources/linkedresource.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2ac0a-105">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ac0a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2ac0a-106">Permissions</span></span>
<span data-ttu-id="2ac0a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ac0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ac0a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ac0a-109">Permission type</span></span>|<span data-ttu-id="2ac0a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2ac0a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ac0a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ac0a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2ac0a-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ac0a-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2ac0a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ac0a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ac0a-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ac0a-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2ac0a-115">应用</span><span class="sxs-lookup"><span data-stu-id="2ac0a-115">Application</span></span>|<span data-ttu-id="2ac0a-116">不支持</span><span class="sxs-lookup"><span data-stu-id="2ac0a-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ac0a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ac0a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="2ac0a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ac0a-118">Request headers</span></span>
|<span data-ttu-id="2ac0a-119">名称</span><span class="sxs-lookup"><span data-stu-id="2ac0a-119">Name</span></span>|<span data-ttu-id="2ac0a-120">说明</span><span class="sxs-lookup"><span data-stu-id="2ac0a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2ac0a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ac0a-121">Authorization</span></span>|<span data-ttu-id="2ac0a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ac0a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2ac0a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ac0a-124">Content-Type</span></span>|<span data-ttu-id="2ac0a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2ac0a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ac0a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ac0a-127">Request body</span></span>
<span data-ttu-id="2ac0a-128">在请求正文中，提供 [linkedResource](../resources/linkedresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ac0a-128">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="2ac0a-129">下表显示了在更新 [linkedResource](../resources/linkedresource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2ac0a-129">The following table shows the properties that are required when you update the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="2ac0a-130">属性</span><span class="sxs-lookup"><span data-stu-id="2ac0a-130">Property</span></span>|<span data-ttu-id="2ac0a-131">类型</span><span class="sxs-lookup"><span data-stu-id="2ac0a-131">Type</span></span>|<span data-ttu-id="2ac0a-132">说明</span><span class="sxs-lookup"><span data-stu-id="2ac0a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ac0a-133">id</span><span class="sxs-lookup"><span data-stu-id="2ac0a-133">id</span></span>|<span data-ttu-id="2ac0a-134">String</span><span class="sxs-lookup"><span data-stu-id="2ac0a-134">String</span></span>|<span data-ttu-id="2ac0a-135">从[实体](../resources/entity.md)继承的链接实体的服务器生成 Id</span><span class="sxs-lookup"><span data-stu-id="2ac0a-135">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|

## <a name="response"></a><span data-ttu-id="2ac0a-136">响应</span><span class="sxs-lookup"><span data-stu-id="2ac0a-136">Response</span></span>

<span data-ttu-id="2ac0a-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ac0a-137">If successful, this method returns a `200 OK` response code and an updated [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ac0a-138">示例</span><span class="sxs-lookup"><span data-stu-id="2ac0a-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ac0a-139">请求</span><span class="sxs-lookup"><span data-stu-id="2ac0a-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2ac0a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ac0a-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "update_linkedresource"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
Content-Type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "webUrl": "http://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
}
```
# <a name="javascript"></a>[<span data-ttu-id="2ac0a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ac0a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ac0a-142">响应</span><span class="sxs-lookup"><span data-stu-id="2ac0a-142">Response</span></span>
<span data-ttu-id="2ac0a-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2ac0a-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
  "webUrl": "http://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```
