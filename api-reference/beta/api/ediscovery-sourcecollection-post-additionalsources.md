---
title: 创建 dataSource
description: 将其他数据源添加到源集合。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: d2dca8b1b2ae6c6e1fc350f9b7185e16608427a7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445998"
---
# <a name="create-datasource"></a><span data-ttu-id="4904d-103">创建 dataSource</span><span class="sxs-lookup"><span data-stu-id="4904d-103">Create dataSource</span></span>

<span data-ttu-id="4904d-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="4904d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4904d-105">将其他数据源添加到源集合。</span><span class="sxs-lookup"><span data-stu-id="4904d-105">Add additional data sources to a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="4904d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4904d-106">Permissions</span></span>

<span data-ttu-id="4904d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4904d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4904d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4904d-109">Permission type</span></span>|<span data-ttu-id="4904d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4904d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4904d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4904d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4904d-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4904d-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="4904d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4904d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4904d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4904d-114">Not supported.</span></span>|
|<span data-ttu-id="4904d-115">Application</span><span class="sxs-lookup"><span data-stu-id="4904d-115">Application</span></span>|<span data-ttu-id="4904d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4904d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4904d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4904d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```

## <a name="request-headers"></a><span data-ttu-id="4904d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4904d-118">Request headers</span></span>

|<span data-ttu-id="4904d-119">名称</span><span class="sxs-lookup"><span data-stu-id="4904d-119">Name</span></span>|<span data-ttu-id="4904d-120">说明</span><span class="sxs-lookup"><span data-stu-id="4904d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4904d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4904d-121">Authorization</span></span>|<span data-ttu-id="4904d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4904d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4904d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4904d-124">Content-Type</span></span>|<span data-ttu-id="4904d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4904d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4904d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4904d-127">Request body</span></span>

<span data-ttu-id="4904d-128">在请求正文中，提供 [dataSource](../resources/ediscovery-datasource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4904d-128">In the request body, supply a JSON representation of the [dataSource](../resources/ediscovery-datasource.md) object.</span></span>

<span data-ttu-id="4904d-129">下表显示创建 [dataSource](../resources/ediscovery-datasource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4904d-129">The following table shows the properties that are required when you create the [dataSource](../resources/ediscovery-datasource.md).</span></span>

|<span data-ttu-id="4904d-130">属性</span><span class="sxs-lookup"><span data-stu-id="4904d-130">Property</span></span>|<span data-ttu-id="4904d-131">类型</span><span class="sxs-lookup"><span data-stu-id="4904d-131">Type</span></span>|<span data-ttu-id="4904d-132">说明</span><span class="sxs-lookup"><span data-stu-id="4904d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4904d-133">id</span><span class="sxs-lookup"><span data-stu-id="4904d-133">id</span></span>|<span data-ttu-id="4904d-134">String</span><span class="sxs-lookup"><span data-stu-id="4904d-134">String</span></span>|<span data-ttu-id="4904d-135">[sourceCollection](../resources/ediscovery-sourcecollection.md)案例的 ID。</span><span class="sxs-lookup"><span data-stu-id="4904d-135">The ID for [sourceCollection](../resources/ediscovery-sourcecollection.md) case.</span></span> <span data-ttu-id="4904d-136">只读。</span><span class="sxs-lookup"><span data-stu-id="4904d-136">Read-only.</span></span> <span data-ttu-id="4904d-137">继承自 [实体](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="4904d-137">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="4904d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="4904d-138">displayName</span></span>|<span data-ttu-id="4904d-139">String</span><span class="sxs-lookup"><span data-stu-id="4904d-139">String</span></span>|<span data-ttu-id="4904d-140">[sourceCollection 的名称](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4904d-140">The name of the [sourceCollection](../resources/ediscovery-sourcecollection.md)</span></span>|
|<span data-ttu-id="4904d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4904d-141">createdDateTime</span></span>|<span data-ttu-id="4904d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4904d-142">DateTimeOffset</span></span>|<span data-ttu-id="4904d-143">创建 [sourceCollection 的](../resources/ediscovery-sourcecollection.md) 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4904d-143">The date and time when the [sourceCollection](../resources/ediscovery-sourcecollection.md) was created.</span></span>|
|<span data-ttu-id="4904d-144">createdBy</span><span class="sxs-lookup"><span data-stu-id="4904d-144">createdBy</span></span>|[<span data-ttu-id="4904d-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="4904d-145">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="4904d-146">创建 [sourceCollection 的用户](../resources/ediscovery-sourcecollection.md)。</span><span class="sxs-lookup"><span data-stu-id="4904d-146">The user who created the [sourceCollection](../resources/ediscovery-sourcecollection.md).</span></span>|

## <a name="response"></a><span data-ttu-id="4904d-147">响应</span><span class="sxs-lookup"><span data-stu-id="4904d-147">Response</span></span>

<span data-ttu-id="4904d-148">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4904d-148">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4904d-149">示例</span><span class="sxs-lookup"><span data-stu-id="4904d-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4904d-150">请求</span><span class="sxs-lookup"><span data-stu-id="4904d-150">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="4904d-151">响应</span><span class="sxs-lookup"><span data-stu-id="4904d-151">Response</span></span>

<span data-ttu-id="4904d-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4904d-152">**Note:** The response object shown here might be shortened for readability.</span></span>
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
