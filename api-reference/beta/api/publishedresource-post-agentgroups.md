---
title: 将 publishedResource 分配给 onPremisesAgentGroup
description: 将**publishedResource**对象分配给**onPremisesAgentGroup**对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ec20b1208906129e5559307fc347e9d39c6dd7e
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840966"
---
# <a name="assign-publishedresource-to-onpremisesagentgroup"></a><span data-ttu-id="2b529-103">将 publishedResource 分配给 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="2b529-103">Assign publishedResource to onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b529-104">将[publishedResource](../resources/publishedresource.md)对象分配给[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2b529-104">Assign a [publishedResource](../resources/publishedresource.md) object to [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b529-105">权限</span><span class="sxs-lookup"><span data-stu-id="2b529-105">Permissions</span></span>

<span data-ttu-id="2b529-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b529-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b529-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b529-108">Permission type</span></span>                        | <span data-ttu-id="2b529-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b529-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="2b529-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b529-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b529-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="2b529-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="2b529-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b529-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b529-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b529-113">Not supported.</span></span> |
| <span data-ttu-id="2b529-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b529-114">Application</span></span>                            | <span data-ttu-id="2b529-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b529-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b529-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b529-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2b529-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b529-117">Request headers</span></span>

| <span data-ttu-id="2b529-118">名称</span><span class="sxs-lookup"><span data-stu-id="2b529-118">Name</span></span>          | <span data-ttu-id="2b529-119">说明</span><span class="sxs-lookup"><span data-stu-id="2b529-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2b529-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b529-120">Authorization</span></span> | <span data-ttu-id="2b529-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="2b529-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b529-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b529-122">Request body</span></span>

<span data-ttu-id="2b529-123">在请求正文中, 提供[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b529-123">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2b529-124">响应</span><span class="sxs-lookup"><span data-stu-id="2b529-124">Response</span></span>

<span data-ttu-id="2b529-125">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[publishedResource](../resources/publishedresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2b529-125">If successful, this method returns a `201 Created` response code and a [publishedResource](../resources/publishedresource.md) object  in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b529-126">示例</span><span class="sxs-lookup"><span data-stu-id="2b529-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b529-127">请求</span><span class="sxs-lookup"><span data-stu-id="2b529-127">Request</span></span>

<span data-ttu-id="2b529-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2b529-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b529-129">响应</span><span class="sxs-lookup"><span data-stu-id="2b529-129">Response</span></span>

<span data-ttu-id="2b529-130">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2b529-130">The following is an example of the response.</span></span>

> <span data-ttu-id="2b529-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2b529-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
