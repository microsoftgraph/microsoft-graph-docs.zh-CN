---
title: Permissions
description: '从组织的应用程序目录 （租户应用程序目录） 中删除应用程序。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: bce53c91d498a36405f44ffa13827cdeb40c074e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953714"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="fef99-103">从组织的应用程序目录中删除应用程序</span><span class="sxs-lookup"><span data-stu-id="fef99-103">Remove an app from your organization's app catalog</span></span>

> <span data-ttu-id="fef99-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fef99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fef99-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fef99-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fef99-106">从组织的应用程序目录 （租户应用程序目录） 中删除[应用程序](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="fef99-106">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="fef99-107">若要从您的组织的应用程序目录中删除您的应用程序，请指定`organization`作为**distributionMethod** [teamsCatalogApp](../resources/teamsapp.md)资源中。</span><span class="sxs-lookup"><span data-stu-id="fef99-107">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="fef99-108">权限</span><span class="sxs-lookup"><span data-stu-id="fef99-108">Permissions</span></span>

<span data-ttu-id="fef99-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="fef99-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="fef99-111">**注意：** 只有全局管理员可以调用此 API。</span><span class="sxs-lookup"><span data-stu-id="fef99-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="fef99-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="fef99-112">Permission Type</span></span>                        | <span data-ttu-id="fef99-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fef99-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="fef99-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fef99-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="fef99-115">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fef99-115">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="fef99-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fef99-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fef99-117">不支持</span><span class="sxs-lookup"><span data-stu-id="fef99-117">Not supported</span></span>|
| <span data-ttu-id="fef99-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="fef99-118">Application</span></span>                            | <span data-ttu-id="fef99-119">不支持</span><span class="sxs-lookup"><span data-stu-id="fef99-119">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="fef99-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fef99-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fef99-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fef99-121">Request headers</span></span>

| <span data-ttu-id="fef99-122">标头</span><span class="sxs-lookup"><span data-stu-id="fef99-122">Header</span></span>        | <span data-ttu-id="fef99-123">值</span><span class="sxs-lookup"><span data-stu-id="fef99-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="fef99-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fef99-124">Authorization</span></span> | <span data-ttu-id="fef99-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fef99-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fef99-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fef99-127">Request body</span></span>

<span data-ttu-id="fef99-128">无。</span><span class="sxs-lookup"><span data-stu-id="fef99-128">None.</span></span>

><span data-ttu-id="fef99-129">**注意：** 使用从[列表发布应用程序](./teamsapp-list.md)的调用返回引用您想要更新的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="fef99-129">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="fef99-130">不要使用 zip 应用程序包的清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="fef99-130">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="fef99-131">响应</span><span class="sxs-lookup"><span data-stu-id="fef99-131">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="fef99-132">示例</span><span class="sxs-lookup"><span data-stu-id="fef99-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fef99-133">请求</span><span class="sxs-lookup"><span data-stu-id="fef99-133">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="fef99-134">响应</span><span class="sxs-lookup"><span data-stu-id="fef99-134">Response</span></span>

```http
HTTP/1.1 204 No Content
```
