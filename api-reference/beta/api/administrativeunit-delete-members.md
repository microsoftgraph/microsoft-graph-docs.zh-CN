---
title: 删除成员
description: 使用此 API 可从管理单元中删除成员 (用户或组)。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 29ea8aa11850909c9e7122c55dc6c686ae9135a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459498"
---
# <a name="remove-a-member"></a><span data-ttu-id="dcef5-103">删除成员</span><span class="sxs-lookup"><span data-stu-id="dcef5-103">Remove a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcef5-104">使用此 API 可从管理单元中删除成员 (用户或组)。</span><span class="sxs-lookup"><span data-stu-id="dcef5-104">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcef5-105">权限</span><span class="sxs-lookup"><span data-stu-id="dcef5-105">Permissions</span></span>
<span data-ttu-id="dcef5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dcef5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dcef5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcef5-108">Permission type</span></span>      | <span data-ttu-id="dcef5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dcef5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcef5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcef5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dcef5-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dcef5-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dcef5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcef5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcef5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcef5-113">Not supported.</span></span>    |
|<span data-ttu-id="dcef5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dcef5-114">Application</span></span> | <span data-ttu-id="dcef5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcef5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcef5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcef5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="dcef5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="dcef5-117">Request headers</span></span>
| <span data-ttu-id="dcef5-118">名称</span><span class="sxs-lookup"><span data-stu-id="dcef5-118">Name</span></span>      |<span data-ttu-id="dcef5-119">说明</span><span class="sxs-lookup"><span data-stu-id="dcef5-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dcef5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcef5-120">Authorization</span></span>  | <span data-ttu-id="dcef5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dcef5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcef5-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcef5-123">Request body</span></span>
<span data-ttu-id="dcef5-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dcef5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcef5-125">响应</span><span class="sxs-lookup"><span data-stu-id="dcef5-125">Response</span></span>

<span data-ttu-id="dcef5-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dcef5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcef5-128">示例</span><span class="sxs-lookup"><span data-stu-id="dcef5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dcef5-129">请求</span><span class="sxs-lookup"><span data-stu-id="dcef5-129">Request</span></span>
<span data-ttu-id="dcef5-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dcef5-130">Here is an example of the request.</span></span> <span data-ttu-id="dcef5-131">在下面的示例中, id1 表示目标管理单元的标识符, id2 表示要从目标管理单元中删除的成员用户或组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dcef5-131">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="dcef5-132">响应</span><span class="sxs-lookup"><span data-stu-id="dcef5-132">Response</span></span>
<span data-ttu-id="dcef5-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dcef5-133">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-delete-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
