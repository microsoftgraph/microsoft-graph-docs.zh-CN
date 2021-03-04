---
title: 创建 sourceCollection
description: 创建新的 sourceCollection 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 69476c91acffc6d0a1edc8a18cc4208c5239fa26
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446080"
---
# <a name="create-sourcecollection"></a><span data-ttu-id="65094-103">创建 sourceCollection</span><span class="sxs-lookup"><span data-stu-id="65094-103">Create sourceCollection</span></span>

<span data-ttu-id="65094-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="65094-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65094-105">创建新的 [sourceCollection](../resources/ediscovery-sourcecollection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65094-105">Create a new [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="65094-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="65094-106">Permissions</span></span>

<span data-ttu-id="65094-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65094-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65094-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="65094-109">Permission type</span></span>|<span data-ttu-id="65094-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65094-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65094-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65094-111">Delegated (work or school account)</span></span>|<span data-ttu-id="65094-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65094-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="65094-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65094-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65094-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="65094-114">Not supported.</span></span>|
|<span data-ttu-id="65094-115">Application</span><span class="sxs-lookup"><span data-stu-id="65094-115">Application</span></span>|<span data-ttu-id="65094-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="65094-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65094-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65094-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections
```

## <a name="request-headers"></a><span data-ttu-id="65094-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="65094-118">Request headers</span></span>

|<span data-ttu-id="65094-119">名称</span><span class="sxs-lookup"><span data-stu-id="65094-119">Name</span></span>|<span data-ttu-id="65094-120">说明</span><span class="sxs-lookup"><span data-stu-id="65094-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="65094-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65094-121">Authorization</span></span>|<span data-ttu-id="65094-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65094-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="65094-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65094-124">Content-Type</span></span>|<span data-ttu-id="65094-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="65094-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65094-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="65094-127">Request body</span></span>

<span data-ttu-id="65094-128">在请求正文中，提供 [sourceCollection](../resources/ediscovery-sourcecollection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65094-128">In the request body, supply a JSON representation of the [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

<span data-ttu-id="65094-129">下表显示创建 [sourceCollection](../resources/ediscovery-sourcecollection.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="65094-129">The following table shows the properties that are required when you create the [sourceCollection](../resources/ediscovery-sourcecollection.md).</span></span>

|<span data-ttu-id="65094-130">属性</span><span class="sxs-lookup"><span data-stu-id="65094-130">Property</span></span>|<span data-ttu-id="65094-131">类型</span><span class="sxs-lookup"><span data-stu-id="65094-131">Type</span></span>|<span data-ttu-id="65094-132">说明</span><span class="sxs-lookup"><span data-stu-id="65094-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65094-133">displayName</span><span class="sxs-lookup"><span data-stu-id="65094-133">displayName</span></span>|<span data-ttu-id="65094-134">String</span><span class="sxs-lookup"><span data-stu-id="65094-134">String</span></span>|<span data-ttu-id="65094-135">**sourceCollection** 显示名称</span><span class="sxs-lookup"><span data-stu-id="65094-135">The display name of the **sourceCollection**</span></span>|
|<span data-ttu-id="65094-136">custodianSources</span><span class="sxs-lookup"><span data-stu-id="65094-136">custodianSources</span></span>|<span data-ttu-id="65094-137">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="65094-137">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection</span></span>|<span data-ttu-id="65094-138">要在此搜索中包括的保管人源。</span><span class="sxs-lookup"><span data-stu-id="65094-138">The custodian sources to include in this search.</span></span> <span data-ttu-id="65094-139">你可以从保管人[siteSources、unifiedGroupSources](../api/ediscovery-custodian-list-sitesources.md)或[userSources](../api/ediscovery-custodian-list-usersources.md)获取 URL 以及源的 ID。 [](../api/ediscovery-custodian-list-unifiedgroupsources.md)</span><span class="sxs-lookup"><span data-stu-id="65094-139">You can get the URL from from custodian [siteSources](../api/ediscovery-custodian-list-sitesources.md), [unifiedGroupSources](../api/ediscovery-custodian-list-unifiedgroupsources.md), or [userSources](../api/ediscovery-custodian-list-usersources.md) plus the ID of the source.</span></span> <span data-ttu-id="65094-140">**注意：** 创建源集合时，需要一个保管人或指定租户源。</span><span class="sxs-lookup"><span data-stu-id="65094-140">**Note:** Either one custodian or specifying tenant source is required when creating a source collection.</span></span> |
|<span data-ttu-id="65094-141">tenantSources</span><span class="sxs-lookup"><span data-stu-id="65094-141">tenantSources</span></span>|<span data-ttu-id="65094-142">microsoft.graph.ediscovery.tenantSources</span><span class="sxs-lookup"><span data-stu-id="65094-142">microsoft.graph.ediscovery.tenantSources</span></span>|<span data-ttu-id="65094-143">指定此参数时，集合将跨越整个工作负荷的服务。</span><span class="sxs-lookup"><span data-stu-id="65094-143">When specified, the collection will span across a service for an entire workload.</span></span> <span data-ttu-id="65094-144">可取值为：`allMailboxes`、`allSites`。</span><span class="sxs-lookup"><span data-stu-id="65094-144">Possible values are: `allMailboxes`, `allSites`.</span></span> <span data-ttu-id="65094-145">**注意：** 创建源集合时，需要一个保管人或指定租户源。</span><span class="sxs-lookup"><span data-stu-id="65094-145">**Note:** Either one custodian or specifying tenant source is required when creating a source collection.</span></span>|

## <a name="response"></a><span data-ttu-id="65094-146">响应</span><span class="sxs-lookup"><span data-stu-id="65094-146">Response</span></span>

<span data-ttu-id="65094-147">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65094-147">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65094-148">示例</span><span class="sxs-lookup"><span data-stu-id="65094-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65094-149">请求</span><span class="sxs-lookup"><span data-stu-id="65094-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_sourcecollection_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections
Content-Type: application/json
Content-length: 272

{
    "displayName": "Quarterly Financials search",
    "contentQuery": "subject:'Quarterly Financials'",
    "custodianSources@odata.bind": [
        "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735"
    ]
}
```

### <a name="response"></a><span data-ttu-id="65094-150">响应</span><span class="sxs-lookup"><span data-stu-id="65094-150">Response</span></span>

<span data-ttu-id="65094-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="65094-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.sourceCollection"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/$entity",
    "description": null,
    "lastModifiedDateTime": "2021-01-12T18:09:03.7378679Z",
    "contentQuery": "subject:'Quarterly Financials'",
    "tenantSources": "none",
    "id": "1a9b4145d8f84e39bc45a7f68c5c5119",
    "displayName": "Quarterly Financials search",
    "createdDateTime": "2021-01-12T18:09:03.417009Z",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.com"
        }
    },
    "lastModifiedBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.com"
        }
    }
}
```
