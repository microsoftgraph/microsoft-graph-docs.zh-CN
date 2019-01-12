---
title: 权限
description: '从组织的应用程序目录 （租户应用程序目录） 中删除应用程序。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 58984044ea59bd38f0232bfa9407c01f97f22708
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943604"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="b4383-103">从组织的应用程序目录中删除应用程序</span><span class="sxs-lookup"><span data-stu-id="b4383-103">Remove an app from your organization's app catalog</span></span>



<span data-ttu-id="b4383-104">从组织的应用程序目录 （租户应用程序目录） 中删除[应用程序](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="b4383-104">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="b4383-105">若要从您的组织的应用程序目录中删除您的应用程序，请指定`organization`作为**distributionMethod** [teamsCatalogApp](../resources/teamsapp.md)资源中。</span><span class="sxs-lookup"><span data-stu-id="b4383-105">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4383-106">权限</span><span class="sxs-lookup"><span data-stu-id="b4383-106">Permissions</span></span>

<span data-ttu-id="b4383-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="b4383-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="b4383-109">**注意：** 只有全局管理员可以调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b4383-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="b4383-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4383-110">Permission Type</span></span>                        | <span data-ttu-id="b4383-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4383-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="b4383-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4383-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4383-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4383-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="b4383-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4383-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4383-115">不支持</span><span class="sxs-lookup"><span data-stu-id="b4383-115">Not supported</span></span>|
| <span data-ttu-id="b4383-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4383-116">Application</span></span>                            | <span data-ttu-id="b4383-117">不支持</span><span class="sxs-lookup"><span data-stu-id="b4383-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4383-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4383-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b4383-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4383-119">Request headers</span></span>

| <span data-ttu-id="b4383-120">标头</span><span class="sxs-lookup"><span data-stu-id="b4383-120">Header</span></span>        | <span data-ttu-id="b4383-121">值</span><span class="sxs-lookup"><span data-stu-id="b4383-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="b4383-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4383-122">Authorization</span></span> | <span data-ttu-id="b4383-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4383-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4383-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4383-125">Request body</span></span>

<span data-ttu-id="b4383-126">无。</span><span class="sxs-lookup"><span data-stu-id="b4383-126">None.</span></span>

><span data-ttu-id="b4383-127">**注意：** 使用从[列表发布应用程序](./teamsapp-list.md)的调用返回引用您想要更新的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="b4383-127">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="b4383-128">不要使用 zip 应用程序包的清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="b4383-128">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="b4383-129">响应</span><span class="sxs-lookup"><span data-stu-id="b4383-129">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="b4383-130">示例</span><span class="sxs-lookup"><span data-stu-id="b4383-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4383-131">请求</span><span class="sxs-lookup"><span data-stu-id="b4383-131">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="b4383-132">响应</span><span class="sxs-lookup"><span data-stu-id="b4383-132">Response</span></span>

```http
HTTP/1.1 204 No Content
```
