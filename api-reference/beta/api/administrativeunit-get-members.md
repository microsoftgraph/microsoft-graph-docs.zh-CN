---
title: 获取成员
description: 使用此 API 获取管理单元中的特定成员 (用户或组)。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3a9752d37fed21ebadbd0e05cc30831b13f30ef5
ms.sourcegitcommit: 27e8ddb53b699f70b676c9648db8f06bb8d831a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/27/2019
ms.locfileid: "35917948"
---
# <a name="get-a-member"></a><span data-ttu-id="c4d3c-103">获取成员</span><span class="sxs-lookup"><span data-stu-id="c4d3c-103">Get a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4d3c-104">使用此 API 获取管理单元中的特定成员 (用户或组)。</span><span class="sxs-lookup"><span data-stu-id="c4d3c-104">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4d3c-105">权限</span><span class="sxs-lookup"><span data-stu-id="c4d3c-105">Permissions</span></span>
<span data-ttu-id="c4d3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4d3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c4d3c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4d3c-108">Permission type</span></span>      | <span data-ttu-id="c4d3c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4d3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4d3c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4d3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c4d3c-111">AdministrativeUnit、AdministrativeUnit、all、Directory.accessasuser.all。 All</span><span class="sxs-lookup"><span data-stu-id="c4d3c-111">AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c4d3c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4d3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4d3c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4d3c-113">Not supported.</span></span>    |
|<span data-ttu-id="c4d3c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4d3c-114">Application</span></span> | <span data-ttu-id="c4d3c-115">AdministrativeUnit、AdministrativeUnit 和所有</span><span class="sxs-lookup"><span data-stu-id="c4d3c-115">AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4d3c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4d3c-116">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c4d3c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4d3c-117">Request headers</span></span>
| <span data-ttu-id="c4d3c-118">名称</span><span class="sxs-lookup"><span data-stu-id="c4d3c-118">Name</span></span>      |<span data-ttu-id="c4d3c-119">说明</span><span class="sxs-lookup"><span data-stu-id="c4d3c-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c4d3c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4d3c-120">Authorization</span></span>  | <span data-ttu-id="c4d3c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4d3c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4d3c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4d3c-123">Request body</span></span>
<span data-ttu-id="c4d3c-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c4d3c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4d3c-125">响应</span><span class="sxs-lookup"><span data-stu-id="c4d3c-125">Response</span></span>

<span data-ttu-id="c4d3c-126">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[user](../resources/user.md)或[group](../resources/group.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c4d3c-126">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4d3c-127">示例</span><span class="sxs-lookup"><span data-stu-id="c4d3c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4d3c-128">请求</span><span class="sxs-lookup"><span data-stu-id="c4d3c-128">Request</span></span>
<span data-ttu-id="c4d3c-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4d3c-129">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="c4d3c-130">响应</span><span class="sxs-lookup"><span data-stu-id="c4d3c-130">Response</span></span>
<span data-ttu-id="c4d3c-131">下面是 respone 的一个示例。</span><span class="sxs-lookup"><span data-stu-id="c4d3c-131">Here is an example of the respone.</span></span> <span data-ttu-id="c4d3c-132">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c4d3c-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c4d3c-133">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c4d3c-133">All of the properties will be returned from an actual call.</span></span>

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
