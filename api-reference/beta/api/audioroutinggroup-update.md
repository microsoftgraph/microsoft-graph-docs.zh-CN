---
title: 更新音频路由组
description: 源和接收器 audioRoutingGroup 的修改。
ms.openlocfilehash: 6edbe0512b13de75645c3094b258de46c21956e9
ms.sourcegitcommit: 4a46cfd112c8089fc07e4e5ccdccaf415a3a0e7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2018
ms.locfileid: "27156024"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="b9e34-103">更新音频路由组</span><span class="sxs-lookup"><span data-stu-id="b9e34-103">Update audio routing group</span></span>

> <span data-ttu-id="b9e34-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b9e34-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9e34-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b9e34-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9e34-106">源和接收器[audioRoutingGroup](../resources/audioroutinggroup.md)的修改。</span><span class="sxs-lookup"><span data-stu-id="b9e34-106">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b9e34-107">权限</span><span class="sxs-lookup"><span data-stu-id="b9e34-107">Permissions</span></span>
<span data-ttu-id="b9e34-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9e34-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9e34-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9e34-110">Permission type</span></span> | <span data-ttu-id="b9e34-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9e34-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="b9e34-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e34-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9e34-113">不支持</span><span class="sxs-lookup"><span data-stu-id="b9e34-113">Not Supported</span></span>                       |
| <span data-ttu-id="b9e34-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e34-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9e34-115">不支持</span><span class="sxs-lookup"><span data-stu-id="b9e34-115">Not Supported</span></span>                       |
| <span data-ttu-id="b9e34-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9e34-116">Application</span></span>     | <span data-ttu-id="b9e34-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="b9e34-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9e34-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9e34-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b9e34-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9e34-119">Request headers</span></span>
| <span data-ttu-id="b9e34-120">名称</span><span class="sxs-lookup"><span data-stu-id="b9e34-120">Name</span></span>          | <span data-ttu-id="b9e34-121">说明</span><span class="sxs-lookup"><span data-stu-id="b9e34-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b9e34-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9e34-122">Authorization</span></span> | <span data-ttu-id="b9e34-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9e34-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9e34-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9e34-125">Request body</span></span>
<span data-ttu-id="b9e34-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="b9e34-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b9e34-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="b9e34-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b9e34-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b9e34-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b9e34-129">属性</span><span class="sxs-lookup"><span data-stu-id="b9e34-129">Property</span></span>       | <span data-ttu-id="b9e34-130">类型</span><span class="sxs-lookup"><span data-stu-id="b9e34-130">Type</span></span>    |<span data-ttu-id="b9e34-131">说明</span><span class="sxs-lookup"><span data-stu-id="b9e34-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b9e34-132">接收器</span><span class="sxs-lookup"><span data-stu-id="b9e34-132">receivers</span></span> | <span data-ttu-id="b9e34-133">String 集合</span><span class="sxs-lookup"><span data-stu-id="b9e34-133">String collection</span></span> | <span data-ttu-id="b9e34-134">AudioRoutingGroup 中的目标参与者。</span><span class="sxs-lookup"><span data-stu-id="b9e34-134">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="b9e34-135">routingMode</span><span class="sxs-lookup"><span data-stu-id="b9e34-135">routingMode</span></span> | <span data-ttu-id="b9e34-136">String</span><span class="sxs-lookup"><span data-stu-id="b9e34-136">String</span></span> | <span data-ttu-id="b9e34-137">可取值为：`oneToOne`、`multicast`。</span><span class="sxs-lookup"><span data-stu-id="b9e34-137">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="b9e34-138">sources</span><span class="sxs-lookup"><span data-stu-id="b9e34-138">sources</span></span> | <span data-ttu-id="b9e34-139">String 集合</span><span class="sxs-lookup"><span data-stu-id="b9e34-139">String collection</span></span> | <span data-ttu-id="b9e34-140">在 audioRoutingGroup 源参与者。</span><span class="sxs-lookup"><span data-stu-id="b9e34-140">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="b9e34-141">响应</span><span class="sxs-lookup"><span data-stu-id="b9e34-141">Response</span></span>
<span data-ttu-id="b9e34-142">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[audioRoutingGroup](../resources/audioroutinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b9e34-142">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9e34-143">示例</span><span class="sxs-lookup"><span data-stu-id="b9e34-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b9e34-144">请求</span><span class="sxs-lookup"><span data-stu-id="b9e34-144">Request</span></span>
<span data-ttu-id="b9e34-145">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9e34-145">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_audioRoutingGroup"
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
##### <a name="response"></a><span data-ttu-id="b9e34-146">响应</span><span class="sxs-lookup"><span data-stu-id="b9e34-146">Response</span></span>

> <span data-ttu-id="b9e34-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b9e34-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
