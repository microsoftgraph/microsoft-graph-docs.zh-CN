---
title: 权限
description: '将应用程序发布到 Microsoft 团队应用程序目录。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c50b183819d7f56c6d5317a6e30840b674be750a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990783"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="ec2c1-103">将应用程序发布到你的组织的应用程序目录</span><span class="sxs-lookup"><span data-stu-id="ec2c1-103">Publish apps to your organization's app catalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec2c1-104">将[应用程序](../resources/teamsapp.md)发布到 Microsoft 团队应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="ec2c1-104">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span> <span data-ttu-id="ec2c1-105">具体而言, 此 API 会将应用程序发布到您的组织的目录 (租户应用程序目录);创建的资源将具有`distributionMethod`  =  `organization`。</span><span class="sxs-lookup"><span data-stu-id="ec2c1-105">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec2c1-106">权限</span><span class="sxs-lookup"><span data-stu-id="ec2c1-106">Permissions</span></span>

<span data-ttu-id="ec2c1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="ec2c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="ec2c1-109">**注意:** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="ec2c1-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="ec2c1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec2c1-110">Permission Type</span></span>                        | <span data-ttu-id="ec2c1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec2c1-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="ec2c1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec2c1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec2c1-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec2c1-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="ec2c1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec2c1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec2c1-115">不支持</span><span class="sxs-lookup"><span data-stu-id="ec2c1-115">Not supported</span></span>|
| <span data-ttu-id="ec2c1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec2c1-116">Application</span></span>                            | <span data-ttu-id="ec2c1-117">不支持</span><span class="sxs-lookup"><span data-stu-id="ec2c1-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec2c1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec2c1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="ec2c1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec2c1-119">Request headers</span></span>

| <span data-ttu-id="ec2c1-120">标头</span><span class="sxs-lookup"><span data-stu-id="ec2c1-120">Header</span></span>        | <span data-ttu-id="ec2c1-121">值</span><span class="sxs-lookup"><span data-stu-id="ec2c1-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="ec2c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec2c1-122">Authorization</span></span> | <span data-ttu-id="ec2c1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec2c1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ec2c1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec2c1-125">Content-Type</span></span>  | <span data-ttu-id="ec2c1-126">application/zip</span><span class="sxs-lookup"><span data-stu-id="ec2c1-126">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec2c1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec2c1-127">Request body</span></span>

<span data-ttu-id="ec2c1-128">团队 Zip 清单有效负载。</span><span class="sxs-lookup"><span data-stu-id="ec2c1-128">Teams Zip Manifest Payload.</span></span> <span data-ttu-id="ec2c1-129">对于 "团队应用程序 zip 文件",[请参阅创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="ec2c1-129">For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> <span data-ttu-id="ec2c1-130">您不能为与该组织中的另一个应用程序具有相同清单 ID 的组织创建应用程序。</span><span class="sxs-lookup"><span data-stu-id="ec2c1-130">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="ec2c1-131">响应</span><span class="sxs-lookup"><span data-stu-id="ec2c1-131">Response</span></span>

<span data-ttu-id="ec2c1-132">如果成功, 此方法将`200 OK`返回响应代码和[teamsCatalogApp](../resources/teamsapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ec2c1-132">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="ec2c1-133">示例</span><span class="sxs-lookup"><span data-stu-id="ec2c1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec2c1-134">请求</span><span class="sxs-lookup"><span data-stu-id="ec2c1-134">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="ec2c1-135">有关如何创建 Microsoft 团队应用程序 zip 文件的信息, 请参阅[创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="ec2c1-135">For information about how to create a Microsoft Teams application zip file, see [Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> 

### <a name="response"></a><span data-ttu-id="ec2c1-136">响应</span><span class="sxs-lookup"><span data-stu-id="ec2c1-136">Response</span></span>

```
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```
