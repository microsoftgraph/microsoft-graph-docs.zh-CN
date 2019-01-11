---
title: 获取组
description: 检索与此 **educationClass** 对应的 Office 365 **group**。
localization_priority: Normal
ms.openlocfilehash: 9f84a1310fbc42d2f5e5a1b7e828dc90a71ab5fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866267"
---
# <a name="get-group"></a><span data-ttu-id="006a5-103">获取组</span><span class="sxs-lookup"><span data-stu-id="006a5-103">Get group</span></span>

> <span data-ttu-id="006a5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="006a5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="006a5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="006a5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="006a5-106">检索与此 **educationClass** 对应的 Office 365 **group**。</span><span class="sxs-lookup"><span data-stu-id="006a5-106">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="006a5-107">**注意：** 如果使用委派令牌，成员只能看到有关自己学校的信息。</span><span class="sxs-lookup"><span data-stu-id="006a5-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="006a5-108">在这种情况下，使用 `...beta/education/me/schools` 资源。</span><span class="sxs-lookup"><span data-stu-id="006a5-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="006a5-109">权限</span><span class="sxs-lookup"><span data-stu-id="006a5-109">Permissions</span></span>
<span data-ttu-id="006a5-110">要调用此 API，需要一组权限。</span><span class="sxs-lookup"><span data-stu-id="006a5-110">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="006a5-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="006a5-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="006a5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="006a5-112">Permission type</span></span>      | <span data-ttu-id="006a5-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="006a5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="006a5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="006a5-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="006a5-115">来自 EduRoster.ReadBasic、EduRoster.Read、EduRoster.Write 以及 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="006a5-115">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="006a5-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="006a5-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="006a5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="006a5-117">Not supported.</span></span>  |
|<span data-ttu-id="006a5-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="006a5-118">Application</span></span> | <span data-ttu-id="006a5-119">EduRoster.Read.All、EduRoster.ReadWrite.All 以及 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="006a5-119">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="006a5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="006a5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="006a5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="006a5-121">Request headers</span></span>
| <span data-ttu-id="006a5-122">标头</span><span class="sxs-lookup"><span data-stu-id="006a5-122">Header</span></span>       | <span data-ttu-id="006a5-123">值</span><span class="sxs-lookup"><span data-stu-id="006a5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="006a5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="006a5-124">Authorization</span></span>  | <span data-ttu-id="006a5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="006a5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="006a5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="006a5-127">Request body</span></span>
<span data-ttu-id="006a5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="006a5-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="006a5-129">响应</span><span class="sxs-lookup"><span data-stu-id="006a5-129">Response</span></span>
<span data-ttu-id="006a5-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="006a5-130">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="006a5-131">示例</span><span class="sxs-lookup"><span data-stu-id="006a5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="006a5-132">请求</span><span class="sxs-lookup"><span data-stu-id="006a5-132">Request</span></span>
<span data-ttu-id="006a5-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="006a5-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group
```
##### <a name="response"></a><span data-ttu-id="006a5-134">响应</span><span class="sxs-lookup"><span data-stu-id="006a5-134">Response</span></span>
<span data-ttu-id="006a5-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="006a5-135">The following is an example of the response.</span></span> 

><span data-ttu-id="006a5-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="006a5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 0087D9B3-1418-4C87-91C9-A18C6D93706B
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
