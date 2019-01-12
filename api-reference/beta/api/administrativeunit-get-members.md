---
title: 获取成员
description: 使用此 API 获取一个管理单元中的特定成员 （用户或组）。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bbceccf30fdc3a9bd43fd25b8eda4cabdb4f7514
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931998"
---
# <a name="get-a-member"></a><span data-ttu-id="94d1a-103">获取成员</span><span class="sxs-lookup"><span data-stu-id="94d1a-103">Get a member</span></span>

> <span data-ttu-id="94d1a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="94d1a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94d1a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="94d1a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94d1a-106">使用此 API 获取一个管理单元中的特定成员 （用户或组）。</span><span class="sxs-lookup"><span data-stu-id="94d1a-106">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="94d1a-107">权限</span><span class="sxs-lookup"><span data-stu-id="94d1a-107">Permissions</span></span>
<span data-ttu-id="94d1a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94d1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="94d1a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="94d1a-110">Permission type</span></span>      | <span data-ttu-id="94d1a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94d1a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94d1a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94d1a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94d1a-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94d1a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="94d1a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94d1a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94d1a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="94d1a-115">Not supported.</span></span>    |
|<span data-ttu-id="94d1a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="94d1a-116">Application</span></span> | <span data-ttu-id="94d1a-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94d1a-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94d1a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94d1a-118">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="94d1a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="94d1a-119">Request headers</span></span>
| <span data-ttu-id="94d1a-120">名称</span><span class="sxs-lookup"><span data-stu-id="94d1a-120">Name</span></span>      |<span data-ttu-id="94d1a-121">说明</span><span class="sxs-lookup"><span data-stu-id="94d1a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94d1a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94d1a-122">Authorization</span></span>  | <span data-ttu-id="94d1a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94d1a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94d1a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="94d1a-125">Request body</span></span>
<span data-ttu-id="94d1a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94d1a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94d1a-127">响应</span><span class="sxs-lookup"><span data-stu-id="94d1a-127">Response</span></span>

<span data-ttu-id="94d1a-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[用户](../resources/user.md)或[组](../resources/group.md)对象。</span><span class="sxs-lookup"><span data-stu-id="94d1a-128">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94d1a-129">示例</span><span class="sxs-lookup"><span data-stu-id="94d1a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94d1a-130">请求</span><span class="sxs-lookup"><span data-stu-id="94d1a-130">Request</span></span>
<span data-ttu-id="94d1a-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94d1a-131">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="94d1a-132">响应</span><span class="sxs-lookup"><span data-stu-id="94d1a-132">Response</span></span>
<span data-ttu-id="94d1a-133">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="94d1a-133">Here is an example of the respone.</span></span> <span data-ttu-id="94d1a-134">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="94d1a-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="94d1a-135">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94d1a-135">All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "@odata.type":"#microsoft.graph.user",
  "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
  "accountEnabled":true,
  "businessPhones":[],
  "companyName":null,
  "displayName":"Demo User"
}
```
