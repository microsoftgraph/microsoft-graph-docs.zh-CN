---
title: 列表中的 Microsoft 团队应用程序目录发布应用程序
description: '列出来自 Microsoft 团队应用程序目录的应用程序。 '
ms.openlocfilehash: 84b5576ed2a7d38783e45b1384c79f05c9ea418b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049373"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="bbbb1-103">列表中的 Microsoft 团队应用程序目录发布应用程序</span><span class="sxs-lookup"><span data-stu-id="bbbb1-103">List the published apps from the Microsoft Teams app catalog</span></span>

> <span data-ttu-id="bbbb1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bbbb1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbbb1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bbbb1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bbbb1-106">从 Microsoft 团队应用程序目录的列表[应用程序](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="bbbb1-106">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="bbbb1-107">这包括来自 Microsoft 团队商店的应用程序，以及来自您组织的应用程序目录 （租户应用程序目录） 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="bbbb1-107">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="bbbb1-108">若要从您的组织的应用程序目录获取应用程序，请指定`Organization`作为**distributionMethod** [teamsCatalogApp](../resources/teamsapp.md)资源中。</span><span class="sxs-lookup"><span data-stu-id="bbbb1-108">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbbb1-109">权限</span><span class="sxs-lookup"><span data-stu-id="bbbb1-109">Permissions</span></span>

<span data-ttu-id="bbbb1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="bbbb1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="bbbb1-112">**注意：** 只有全局管理员可以调用此 API。</span><span class="sxs-lookup"><span data-stu-id="bbbb1-112">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="bbbb1-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbbb1-113">Permission Type</span></span>                        | <span data-ttu-id="bbbb1-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bbbb1-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="bbbb1-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbbb1-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbbb1-116">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbbb1-116">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="bbbb1-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbbb1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbbb1-118">不支持</span><span class="sxs-lookup"><span data-stu-id="bbbb1-118">Not supported</span></span>|
| <span data-ttu-id="bbbb1-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbbb1-119">Application</span></span>                            | <span data-ttu-id="bbbb1-120">不支持</span><span class="sxs-lookup"><span data-stu-id="bbbb1-120">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbbb1-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbbb1-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bbbb1-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bbbb1-122">Optional query parameters</span></span>
<span data-ttu-id="bbbb1-123">此方法支持 $filter，$select，和 $expand [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="bbbb1-123">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbbb1-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbbb1-124">Request headers</span></span>

| <span data-ttu-id="bbbb1-125">标头</span><span class="sxs-lookup"><span data-stu-id="bbbb1-125">Header</span></span>        | <span data-ttu-id="bbbb1-126">值</span><span class="sxs-lookup"><span data-stu-id="bbbb1-126">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="bbbb1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbbb1-127">Authorization</span></span> | <span data-ttu-id="bbbb1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bbbb1-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bbbb1-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbbb1-130">Request body</span></span>
<span data-ttu-id="bbbb1-131">无。</span><span class="sxs-lookup"><span data-stu-id="bbbb1-131">None.</span></span>

><span data-ttu-id="bbbb1-132">**注意：** 您可以在任何[teamsCatalogApp](../resources/teamsapp.md)对象，以缩短结果列表中的字段进行筛选。</span><span class="sxs-lookup"><span data-stu-id="bbbb1-132">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="bbbb1-133">您可以使用任何以下筛选器操作： 等于、 不等，或，并且没有。</span><span class="sxs-lookup"><span data-stu-id="bbbb1-133">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="bbbb1-134">响应</span><span class="sxs-lookup"><span data-stu-id="bbbb1-134">Response</span></span>
<span data-ttu-id="bbbb1-135">如果成功，此方法返回`200 OK`响应代码和响应正文中的[teamsCatalogApp](../resources/teamsapp.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="bbbb1-135">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bbbb1-136">示例</span><span class="sxs-lookup"><span data-stu-id="bbbb1-136">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="bbbb1-137">示例 1</span><span class="sxs-lookup"><span data-stu-id="bbbb1-137">Example 1</span></span>
<span data-ttu-id="bbbb1-138">以下示例将列出所有特定于您的租户的应用程序。</span><span class="sxs-lookup"><span data-stu-id="bbbb1-138">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="bbbb1-139">请求</span><span class="sxs-lookup"><span data-stu-id="bbbb1-139">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="bbbb1-140">响应</span><span class="sxs-lookup"><span data-stu-id="bbbb1-140">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

### <a name="example-2"></a><span data-ttu-id="bbbb1-141">示例 2</span><span class="sxs-lookup"><span data-stu-id="bbbb1-141">Example 2</span></span>

<span data-ttu-id="bbbb1-142">以下示例将列出具有给定 ID 的应用程序</span><span class="sxs-lookup"><span data-stu-id="bbbb1-142">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="bbbb1-143">请求</span><span class="sxs-lookup"><span data-stu-id="bbbb1-143">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="bbbb1-144">响应</span><span class="sxs-lookup"><span data-stu-id="bbbb1-144">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

