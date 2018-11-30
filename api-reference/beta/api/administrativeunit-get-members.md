---
title: 获取成员
description: 使用此 API 获取一个管理单元中的特定成员 （用户或组）。
ms.openlocfilehash: 741a24434056783c3f008de6fb7694082b393092
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044287"
---
# <a name="get-a-member"></a><span data-ttu-id="6b492-103">获取成员</span><span class="sxs-lookup"><span data-stu-id="6b492-103">Get a member</span></span>

> <span data-ttu-id="6b492-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6b492-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b492-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6b492-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b492-106">使用此 API 获取一个管理单元中的特定成员 （用户或组）。</span><span class="sxs-lookup"><span data-stu-id="6b492-106">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b492-107">权限</span><span class="sxs-lookup"><span data-stu-id="6b492-107">Permissions</span></span>
<span data-ttu-id="6b492-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b492-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6b492-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b492-110">Permission type</span></span>      | <span data-ttu-id="6b492-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b492-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b492-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b492-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6b492-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6b492-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6b492-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b492-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b492-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b492-115">Not supported.</span></span>    |
|<span data-ttu-id="6b492-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b492-116">Application</span></span> | <span data-ttu-id="6b492-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b492-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b492-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b492-118">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6b492-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b492-119">Request headers</span></span>
| <span data-ttu-id="6b492-120">名称</span><span class="sxs-lookup"><span data-stu-id="6b492-120">Name</span></span>      |<span data-ttu-id="6b492-121">说明</span><span class="sxs-lookup"><span data-stu-id="6b492-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6b492-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b492-122">Authorization</span></span>  | <span data-ttu-id="6b492-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b492-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b492-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b492-125">Request body</span></span>
<span data-ttu-id="6b492-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6b492-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b492-127">响应</span><span class="sxs-lookup"><span data-stu-id="6b492-127">Response</span></span>

<span data-ttu-id="6b492-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[用户](../resources/user.md)或[组](../resources/group.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6b492-128">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b492-129">示例</span><span class="sxs-lookup"><span data-stu-id="6b492-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b492-130">请求</span><span class="sxs-lookup"><span data-stu-id="6b492-130">Request</span></span>
<span data-ttu-id="6b492-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b492-131">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="6b492-132">响应</span><span class="sxs-lookup"><span data-stu-id="6b492-132">Response</span></span>
<span data-ttu-id="6b492-133">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="6b492-133">Here is an example of the respone.</span></span> <span data-ttu-id="6b492-134">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6b492-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6b492-135">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b492-135">All of the properties will be returned from an actual call.</span></span>

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