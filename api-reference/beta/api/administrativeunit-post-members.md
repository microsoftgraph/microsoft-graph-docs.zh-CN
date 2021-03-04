---
title: 添加成员
description: 使用此 API 将用户或 (组) 添加到管理单元。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6df32e3023752d3edf32163b3e99a377df8a5de1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438734"
---
# <a name="add-a-member"></a><span data-ttu-id="8ff98-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="8ff98-103">Add a member</span></span>

<span data-ttu-id="8ff98-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ff98-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ff98-105">使用此 API 将用户或 (组) 添加到管理单元。</span><span class="sxs-lookup"><span data-stu-id="8ff98-105">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="8ff98-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8ff98-106">Permissions</span></span>
<span data-ttu-id="8ff98-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ff98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8ff98-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ff98-109">Permission type</span></span>      | <span data-ttu-id="8ff98-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ff98-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ff98-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ff98-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8ff98-112">AdministrativeUnit.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8ff98-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8ff98-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ff98-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ff98-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ff98-114">Not supported.</span></span>    |
|<span data-ttu-id="8ff98-115">Application</span><span class="sxs-lookup"><span data-stu-id="8ff98-115">Application</span></span> | <span data-ttu-id="8ff98-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff98-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ff98-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ff98-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="8ff98-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ff98-118">Request headers</span></span>
| <span data-ttu-id="8ff98-119">名称</span><span class="sxs-lookup"><span data-stu-id="8ff98-119">Name</span></span>      |<span data-ttu-id="8ff98-120">说明</span><span class="sxs-lookup"><span data-stu-id="8ff98-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8ff98-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ff98-121">Authorization</span></span>  | <span data-ttu-id="8ff98-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ff98-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ff98-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ff98-124">Request body</span></span>
<span data-ttu-id="8ff98-125">在请求正文中，提供要添加的用户、组或 `id` [directoryObject。](../resources/directoryobject.md) [](../resources/user.md) [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="8ff98-125">In the request body, provide the `id` of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="8ff98-126">响应</span><span class="sxs-lookup"><span data-stu-id="8ff98-126">Response</span></span>

<span data-ttu-id="8ff98-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8ff98-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ff98-129">示例</span><span class="sxs-lookup"><span data-stu-id="8ff98-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ff98-130">请求</span><span class="sxs-lookup"><span data-stu-id="8ff98-130">Request</span></span>
<span data-ttu-id="8ff98-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ff98-131">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
<span data-ttu-id="8ff98-132">在请求正文中，提供 `id` [要](../resources/user.md) 添加的用户或 [组](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ff98-132">In the request body, provide the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

##### <a name="response"></a><span data-ttu-id="8ff98-133">响应</span><span class="sxs-lookup"><span data-stu-id="8ff98-133">Response</span></span>
<span data-ttu-id="8ff98-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8ff98-134">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```


