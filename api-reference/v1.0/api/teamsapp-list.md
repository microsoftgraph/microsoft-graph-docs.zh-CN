---
title: 列表中的 Microsoft 团队应用程序目录发布应用程序
description: '列出来自 Microsoft 团队应用程序目录的应用程序。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fc8648ac99a3b502956ce07d5c5b53bab930095e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945585"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="026b9-103">列表中的 Microsoft 团队应用程序目录发布应用程序</span><span class="sxs-lookup"><span data-stu-id="026b9-103">List the published apps from the Microsoft Teams app catalog</span></span>



<span data-ttu-id="026b9-104">从 Microsoft 团队应用程序目录的列表[应用程序](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="026b9-104">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="026b9-105">这包括来自 Microsoft 团队商店的应用程序，以及来自您组织的应用程序目录 （租户应用程序目录） 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="026b9-105">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="026b9-106">若要从您的组织的应用程序目录获取应用程序，请指定`Organization`作为**distributionMethod** [teamsCatalogApp](../resources/teamsapp.md)资源中。</span><span class="sxs-lookup"><span data-stu-id="026b9-106">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="026b9-107">权限</span><span class="sxs-lookup"><span data-stu-id="026b9-107">Permissions</span></span>

<span data-ttu-id="026b9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="026b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="026b9-110">**注意：** 只有全局管理员可以调用此 API。</span><span class="sxs-lookup"><span data-stu-id="026b9-110">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="026b9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="026b9-111">Permission Type</span></span>                        | <span data-ttu-id="026b9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="026b9-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="026b9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="026b9-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="026b9-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="026b9-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="026b9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="026b9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="026b9-116">不支持</span><span class="sxs-lookup"><span data-stu-id="026b9-116">Not supported</span></span>|
| <span data-ttu-id="026b9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="026b9-117">Application</span></span>                            | <span data-ttu-id="026b9-118">不支持</span><span class="sxs-lookup"><span data-stu-id="026b9-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="026b9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="026b9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="026b9-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="026b9-120">Optional query parameters</span></span>
<span data-ttu-id="026b9-121">此方法支持 $filter，$select，和 $expand [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="026b9-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="026b9-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="026b9-122">Request headers</span></span>

| <span data-ttu-id="026b9-123">标头</span><span class="sxs-lookup"><span data-stu-id="026b9-123">Header</span></span>        | <span data-ttu-id="026b9-124">值</span><span class="sxs-lookup"><span data-stu-id="026b9-124">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="026b9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="026b9-125">Authorization</span></span> | <span data-ttu-id="026b9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="026b9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="026b9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="026b9-128">Request body</span></span>
<span data-ttu-id="026b9-129">无。</span><span class="sxs-lookup"><span data-stu-id="026b9-129">None.</span></span>

><span data-ttu-id="026b9-130">**注意：** 您可以在任何[teamsCatalogApp](../resources/teamsapp.md)对象，以缩短结果列表中的字段进行筛选。</span><span class="sxs-lookup"><span data-stu-id="026b9-130">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="026b9-131">您可以使用任何以下筛选器操作： 等于、 不等，或，并且没有。</span><span class="sxs-lookup"><span data-stu-id="026b9-131">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="026b9-132">响应</span><span class="sxs-lookup"><span data-stu-id="026b9-132">Response</span></span>
<span data-ttu-id="026b9-133">如果成功，此方法返回`200 OK`响应代码和响应正文中的[teamsCatalogApp](../resources/teamsapp.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="026b9-133">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="026b9-134">示例</span><span class="sxs-lookup"><span data-stu-id="026b9-134">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="026b9-135">示例 1</span><span class="sxs-lookup"><span data-stu-id="026b9-135">Example 1</span></span>
<span data-ttu-id="026b9-136">以下示例将列出所有特定于您的租户的应用程序。</span><span class="sxs-lookup"><span data-stu-id="026b9-136">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="026b9-137">请求</span><span class="sxs-lookup"><span data-stu-id="026b9-137">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="026b9-138">响应</span><span class="sxs-lookup"><span data-stu-id="026b9-138">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="026b9-139">示例 2</span><span class="sxs-lookup"><span data-stu-id="026b9-139">Example 2</span></span>

<span data-ttu-id="026b9-140">以下示例将列出具有给定 ID 的应用程序</span><span class="sxs-lookup"><span data-stu-id="026b9-140">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="026b9-141">请求</span><span class="sxs-lookup"><span data-stu-id="026b9-141">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="026b9-142">响应</span><span class="sxs-lookup"><span data-stu-id="026b9-142">Response</span></span>
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

