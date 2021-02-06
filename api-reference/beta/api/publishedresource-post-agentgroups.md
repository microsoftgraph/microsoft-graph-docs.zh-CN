---
title: 将 publishedResource 分配给 onPremisesAgentGroup
description: 将 **publishedResource** 对象分配给 **onPremisesAgentGroup** 对象。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 6e30689074c566511e638db484e7b29db6f9373e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130674"
---
# <a name="assign-publishedresource-to-onpremisesagentgroup"></a><span data-ttu-id="468bc-103">将 publishedResource 分配给 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="468bc-103">Assign publishedResource to onPremisesAgentGroup</span></span>

<span data-ttu-id="468bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="468bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="468bc-105">将 [publishedResource](../resources/publishedresource.md) 对象分配给 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="468bc-105">Assign a [publishedResource](../resources/publishedresource.md) object to [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="468bc-106">权限</span><span class="sxs-lookup"><span data-stu-id="468bc-106">Permissions</span></span>

<span data-ttu-id="468bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="468bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="468bc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="468bc-109">Permission type</span></span>                        | <span data-ttu-id="468bc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="468bc-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="468bc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="468bc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="468bc-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="468bc-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="468bc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="468bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="468bc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="468bc-114">Not supported.</span></span> |
| <span data-ttu-id="468bc-115">Application</span><span class="sxs-lookup"><span data-stu-id="468bc-115">Application</span></span>                            | <span data-ttu-id="468bc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="468bc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="468bc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="468bc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="468bc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="468bc-118">Request headers</span></span>

| <span data-ttu-id="468bc-119">名称</span><span class="sxs-lookup"><span data-stu-id="468bc-119">Name</span></span>          | <span data-ttu-id="468bc-120">说明</span><span class="sxs-lookup"><span data-stu-id="468bc-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="468bc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="468bc-121">Authorization</span></span> | <span data-ttu-id="468bc-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="468bc-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="468bc-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="468bc-123">Request body</span></span>

<span data-ttu-id="468bc-124">在请求正文中，提供 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="468bc-124">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="468bc-125">响应</span><span class="sxs-lookup"><span data-stu-id="468bc-125">Response</span></span>

<span data-ttu-id="468bc-126">如果成功，此方法在响应 `201 Created` 正文中返回响应代码和 [publishedResource](../resources/publishedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="468bc-126">If successful, this method returns a `201 Created` response code and a [publishedResource](../resources/publishedresource.md) object  in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="468bc-127">示例</span><span class="sxs-lookup"><span data-stu-id="468bc-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="468bc-128">请求</span><span class="sxs-lookup"><span data-stu-id="468bc-128">Request</span></span>

<span data-ttu-id="468bc-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="468bc-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisespublishingprofile"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
Content-type: application/json

```http
{
 "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/2B032383-897C-42BA-917E-700B6890BDC3/"
}
```

### <a name="response"></a><span data-ttu-id="468bc-130">响应</span><span class="sxs-lookup"><span data-stu-id="468bc-130">Response</span></span>

<span data-ttu-id="468bc-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="468bc-131">The following is an example of the response.</span></span>

> <span data-ttu-id="468bc-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="468bc-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 204
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



