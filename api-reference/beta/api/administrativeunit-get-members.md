---
title: 获取成员
description: 使用此 API 获取管理单元中的特定成员 (用户或组)。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7bf15df8dc61bb8f86eb21aa748a3bcf96588976
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322823"
---
# <a name="get-a-member"></a><span data-ttu-id="86149-103">获取成员</span><span class="sxs-lookup"><span data-stu-id="86149-103">Get a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86149-104">使用此 API 获取管理单元中的特定成员 (用户或组)。</span><span class="sxs-lookup"><span data-stu-id="86149-104">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="86149-105">权限</span><span class="sxs-lookup"><span data-stu-id="86149-105">Permissions</span></span>
<span data-ttu-id="86149-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86149-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="86149-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="86149-108">Permission type</span></span>      | <span data-ttu-id="86149-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86149-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86149-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86149-110">Delegated (work or school account)</span></span> | <span data-ttu-id="86149-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="86149-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="86149-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86149-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86149-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="86149-113">Not supported.</span></span>    |
|<span data-ttu-id="86149-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="86149-114">Application</span></span> | <span data-ttu-id="86149-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86149-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="86149-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86149-116">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="86149-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="86149-117">Request headers</span></span>
| <span data-ttu-id="86149-118">名称</span><span class="sxs-lookup"><span data-stu-id="86149-118">Name</span></span>      |<span data-ttu-id="86149-119">说明</span><span class="sxs-lookup"><span data-stu-id="86149-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="86149-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="86149-120">Authorization</span></span>  | <span data-ttu-id="86149-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="86149-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86149-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="86149-123">Request body</span></span>
<span data-ttu-id="86149-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="86149-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86149-125">响应</span><span class="sxs-lookup"><span data-stu-id="86149-125">Response</span></span>

<span data-ttu-id="86149-126">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[user](../resources/user.md)或[group](../resources/group.md)对象。</span><span class="sxs-lookup"><span data-stu-id="86149-126">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86149-127">示例</span><span class="sxs-lookup"><span data-stu-id="86149-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86149-128">请求</span><span class="sxs-lookup"><span data-stu-id="86149-128">Request</span></span>
<span data-ttu-id="86149-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86149-129">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="86149-130">响应</span><span class="sxs-lookup"><span data-stu-id="86149-130">Response</span></span>
<span data-ttu-id="86149-131">下面是 respone 的一个示例。</span><span class="sxs-lookup"><span data-stu-id="86149-131">Here is an example of the respone.</span></span> <span data-ttu-id="86149-132">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="86149-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="86149-133">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="86149-133">All of the properties will be returned from an actual call.</span></span>

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
