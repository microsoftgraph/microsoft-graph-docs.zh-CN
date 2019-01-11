---
title: Permissions
description: '更新应用程序之前发布到 Microsoft 团队应用程序目录。 '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 125d078b5882e08ff5053acee372d8f352f6a2b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861668"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="e0bf7-103">更新应用程序发布到组织的应用程序目录</span><span class="sxs-lookup"><span data-stu-id="e0bf7-103">Update apps published to your organization's app catalog</span></span>

> <span data-ttu-id="e0bf7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e0bf7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0bf7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e0bf7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e0bf7-106">更新[应用程序](../resources/teamsapp.md)之前发布到 Microsoft 团队应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="e0bf7-106">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="e0bf7-107">此 API 专门更新应用程序发布到组织的应用程序目录 （租户应用程序目录）。</span><span class="sxs-lookup"><span data-stu-id="e0bf7-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="e0bf7-108">若要发布到组织的应用程序目录，请指定`organization`作为**distributionMethod** [teamsCatalogApp](../resources/teamsapp.md)资源中。</span><span class="sxs-lookup"><span data-stu-id="e0bf7-108">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0bf7-109">权限</span><span class="sxs-lookup"><span data-stu-id="e0bf7-109">Permissions</span></span>

<span data-ttu-id="e0bf7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="e0bf7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="e0bf7-112">**注意：** 只有全局管理员可以调用此 API。</span><span class="sxs-lookup"><span data-stu-id="e0bf7-112">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="e0bf7-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0bf7-113">Permission Type</span></span>                        | <span data-ttu-id="e0bf7-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0bf7-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="e0bf7-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0bf7-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0bf7-116">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0bf7-116">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="e0bf7-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0bf7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0bf7-118">不支持</span><span class="sxs-lookup"><span data-stu-id="e0bf7-118">Not supported</span></span>|
| <span data-ttu-id="e0bf7-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0bf7-119">Application</span></span>                            | <span data-ttu-id="e0bf7-120">不支持</span><span class="sxs-lookup"><span data-stu-id="e0bf7-120">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0bf7-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0bf7-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e0bf7-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0bf7-122">Request headers</span></span>

| <span data-ttu-id="e0bf7-123">标头</span><span class="sxs-lookup"><span data-stu-id="e0bf7-123">Header</span></span>        | <span data-ttu-id="e0bf7-124">值</span><span class="sxs-lookup"><span data-stu-id="e0bf7-124">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="e0bf7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0bf7-125">Authorization</span></span> | <span data-ttu-id="e0bf7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0bf7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e0bf7-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0bf7-128">Content-Type</span></span>  | <span data-ttu-id="e0bf7-129">应用程序/zip</span><span class="sxs-lookup"><span data-stu-id="e0bf7-129">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0bf7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0bf7-130">Request body</span></span>

<span data-ttu-id="e0bf7-131">团队 Zip 清单负载： 团队应用程序 zip 文件，[请参阅创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="e0bf7-131">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="e0bf7-132">**注意：** 使用从[列表发布应用程序](./teamsapp-list.md)的调用返回引用您想要更新的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="e0bf7-132">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="e0bf7-133">不要使用 zip 应用程序包的清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="e0bf7-133">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="e0bf7-134">响应</span><span class="sxs-lookup"><span data-stu-id="e0bf7-134">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="e0bf7-135">示例</span><span class="sxs-lookup"><span data-stu-id="e0bf7-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0bf7-136">请求</span><span class="sxs-lookup"><span data-stu-id="e0bf7-136">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="e0bf7-137">团队应用程序 zip 文件，[请参阅创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="e0bf7-137">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="e0bf7-138">响应</span><span class="sxs-lookup"><span data-stu-id="e0bf7-138">Response</span></span>

```
HTTP/1.1 204 No Content
```
