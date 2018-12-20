---
title: 更新音频路由组
description: 源和接收器 audioRoutingGroup 的修改。
author: VinodRavichandran
ms.openlocfilehash: f1fac21e2d52818ee068bfe64e8db7853332d993
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380364"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="756dd-103">更新音频路由组</span><span class="sxs-lookup"><span data-stu-id="756dd-103">Update audio routing group</span></span>

> <span data-ttu-id="756dd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="756dd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="756dd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="756dd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="756dd-106">源和接收器[audioRoutingGroup](../resources/audioroutinggroup.md)的修改。</span><span class="sxs-lookup"><span data-stu-id="756dd-106">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="756dd-107">权限</span><span class="sxs-lookup"><span data-stu-id="756dd-107">Permissions</span></span>
<span data-ttu-id="756dd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="756dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="756dd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="756dd-110">Permission type</span></span> | <span data-ttu-id="756dd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="756dd-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="756dd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="756dd-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="756dd-113">不支持</span><span class="sxs-lookup"><span data-stu-id="756dd-113">Not Supported</span></span>                       |
| <span data-ttu-id="756dd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="756dd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="756dd-115">不支持</span><span class="sxs-lookup"><span data-stu-id="756dd-115">Not Supported</span></span>                       |
| <span data-ttu-id="756dd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="756dd-116">Application</span></span>     | <span data-ttu-id="756dd-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="756dd-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="756dd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="756dd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="756dd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="756dd-119">Request headers</span></span>
| <span data-ttu-id="756dd-120">名称</span><span class="sxs-lookup"><span data-stu-id="756dd-120">Name</span></span>          | <span data-ttu-id="756dd-121">说明</span><span class="sxs-lookup"><span data-stu-id="756dd-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="756dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="756dd-122">Authorization</span></span> | <span data-ttu-id="756dd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="756dd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="756dd-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="756dd-125">Request body</span></span>
<span data-ttu-id="756dd-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="756dd-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="756dd-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="756dd-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="756dd-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="756dd-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="756dd-129">属性</span><span class="sxs-lookup"><span data-stu-id="756dd-129">Property</span></span>       | <span data-ttu-id="756dd-130">类型</span><span class="sxs-lookup"><span data-stu-id="756dd-130">Type</span></span>    |<span data-ttu-id="756dd-131">说明</span><span class="sxs-lookup"><span data-stu-id="756dd-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="756dd-132">接收器</span><span class="sxs-lookup"><span data-stu-id="756dd-132">receivers</span></span> | <span data-ttu-id="756dd-133">String 集合</span><span class="sxs-lookup"><span data-stu-id="756dd-133">String collection</span></span> | <span data-ttu-id="756dd-134">AudioRoutingGroup 中的目标参与者。</span><span class="sxs-lookup"><span data-stu-id="756dd-134">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="756dd-135">routingMode</span><span class="sxs-lookup"><span data-stu-id="756dd-135">routingMode</span></span> | <span data-ttu-id="756dd-136">String</span><span class="sxs-lookup"><span data-stu-id="756dd-136">String</span></span> | <span data-ttu-id="756dd-137">可取值为：`oneToOne`、`multicast`。</span><span class="sxs-lookup"><span data-stu-id="756dd-137">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="756dd-138">sources</span><span class="sxs-lookup"><span data-stu-id="756dd-138">sources</span></span> | <span data-ttu-id="756dd-139">String 集合</span><span class="sxs-lookup"><span data-stu-id="756dd-139">String collection</span></span> | <span data-ttu-id="756dd-140">在 audioRoutingGroup 源参与者。</span><span class="sxs-lookup"><span data-stu-id="756dd-140">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="756dd-141">响应</span><span class="sxs-lookup"><span data-stu-id="756dd-141">Response</span></span>
<span data-ttu-id="756dd-142">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[audioRoutingGroup](../resources/audioroutinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="756dd-142">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="756dd-143">示例</span><span class="sxs-lookup"><span data-stu-id="756dd-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="756dd-144">请求</span><span class="sxs-lookup"><span data-stu-id="756dd-144">Request</span></span>
<span data-ttu-id="756dd-145">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="756dd-145">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update-audioRoutingGroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="756dd-146">响应</span><span class="sxs-lookup"><span data-stu-id="756dd-146">Response</span></span>

> <span data-ttu-id="756dd-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="756dd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->