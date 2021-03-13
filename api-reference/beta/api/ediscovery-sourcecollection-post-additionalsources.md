---
title: 创建 dataSource
description: 向源集合添加其他数据源。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 61da920c39cb75583661fde46c9bdbcc0a5d568d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772595"
---
# <a name="create-datasource"></a><span data-ttu-id="d695e-103">创建 dataSource</span><span class="sxs-lookup"><span data-stu-id="d695e-103">Create dataSource</span></span>

<span data-ttu-id="d695e-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="d695e-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d695e-105">向源集合添加其他数据源。</span><span class="sxs-lookup"><span data-stu-id="d695e-105">Add additional data sources to a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="d695e-106">权限</span><span class="sxs-lookup"><span data-stu-id="d695e-106">Permissions</span></span>

<span data-ttu-id="d695e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d695e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d695e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d695e-109">Permission type</span></span>|<span data-ttu-id="d695e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d695e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d695e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d695e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d695e-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d695e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="d695e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d695e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d695e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d695e-114">Not supported.</span></span>|
|<span data-ttu-id="d695e-115">Application</span><span class="sxs-lookup"><span data-stu-id="d695e-115">Application</span></span>|<span data-ttu-id="d695e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d695e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d695e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d695e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```

## <a name="request-headers"></a><span data-ttu-id="d695e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d695e-118">Request headers</span></span>

|<span data-ttu-id="d695e-119">名称</span><span class="sxs-lookup"><span data-stu-id="d695e-119">Name</span></span>|<span data-ttu-id="d695e-120">说明</span><span class="sxs-lookup"><span data-stu-id="d695e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d695e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d695e-121">Authorization</span></span>|<span data-ttu-id="d695e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d695e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d695e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d695e-124">Content-Type</span></span>|<span data-ttu-id="d695e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d695e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d695e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d695e-127">Request body</span></span>

<span data-ttu-id="d695e-128">在请求正文中，提供 [dataSource](../resources/ediscovery-datasource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d695e-128">In the request body, supply a JSON representation of the [dataSource](../resources/ediscovery-datasource.md) object.</span></span>

<span data-ttu-id="d695e-129">下表显示创建 [dataSource](../resources/ediscovery-datasource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d695e-129">The following table shows the properties that are required when you create the [dataSource](../resources/ediscovery-datasource.md).</span></span>

|<span data-ttu-id="d695e-130">属性</span><span class="sxs-lookup"><span data-stu-id="d695e-130">Property</span></span>|<span data-ttu-id="d695e-131">类型</span><span class="sxs-lookup"><span data-stu-id="d695e-131">Type</span></span>|<span data-ttu-id="d695e-132">说明</span><span class="sxs-lookup"><span data-stu-id="d695e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d695e-133">id</span><span class="sxs-lookup"><span data-stu-id="d695e-133">id</span></span>|<span data-ttu-id="d695e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d695e-134">String</span></span>|<span data-ttu-id="d695e-135">[sourceCollection](../resources/ediscovery-sourcecollection.md)案例的 ID。</span><span class="sxs-lookup"><span data-stu-id="d695e-135">The ID for [sourceCollection](../resources/ediscovery-sourcecollection.md) case.</span></span> <span data-ttu-id="d695e-136">只读。</span><span class="sxs-lookup"><span data-stu-id="d695e-136">Read-only.</span></span> <span data-ttu-id="d695e-137">继承自 [实体](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="d695e-137">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="d695e-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d695e-138">displayName</span></span>|<span data-ttu-id="d695e-139">字符串</span><span class="sxs-lookup"><span data-stu-id="d695e-139">String</span></span>|<span data-ttu-id="d695e-140">[sourceCollection 的名称](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d695e-140">The name of the [sourceCollection](../resources/ediscovery-sourcecollection.md)</span></span>|
|<span data-ttu-id="d695e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d695e-141">createdDateTime</span></span>|<span data-ttu-id="d695e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d695e-142">DateTimeOffset</span></span>|<span data-ttu-id="d695e-143">创建 [sourceCollection](../resources/ediscovery-sourcecollection.md) 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d695e-143">The date and time when the [sourceCollection](../resources/ediscovery-sourcecollection.md) was created.</span></span>|
|<span data-ttu-id="d695e-144">createdBy</span><span class="sxs-lookup"><span data-stu-id="d695e-144">createdBy</span></span>|[<span data-ttu-id="d695e-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="d695e-145">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="d695e-146">创建 [sourceCollection 的用户](../resources/ediscovery-sourcecollection.md)。</span><span class="sxs-lookup"><span data-stu-id="d695e-146">The user who created the [sourceCollection](../resources/ediscovery-sourcecollection.md).</span></span>|

## <a name="response"></a><span data-ttu-id="d695e-147">响应</span><span class="sxs-lookup"><span data-stu-id="d695e-147">Response</span></span>

<span data-ttu-id="d695e-148">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d695e-148">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d695e-149">示例</span><span class="sxs-lookup"><span data-stu-id="d695e-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d695e-150">请求</span><span class="sxs-lookup"><span data-stu-id="d695e-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d695e-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="d695e-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_datasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
Content-Type: application/json
Content-length: 179

{
    "@odata.type": "#microsoft.graph.ediscovery.userSource",
    "email": "badguy@contoso.com"
}
```
# <a name="c"></a>[<span data-ttu-id="d695e-152">C#</span><span class="sxs-lookup"><span data-stu-id="d695e-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-datasource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d695e-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d695e-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-datasource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d695e-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d695e-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-datasource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d695e-155">Java</span><span class="sxs-lookup"><span data-stu-id="d695e-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-datasource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d695e-156">响应</span><span class="sxs-lookup"><span data-stu-id="d695e-156">Response</span></span>

<span data-ttu-id="d695e-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d695e-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.dataSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.ediscovery.dataSource",
  "id": "0fb67fc5-7fc5-0fb6-c57f-b60fc57fb60f",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```
