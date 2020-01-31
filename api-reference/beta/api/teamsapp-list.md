---
title: 列出 Microsoft 团队应用程序目录中已发布的应用程序
description: '列出 Microsoft 团队应用程序目录中的应用程序。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4a27a7b63248ddb94e4ea819300f325e04a02c9f
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636516"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="71253-103">列出 Microsoft 团队应用程序目录中已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="71253-103">List the published apps from the Microsoft Teams app catalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71253-104">列出 Microsoft 团队应用程序目录中的[应用程序](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="71253-104">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="71253-105">这包括 Microsoft 团队存储区中的应用程序，以及组织的应用程序目录（租户应用程序目录）中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="71253-105">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="71253-106">若要仅从组织的应用程序目录中获取应用`Organization`程序，请在[teamsCatalogApp](../resources/teamsapp.md)资源中将其指定为**distributionMethod** 。</span><span class="sxs-lookup"><span data-stu-id="71253-106">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="71253-107">权限</span><span class="sxs-lookup"><span data-stu-id="71253-107">Permissions</span></span>

<span data-ttu-id="71253-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="71253-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

| <span data-ttu-id="71253-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="71253-110">Permission Type</span></span>                        | <span data-ttu-id="71253-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71253-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="71253-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71253-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="71253-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71253-113">AppCatalog.ReadWrite.All</span></span>            |
| <span data-ttu-id="71253-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71253-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71253-115">不支持</span><span class="sxs-lookup"><span data-stu-id="71253-115">Not supported</span></span>                       |
| <span data-ttu-id="71253-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="71253-116">Application</span></span>                            | <span data-ttu-id="71253-117">不支持</span><span class="sxs-lookup"><span data-stu-id="71253-117">Not supported</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="71253-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71253-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71253-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="71253-119">Optional query parameters</span></span>

<span data-ttu-id="71253-120">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="71253-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71253-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="71253-121">Request headers</span></span>

| <span data-ttu-id="71253-122">标头</span><span class="sxs-lookup"><span data-stu-id="71253-122">Header</span></span>        | <span data-ttu-id="71253-123">值</span><span class="sxs-lookup"><span data-stu-id="71253-123">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="71253-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="71253-124">Authorization</span></span> | <span data-ttu-id="71253-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71253-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71253-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="71253-127">Request body</span></span>

<span data-ttu-id="71253-128">无。</span><span class="sxs-lookup"><span data-stu-id="71253-128">None.</span></span>

> <span data-ttu-id="71253-129">**注意：** 您可以对[teamsCatalogApp](../resources/teamsapp.md)对象的任何字段进行筛选，以缩短结果列表。</span><span class="sxs-lookup"><span data-stu-id="71253-129">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="71253-130">您可以使用以下任何筛选器操作：等于、不等于、和、或，而不是。</span><span class="sxs-lookup"><span data-stu-id="71253-130">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="71253-131">响应</span><span class="sxs-lookup"><span data-stu-id="71253-131">Response</span></span>

<span data-ttu-id="71253-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[teamsCatalogApp](../resources/teamsapp.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="71253-132">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71253-133">示例</span><span class="sxs-lookup"><span data-stu-id="71253-133">Examples</span></span>

### <a name="example-1-list-all-applications"></a><span data-ttu-id="71253-134">示例1：列出所有应用程序</span><span class="sxs-lookup"><span data-stu-id="71253-134">Example 1: List all applications</span></span>

<span data-ttu-id="71253-135">下面的示例列出了特定于您的租户的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="71253-135">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="71253-136">请求</span><span class="sxs-lookup"><span data-stu-id="71253-136">Request</span></span>

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="71253-137">响应</span><span class="sxs-lookup"><span data-stu-id="71253-137">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="71253-138">示例2：列出具有给定 ID 的应用程序</span><span class="sxs-lookup"><span data-stu-id="71253-138">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="71253-139">下面的示例列出了具有给定 ID 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="71253-139">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="71253-140">请求</span><span class="sxs-lookup"><span data-stu-id="71253-140">Request</span></span>

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="71253-141">响应</span><span class="sxs-lookup"><span data-stu-id="71253-141">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

