---
title: 'privilegedApproval: myRequests'
description: 获取请求者的审批请求。
localization_priority: Normal
ms.openlocfilehash: 9fcbdab424c98633a8f543875b9b7c2275894df0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546666"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="95939-103">privilegedApproval: myRequests</span><span class="sxs-lookup"><span data-stu-id="95939-103">privilegedApproval: myRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95939-104">获取请求者的审批请求。</span><span class="sxs-lookup"><span data-stu-id="95939-104">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="95939-105">权限</span><span class="sxs-lookup"><span data-stu-id="95939-105">Permissions</span></span>
<span data-ttu-id="95939-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95939-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="95939-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="95939-108">Permission type</span></span>      | <span data-ttu-id="95939-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="95939-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95939-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95939-110">Delegated (work or school account)</span></span> | <span data-ttu-id="95939-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="95939-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="95939-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95939-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95939-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="95939-113">Not supported.</span></span>    |
|<span data-ttu-id="95939-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="95939-114">Application</span></span> | <span data-ttu-id="95939-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="95939-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="95939-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95939-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="95939-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="95939-117">Request headers</span></span>
| <span data-ttu-id="95939-118">名称</span><span class="sxs-lookup"><span data-stu-id="95939-118">Name</span></span>       | <span data-ttu-id="95939-119">说明</span><span class="sxs-lookup"><span data-stu-id="95939-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="95939-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="95939-120">Authorization</span></span>  | <span data-ttu-id="95939-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="95939-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95939-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="95939-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="95939-124">响应</span><span class="sxs-lookup"><span data-stu-id="95939-124">Response</span></span>

<span data-ttu-id="95939-125">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[privilegedApproval](../resources/privilegedapproval.md)对象。</span><span class="sxs-lookup"><span data-stu-id="95939-125">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="95939-126">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="95939-126">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="95939-127">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="95939-127">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="95939-128">示例</span><span class="sxs-lookup"><span data-stu-id="95939-128">Example</span></span>
<span data-ttu-id="95939-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="95939-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="95939-130">请求</span><span class="sxs-lookup"><span data-stu-id="95939-130">Request</span></span>
<span data-ttu-id="95939-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95939-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```

##### <a name="response"></a><span data-ttu-id="95939-132">响应</span><span class="sxs-lookup"><span data-stu-id="95939-132">Response</span></span>
<span data-ttu-id="95939-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95939-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval: myRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-myrequests.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
