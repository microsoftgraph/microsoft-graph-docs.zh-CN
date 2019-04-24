---
title: 权限
description: '更新之前发布到 Microsoft 团队应用程序目录的应用程序。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b89380a423bf01f6a2bd7e56086cc9290be094cb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521829"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="6eeda-103">更新发布到组织的应用程序目录的应用程序</span><span class="sxs-lookup"><span data-stu-id="6eeda-103">Update apps published to your organization's app catalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6eeda-104">更新之前发布到 Microsoft 团队应用程序目录的[应用程序](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="6eeda-104">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="6eeda-105">此 API 专门更新发布到您的组织的应用程序目录 (租户应用程序目录) 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="6eeda-105">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="6eeda-106">若要发布到您的组织的应用程序`organization`目录, 请在[teamsCatalogApp](../resources/teamsapp.md)资源中将其指定为**distributionMethod** 。</span><span class="sxs-lookup"><span data-stu-id="6eeda-106">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="6eeda-107">权限</span><span class="sxs-lookup"><span data-stu-id="6eeda-107">Permissions</span></span>

<span data-ttu-id="6eeda-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="6eeda-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="6eeda-110">**注意:** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6eeda-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="6eeda-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6eeda-111">Permission Type</span></span>                        | <span data-ttu-id="6eeda-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6eeda-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="6eeda-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6eeda-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6eeda-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6eeda-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="6eeda-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6eeda-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6eeda-116">不支持</span><span class="sxs-lookup"><span data-stu-id="6eeda-116">Not supported</span></span>|
| <span data-ttu-id="6eeda-117">Application</span><span class="sxs-lookup"><span data-stu-id="6eeda-117">Application</span></span>                            | <span data-ttu-id="6eeda-118">不支持</span><span class="sxs-lookup"><span data-stu-id="6eeda-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="6eeda-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6eeda-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6eeda-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6eeda-120">Request headers</span></span>

| <span data-ttu-id="6eeda-121">标头</span><span class="sxs-lookup"><span data-stu-id="6eeda-121">Header</span></span>        | <span data-ttu-id="6eeda-122">值</span><span class="sxs-lookup"><span data-stu-id="6eeda-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="6eeda-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6eeda-123">Authorization</span></span> | <span data-ttu-id="6eeda-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6eeda-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6eeda-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6eeda-126">Content-Type</span></span>  | <span data-ttu-id="6eeda-127">application/zip</span><span class="sxs-lookup"><span data-stu-id="6eeda-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="6eeda-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6eeda-128">Request body</span></span>

<span data-ttu-id="6eeda-129">团队 Zip 清单有效负载: 对于团队应用程序 Zip 文件,[请参阅创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="6eeda-129">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="6eeda-130">**注意:** 使用从[列表已发布的应用程序](./teamsapp-list.md)调用中返回的 ID 引用要更新的应用程序。</span><span class="sxs-lookup"><span data-stu-id="6eeda-130">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="6eeda-131">请勿使用 zip 应用程序包清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="6eeda-131">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="6eeda-132">响应</span><span class="sxs-lookup"><span data-stu-id="6eeda-132">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="6eeda-133">示例</span><span class="sxs-lookup"><span data-stu-id="6eeda-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6eeda-134">请求</span><span class="sxs-lookup"><span data-stu-id="6eeda-134">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="6eeda-135">对于团队应用程序 zip 文件,[请参阅创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="6eeda-135">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="6eeda-136">响应</span><span class="sxs-lookup"><span data-stu-id="6eeda-136">Response</span></span>

```
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
