---
title: 添加成员
description: 使用此 API 将成员（用户或组）添加到管理单元。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1c8eb575415f9063405b6c8d7c9891eb0cb9aaaf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441695"
---
# <a name="add-a-member"></a><span data-ttu-id="5b058-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="5b058-103">Add a member</span></span>

<span data-ttu-id="5b058-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5b058-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b058-105">使用此 API 将成员（用户或组）添加到管理单元。</span><span class="sxs-lookup"><span data-stu-id="5b058-105">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="5b058-106">权限</span><span class="sxs-lookup"><span data-stu-id="5b058-106">Permissions</span></span>
<span data-ttu-id="5b058-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5b058-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b058-109">Permission type</span></span>      | <span data-ttu-id="5b058-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b058-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b058-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b058-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5b058-112">AdministrativeUnit、Directory.accessasuser.all 和所有</span><span class="sxs-lookup"><span data-stu-id="5b058-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5b058-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b058-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b058-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b058-114">Not supported.</span></span>    |
|<span data-ttu-id="5b058-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b058-115">Application</span></span> | <span data-ttu-id="5b058-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b058-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b058-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b058-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5b058-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b058-118">Request headers</span></span>
| <span data-ttu-id="5b058-119">名称</span><span class="sxs-lookup"><span data-stu-id="5b058-119">Name</span></span>      |<span data-ttu-id="5b058-120">说明</span><span class="sxs-lookup"><span data-stu-id="5b058-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5b058-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b058-121">Authorization</span></span>  | <span data-ttu-id="5b058-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b058-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b058-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b058-124">Request body</span></span>
<span data-ttu-id="5b058-125">在请求正文中，提供要`id`添加的[用户](../resources/user.md)、[组](../resources/group.md)或[directoryObject](../resources/directoryobject.md) 。</span><span class="sxs-lookup"><span data-stu-id="5b058-125">In the request body, provide the `id` of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="5b058-126">响应</span><span class="sxs-lookup"><span data-stu-id="5b058-126">Response</span></span>

<span data-ttu-id="5b058-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5b058-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b058-129">示例</span><span class="sxs-lookup"><span data-stu-id="5b058-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b058-130">请求</span><span class="sxs-lookup"><span data-stu-id="5b058-130">Request</span></span>
<span data-ttu-id="5b058-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b058-131">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
<span data-ttu-id="5b058-132">在请求正文中，提供`id`要添加的[用户](../resources/user.md)或[组](../resources/group.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5b058-132">In the request body, provide the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

##### <a name="response"></a><span data-ttu-id="5b058-133">响应</span><span class="sxs-lookup"><span data-stu-id="5b058-133">Response</span></span>
<span data-ttu-id="5b058-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5b058-134">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
