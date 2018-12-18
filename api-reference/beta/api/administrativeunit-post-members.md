---
title: 添加成员
description: 使用此 API 成员 （用户或组） 添加到一个管理单元。
author: lleonard-msft
ms.openlocfilehash: be47dbf06c5f59c0a4aaaea4f8c8b4aa8c3ce902
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339226"
---
# <a name="add-a-member"></a><span data-ttu-id="e4085-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="e4085-103">Add a member</span></span>

> <span data-ttu-id="e4085-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e4085-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4085-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e4085-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4085-106">使用此 API 成员 （用户或组） 添加到一个管理单元。</span><span class="sxs-lookup"><span data-stu-id="e4085-106">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="e4085-107">权限</span><span class="sxs-lookup"><span data-stu-id="e4085-107">Permissions</span></span>
<span data-ttu-id="e4085-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4085-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e4085-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4085-110">Permission type</span></span>      | <span data-ttu-id="e4085-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4085-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4085-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4085-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e4085-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e4085-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e4085-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4085-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4085-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4085-115">Not supported.</span></span>    |
|<span data-ttu-id="e4085-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4085-116">Application</span></span> | <span data-ttu-id="e4085-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4085-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4085-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4085-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e4085-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4085-119">Request headers</span></span>
| <span data-ttu-id="e4085-120">Name</span><span class="sxs-lookup"><span data-stu-id="e4085-120">Name</span></span>      |<span data-ttu-id="e4085-121">说明</span><span class="sxs-lookup"><span data-stu-id="e4085-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e4085-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4085-122">Authorization</span></span>  | <span data-ttu-id="e4085-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e4085-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4085-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4085-125">Request body</span></span>
<span data-ttu-id="e4085-126">在请求正文中，提供[用户](../resources/user.md)、[组](../resources/group.md)或[directoryObject](../resources/directoryobject.md)要添加的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4085-126">In the request body, supply a JSON representation of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="e4085-127">响应</span><span class="sxs-lookup"><span data-stu-id="e4085-127">Response</span></span>

<span data-ttu-id="e4085-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e4085-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4085-130">示例</span><span class="sxs-lookup"><span data-stu-id="e4085-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4085-131">请求</span><span class="sxs-lookup"><span data-stu-id="e4085-131">Request</span></span>
<span data-ttu-id="e4085-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4085-132">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
<span data-ttu-id="e4085-133">在请求正文中，提供的 JSON 表示形式`id`您想要添加的[用户](../resources/user.md)或[组](../resources/group.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e4085-133">In the request body, supply a JSON representation of the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

##### <a name="response"></a><span data-ttu-id="e4085-134">响应</span><span class="sxs-lookup"><span data-stu-id="e4085-134">Response</span></span>
<span data-ttu-id="e4085-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e4085-135">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
