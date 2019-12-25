---
title: 权限
description: '更新之前发布到 Microsoft 团队应用程序目录的应用程序。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a1c66f2d189d3c85316277ee6c23b6c798d610f3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864087"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="8b06d-103">更新发布到组织的应用程序目录的应用程序</span><span class="sxs-lookup"><span data-stu-id="8b06d-103">Update apps published to your organization's app catalog</span></span>



<span data-ttu-id="8b06d-104">更新之前发布到 Microsoft 团队应用程序目录的[应用程序](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="8b06d-104">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="8b06d-105">此 API 专门更新发布到您的组织的应用程序目录（租户应用程序目录）的应用程序。</span><span class="sxs-lookup"><span data-stu-id="8b06d-105">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>
<span data-ttu-id="8b06d-106">若要发布到您的组织的应用程序`organization`目录，请在[teamsCatalogApp](../resources/teamsapp.md)资源中将其指定为**distributionMethod** 。</span><span class="sxs-lookup"><span data-stu-id="8b06d-106">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b06d-107">权限</span><span class="sxs-lookup"><span data-stu-id="8b06d-107">Permissions</span></span>

<span data-ttu-id="8b06d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="8b06d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="8b06d-110">**注意：** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8b06d-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="8b06d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b06d-111">Permission Type</span></span>                        | <span data-ttu-id="8b06d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b06d-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="8b06d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b06d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b06d-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b06d-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="8b06d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b06d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b06d-116">不支持</span><span class="sxs-lookup"><span data-stu-id="8b06d-116">Not supported</span></span>|
| <span data-ttu-id="8b06d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b06d-117">Application</span></span>                            | <span data-ttu-id="8b06d-118">不支持</span><span class="sxs-lookup"><span data-stu-id="8b06d-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b06d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b06d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8b06d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b06d-120">Request headers</span></span>

| <span data-ttu-id="8b06d-121">标头</span><span class="sxs-lookup"><span data-stu-id="8b06d-121">Header</span></span>        | <span data-ttu-id="8b06d-122">值</span><span class="sxs-lookup"><span data-stu-id="8b06d-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="8b06d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b06d-123">Authorization</span></span> | <span data-ttu-id="8b06d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8b06d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8b06d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b06d-126">Content-Type</span></span>  | <span data-ttu-id="8b06d-127">application/zip</span><span class="sxs-lookup"><span data-stu-id="8b06d-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b06d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b06d-128">Request body</span></span>

<span data-ttu-id="8b06d-129">团队 Zip 清单有效负载：对于团队应用程序 Zip 文件，[请参阅创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="8b06d-129">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="8b06d-130">**注意：** 使用从[列表已发布的应用程序](./teamsapp-list.md)调用中返回的 ID 引用要更新的应用程序。</span><span class="sxs-lookup"><span data-stu-id="8b06d-130">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span>
<span data-ttu-id="8b06d-131">请勿使用 zip 应用程序包清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="8b06d-131">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="8b06d-132">响应</span><span class="sxs-lookup"><span data-stu-id="8b06d-132">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="8b06d-133">示例</span><span class="sxs-lookup"><span data-stu-id="8b06d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b06d-134">请求</span><span class="sxs-lookup"><span data-stu-id="8b06d-134">Request</span></span>

```
PUT https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="8b06d-135">对于团队应用程序 zip 文件，[请参阅创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="8b06d-135">For Teams application zip file [see Create app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="8b06d-136">响应</span><span class="sxs-lookup"><span data-stu-id="8b06d-136">Response</span></span>

```
HTTP/1.1 204 No Content
```
