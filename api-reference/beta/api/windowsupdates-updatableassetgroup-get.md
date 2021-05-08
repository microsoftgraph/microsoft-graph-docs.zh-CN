---
title: 获取 updatableAssetGroup
description: 读取 updatableAssetGroup 对象的属性和关系。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 96019f9fac94e79e51963ce98a878799b58d918e
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52238939"
---
# <a name="get-updatableassetgroup"></a><span data-ttu-id="d30c0-103">获取 updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="d30c0-103">Get updatableAssetGroup</span></span>
<span data-ttu-id="d30c0-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="d30c0-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d30c0-105">读取 [updatableAssetGroup 对象的属性和](../resources/windowsupdates-updatableassetgroup.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="d30c0-105">Read the properties and relationships of an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d30c0-106">权限</span><span class="sxs-lookup"><span data-stu-id="d30c0-106">Permissions</span></span>
<span data-ttu-id="d30c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d30c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d30c0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d30c0-109">Permission type</span></span>|<span data-ttu-id="d30c0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d30c0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d30c0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d30c0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d30c0-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d30c0-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="d30c0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d30c0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d30c0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d30c0-114">Not supported.</span></span>|
|<span data-ttu-id="d30c0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d30c0-115">Application</span></span>|<span data-ttu-id="d30c0-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d30c0-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d30c0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d30c0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{updatableAssetGroupId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d30c0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d30c0-118">Optional query parameters</span></span>
<span data-ttu-id="d30c0-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d30c0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d30c0-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d30c0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d30c0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d30c0-121">Request headers</span></span>
|<span data-ttu-id="d30c0-122">名称</span><span class="sxs-lookup"><span data-stu-id="d30c0-122">Name</span></span>|<span data-ttu-id="d30c0-123">说明</span><span class="sxs-lookup"><span data-stu-id="d30c0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d30c0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d30c0-124">Authorization</span></span>|<span data-ttu-id="d30c0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d30c0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d30c0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d30c0-127">Request body</span></span>
<span data-ttu-id="d30c0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d30c0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d30c0-129">响应</span><span class="sxs-lookup"><span data-stu-id="d30c0-129">Response</span></span>

<span data-ttu-id="d30c0-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d30c0-130">If successful, this method returns a `200 OK` response code and an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d30c0-131">示例</span><span class="sxs-lookup"><span data-stu-id="d30c0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d30c0-132">请求</span><span class="sxs-lookup"><span data-stu-id="d30c0-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d30c0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d30c0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_updatableassetgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/5c55730b-730b-5c55-0b73-555c0b73555c
```
# <a name="c"></a>[<span data-ttu-id="d30c0-134">C#</span><span class="sxs-lookup"><span data-stu-id="d30c0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-updatableassetgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d30c0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d30c0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-updatableassetgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d30c0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d30c0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-updatableassetgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d30c0-137">Java</span><span class="sxs-lookup"><span data-stu-id="d30c0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-updatableassetgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d30c0-138">响应</span><span class="sxs-lookup"><span data-stu-id="d30c0-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetGroup"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
    "id": "5c55730b-730b-5c55-0b73-555c0b73555c"
  }
}
```

