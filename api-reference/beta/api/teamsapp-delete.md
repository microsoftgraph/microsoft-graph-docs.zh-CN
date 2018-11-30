---
title: Permissions
description: '从组织的应用程序目录 （租户应用程序目录） 中删除应用程序。 '
ms.openlocfilehash: c3ee6433f38cfd52548af5ac27f3e3c9891af8d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049155"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="1810a-103">从组织的应用程序目录中删除应用程序</span><span class="sxs-lookup"><span data-stu-id="1810a-103">Remove an app from your organization's app catalog</span></span>

> <span data-ttu-id="1810a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1810a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1810a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1810a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1810a-106">从组织的应用程序目录 （租户应用程序目录） 中删除[应用程序](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="1810a-106">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="1810a-107">若要从您的组织的应用程序目录中删除您的应用程序，请指定`organization`作为**distributionMethod** [teamsCatalogApp](../resources/teamsapp.md)资源中。</span><span class="sxs-lookup"><span data-stu-id="1810a-107">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="1810a-108">权限</span><span class="sxs-lookup"><span data-stu-id="1810a-108">Permissions</span></span>

<span data-ttu-id="1810a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="1810a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="1810a-111">**注意：** 只有全局管理员可以调用此 API。</span><span class="sxs-lookup"><span data-stu-id="1810a-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="1810a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="1810a-112">Permission Type</span></span>                        | <span data-ttu-id="1810a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1810a-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="1810a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1810a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="1810a-115">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1810a-115">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="1810a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1810a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1810a-117">不支持</span><span class="sxs-lookup"><span data-stu-id="1810a-117">Not supported</span></span>|
| <span data-ttu-id="1810a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="1810a-118">Application</span></span>                            | <span data-ttu-id="1810a-119">不支持</span><span class="sxs-lookup"><span data-stu-id="1810a-119">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="1810a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1810a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1810a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1810a-121">Request headers</span></span>

| <span data-ttu-id="1810a-122">标头</span><span class="sxs-lookup"><span data-stu-id="1810a-122">Header</span></span>        | <span data-ttu-id="1810a-123">值</span><span class="sxs-lookup"><span data-stu-id="1810a-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="1810a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1810a-124">Authorization</span></span> | <span data-ttu-id="1810a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1810a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1810a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1810a-127">Request body</span></span>

<span data-ttu-id="1810a-128">无。</span><span class="sxs-lookup"><span data-stu-id="1810a-128">None.</span></span>

><span data-ttu-id="1810a-129">**注意：** 使用从[列表发布应用程序](./teamsapp-list.md)的调用返回引用您想要更新的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="1810a-129">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="1810a-130">不要使用 zip 应用程序包的清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="1810a-130">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="1810a-131">响应</span><span class="sxs-lookup"><span data-stu-id="1810a-131">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="1810a-132">示例</span><span class="sxs-lookup"><span data-stu-id="1810a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1810a-133">请求</span><span class="sxs-lookup"><span data-stu-id="1810a-133">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="1810a-134">响应</span><span class="sxs-lookup"><span data-stu-id="1810a-134">Response</span></span>

```http
HTTP/1.1 204 No Content
```
