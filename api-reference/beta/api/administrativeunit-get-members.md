---
title: 获取成员
description: 使用此 API 获取管理单元中的特定成员（用户或组）。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a40542dff19460bf166753dcfbeb401bb22b0b53
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441751"
---
# <a name="get-a-member"></a><span data-ttu-id="8f94b-103">获取成员</span><span class="sxs-lookup"><span data-stu-id="8f94b-103">Get a member</span></span>

<span data-ttu-id="8f94b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8f94b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f94b-105">使用此 API 获取管理单元中的特定成员（用户或组）。</span><span class="sxs-lookup"><span data-stu-id="8f94b-105">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f94b-106">权限</span><span class="sxs-lookup"><span data-stu-id="8f94b-106">Permissions</span></span>
<span data-ttu-id="8f94b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f94b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8f94b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f94b-109">Permission type</span></span>      | <span data-ttu-id="8f94b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f94b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f94b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f94b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8f94b-112">AdministrativeUnit、AdministrativeUnit、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="8f94b-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8f94b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f94b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f94b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f94b-114">Not supported.</span></span>    |
|<span data-ttu-id="8f94b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f94b-115">Application</span></span> | <span data-ttu-id="8f94b-116">AdministrativeUnit、AdministrativeUnit、all、all、all、All 和所有的</span><span class="sxs-lookup"><span data-stu-id="8f94b-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f94b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f94b-117">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8f94b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f94b-118">Request headers</span></span>
| <span data-ttu-id="8f94b-119">名称</span><span class="sxs-lookup"><span data-stu-id="8f94b-119">Name</span></span>      |<span data-ttu-id="8f94b-120">说明</span><span class="sxs-lookup"><span data-stu-id="8f94b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8f94b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f94b-121">Authorization</span></span>  | <span data-ttu-id="8f94b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f94b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f94b-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f94b-124">Request body</span></span>
<span data-ttu-id="8f94b-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8f94b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f94b-126">响应</span><span class="sxs-lookup"><span data-stu-id="8f94b-126">Response</span></span>

<span data-ttu-id="8f94b-127">如果成功，此方法在响应`200 OK`正文中返回响应代码和[user](../resources/user.md)或[group](../resources/group.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8f94b-127">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f94b-128">示例</span><span class="sxs-lookup"><span data-stu-id="8f94b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f94b-129">请求</span><span class="sxs-lookup"><span data-stu-id="8f94b-129">Request</span></span>
<span data-ttu-id="8f94b-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f94b-130">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="8f94b-131">响应</span><span class="sxs-lookup"><span data-stu-id="8f94b-131">Response</span></span>
<span data-ttu-id="8f94b-132">下面是 respone 的一个示例。</span><span class="sxs-lookup"><span data-stu-id="8f94b-132">Here is an example of the respone.</span></span> <span data-ttu-id="8f94b-133">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8f94b-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8f94b-134">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f94b-134">All of the properties will be returned from an actual call.</span></span>

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
