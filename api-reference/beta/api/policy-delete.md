---
title: 删除策略
description: 删除策略。
localization_priority: Normal
ms.openlocfilehash: e4e5f5372e2904e1f74bc25224e3d2b1ce7ba154
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538726"
---
# <a name="delete-policy"></a><span data-ttu-id="c544d-103">删除策略</span><span class="sxs-lookup"><span data-stu-id="c544d-103">Delete Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c544d-104">删除[策略](../resources/policy.md)。</span><span class="sxs-lookup"><span data-stu-id="c544d-104">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c544d-105">权限</span><span class="sxs-lookup"><span data-stu-id="c544d-105">Permissions</span></span>
<span data-ttu-id="c544d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c544d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c544d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c544d-108">Permission type</span></span>      | <span data-ttu-id="c544d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c544d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c544d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c544d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c544d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c544d-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c544d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c544d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c544d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c544d-113">Not supported.</span></span>    |
|<span data-ttu-id="c544d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c544d-114">Application</span></span> | <span data-ttu-id="c544d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c544d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c544d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c544d-116">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c544d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c544d-117">Request headers</span></span>
| <span data-ttu-id="c544d-118">名称</span><span class="sxs-lookup"><span data-stu-id="c544d-118">Name</span></span>       | <span data-ttu-id="c544d-119">类型</span><span class="sxs-lookup"><span data-stu-id="c544d-119">Type</span></span> | <span data-ttu-id="c544d-120">说明</span><span class="sxs-lookup"><span data-stu-id="c544d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c544d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c544d-121">Authorization</span></span>  | <span data-ttu-id="c544d-122">string</span><span class="sxs-lookup"><span data-stu-id="c544d-122">string</span></span>  | <span data-ttu-id="c544d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c544d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c544d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c544d-125">Request body</span></span>
<span data-ttu-id="c544d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c544d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c544d-127">响应</span><span class="sxs-lookup"><span data-stu-id="c544d-127">Response</span></span>

<span data-ttu-id="c544d-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c544d-128">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="c544d-129">如果不成功 .。。</span><span class="sxs-lookup"><span data-stu-id="c544d-129">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="c544d-130">示例</span><span class="sxs-lookup"><span data-stu-id="c544d-130">Example</span></span>
<span data-ttu-id="c544d-131">下面的示例删除一个策略。</span><span class="sxs-lookup"><span data-stu-id="c544d-131">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="c544d-132">请求</span><span class="sxs-lookup"><span data-stu-id="c544d-132">Request</span></span>
<span data-ttu-id="c544d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c544d-133">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="c544d-134">响应</span><span class="sxs-lookup"><span data-stu-id="c544d-134">Response</span></span>
<span data-ttu-id="c544d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c544d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
