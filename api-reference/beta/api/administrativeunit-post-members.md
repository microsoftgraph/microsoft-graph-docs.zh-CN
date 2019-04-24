---
title: 添加成员
description: 使用此 API 将成员 (用户或组) 添加到管理单元。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c1cc9ce7e091ac96ca2484c74404c3a4b04b19ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459230"
---
# <a name="add-a-member"></a><span data-ttu-id="1d3f2-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="1d3f2-103">Add a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d3f2-104">使用此 API 将成员 (用户或组) 添加到管理单元。</span><span class="sxs-lookup"><span data-stu-id="1d3f2-104">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="1d3f2-105">权限</span><span class="sxs-lookup"><span data-stu-id="1d3f2-105">Permissions</span></span>
<span data-ttu-id="1d3f2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d3f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1d3f2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d3f2-108">Permission type</span></span>      | <span data-ttu-id="1d3f2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1d3f2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d3f2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d3f2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1d3f2-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d3f2-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d3f2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d3f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d3f2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d3f2-113">Not supported.</span></span>    |
|<span data-ttu-id="1d3f2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d3f2-114">Application</span></span> | <span data-ttu-id="1d3f2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d3f2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d3f2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d3f2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="1d3f2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d3f2-117">Request headers</span></span>
| <span data-ttu-id="1d3f2-118">名称</span><span class="sxs-lookup"><span data-stu-id="1d3f2-118">Name</span></span>      |<span data-ttu-id="1d3f2-119">说明</span><span class="sxs-lookup"><span data-stu-id="1d3f2-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1d3f2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d3f2-120">Authorization</span></span>  | <span data-ttu-id="1d3f2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1d3f2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d3f2-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d3f2-123">Request body</span></span>
<span data-ttu-id="1d3f2-124">在请求正文中, 提供要添加的[用户](../resources/user.md)、[组](../resources/group.md)或[directoryObject](../resources/directoryobject.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d3f2-124">In the request body, supply a JSON representation of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="1d3f2-125">响应</span><span class="sxs-lookup"><span data-stu-id="1d3f2-125">Response</span></span>

<span data-ttu-id="1d3f2-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1d3f2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d3f2-128">示例</span><span class="sxs-lookup"><span data-stu-id="1d3f2-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d3f2-129">请求</span><span class="sxs-lookup"><span data-stu-id="1d3f2-129">Request</span></span>
<span data-ttu-id="1d3f2-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1d3f2-130">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
<span data-ttu-id="1d3f2-131">在请求正文中, 提供要添加的[用户](../resources/user.md)或`id` [组](../resources/group.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d3f2-131">In the request body, supply a JSON representation of the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

##### <a name="response"></a><span data-ttu-id="1d3f2-132">响应</span><span class="sxs-lookup"><span data-stu-id="1d3f2-132">Response</span></span>
<span data-ttu-id="1d3f2-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1d3f2-133">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-post-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
