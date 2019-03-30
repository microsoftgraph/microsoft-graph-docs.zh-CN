---
title: 确认 riskyUsers 已泄露
description: 确认 riskyUsers 对象是否已泄露。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 9ae07bf8d1d4a41764aa145a9c7508da339d7ce2
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/30/2019
ms.locfileid: "31013122"
---
# <a name="confirm-riskyusers-compromised"></a><span data-ttu-id="3156f-103">确认 riskyUsers 已泄露</span><span class="sxs-lookup"><span data-stu-id="3156f-103">Confirm riskyUsers compromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="3156f-104">**注意:** riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="3156f-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="3156f-105">确认[riskyUsers](../resources/riskyuser.md)对象是否已泄露。</span><span class="sxs-lookup"><span data-stu-id="3156f-105">Confirm a [riskyUsers](../resources/riskyuser.md) object as compromised.</span></span> <span data-ttu-id="3156f-106">这会将目标用户的风险级别设置为 "高"。</span><span class="sxs-lookup"><span data-stu-id="3156f-106">This will set the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="3156f-107">权限</span><span class="sxs-lookup"><span data-stu-id="3156f-107">Permissions</span></span>
<span data-ttu-id="3156f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3156f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3156f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3156f-110">Permission type</span></span>      | <span data-ttu-id="3156f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3156f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3156f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3156f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3156f-113">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="3156f-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="3156f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3156f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3156f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3156f-115">Not supported.</span></span>    |
|<span data-ttu-id="3156f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3156f-116">Application</span></span> | <span data-ttu-id="3156f-117">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="3156f-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3156f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3156f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="3156f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3156f-119">Request headers</span></span>
| <span data-ttu-id="3156f-120">名称</span><span class="sxs-lookup"><span data-stu-id="3156f-120">Name</span></span>      |<span data-ttu-id="3156f-121">说明</span><span class="sxs-lookup"><span data-stu-id="3156f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3156f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3156f-122">Authorization</span></span>  | <span data-ttu-id="3156f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3156f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3156f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3156f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3156f-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="3156f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3156f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3156f-128">Request body</span></span>
<span data-ttu-id="3156f-129">在请求正文中指定要消除的 userIds。</span><span class="sxs-lookup"><span data-stu-id="3156f-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="3156f-130">响应</span><span class="sxs-lookup"><span data-stu-id="3156f-130">Response</span></span>

<span data-ttu-id="3156f-131">如果成功, 此方法将`204 No Content`返回响应代码</span><span class="sxs-lookup"><span data-stu-id="3156f-131">If successful, this method returns a `204 No Content` response code</span></span>
## <a name="example"></a><span data-ttu-id="3156f-132">示例</span><span class="sxs-lookup"><span data-stu-id="3156f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3156f-133">请求</span><span class="sxs-lookup"><span data-stu-id="3156f-133">Request</span></span>
<span data-ttu-id="3156f-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3156f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/confirmCompromised


Request Body
{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="3156f-135">响应</span><span class="sxs-lookup"><span data-stu-id="3156f-135">Response</span></span>
<span data-ttu-id="3156f-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3156f-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 204 NoContent
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-confirmcompromised.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
