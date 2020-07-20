---
title: 创建 connectorGroup
description: 创建 connectorGroup 对象。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7978a526884d6d1c1c8c286a9ea9caa4f01f4302
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006859"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="daf36-103">创建 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="daf36-103">Create connectorGroup</span></span>

<span data-ttu-id="daf36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daf36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daf36-105">创建[connectorGroup](../resources/connectorgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="daf36-105">Create a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="daf36-106">权限</span><span class="sxs-lookup"><span data-stu-id="daf36-106">Permissions</span></span>
<span data-ttu-id="daf36-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="daf36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daf36-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="daf36-109">Permission type</span></span>      | <span data-ttu-id="daf36-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="daf36-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="daf36-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="daf36-111">Delegated (work or school account)</span></span> | <span data-ttu-id="daf36-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="daf36-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="daf36-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="daf36-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daf36-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="daf36-114">Not supported.</span></span>    |
|<span data-ttu-id="daf36-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="daf36-115">Application</span></span> | <span data-ttu-id="daf36-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="daf36-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="daf36-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="daf36-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-request-headers"></a><span data-ttu-id="daf36-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="daf36-118">Optional request headers</span></span>
| <span data-ttu-id="daf36-119">名称</span><span class="sxs-lookup"><span data-stu-id="daf36-119">Name</span></span>       | <span data-ttu-id="daf36-120">说明</span><span class="sxs-lookup"><span data-stu-id="daf36-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="daf36-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="daf36-121">Authorization</span></span>  | <span data-ttu-id="daf36-122">负载.</span><span class="sxs-lookup"><span data-stu-id="daf36-122">Bearer.</span></span> <span data-ttu-id="daf36-123">必需。</span><span class="sxs-lookup"><span data-stu-id="daf36-123">Required.</span></span>|
| <span data-ttu-id="daf36-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="daf36-124">Content-type</span></span> | <span data-ttu-id="daf36-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="daf36-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="daf36-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="daf36-127">Request body</span></span>
<span data-ttu-id="daf36-128">在请求正文中，提供[connectorGroup](../resources/connectorgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="daf36-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>
<span data-ttu-id="daf36-129">下表列出了可用于**connectorGroup**的属性。</span><span class="sxs-lookup"><span data-stu-id="daf36-129">The following table lists the properties available for a **connectorGroup**.</span></span> <span data-ttu-id="daf36-130">**Name**属性是必需属性。</span><span class="sxs-lookup"><span data-stu-id="daf36-130">The **name** property is a required property.</span></span>

| <span data-ttu-id="daf36-131">属性</span><span class="sxs-lookup"><span data-stu-id="daf36-131">Property</span></span>     | <span data-ttu-id="daf36-132">类型</span><span class="sxs-lookup"><span data-stu-id="daf36-132">Type</span></span>   |<span data-ttu-id="daf36-133">说明</span><span class="sxs-lookup"><span data-stu-id="daf36-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="daf36-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="daf36-134">connectorGroupType</span></span>|<span data-ttu-id="daf36-135">string</span><span class="sxs-lookup"><span data-stu-id="daf36-135">string</span></span>| <span data-ttu-id="daf36-136">指示混合代理的类型。</span><span class="sxs-lookup"><span data-stu-id="daf36-136">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="daf36-137">此属性由系统预设。</span><span class="sxs-lookup"><span data-stu-id="daf36-137">This property is preset by the system.</span></span>|
|<span data-ttu-id="daf36-138">id</span><span class="sxs-lookup"><span data-stu-id="daf36-138">id</span></span>|<span data-ttu-id="daf36-139">string</span><span class="sxs-lookup"><span data-stu-id="daf36-139">string</span></span>| <span data-ttu-id="daf36-140">此 connectorGroup 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="daf36-140">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="daf36-141">只读。</span><span class="sxs-lookup"><span data-stu-id="daf36-141">Read-only.</span></span> |
|<span data-ttu-id="daf36-142">isDefault</span><span class="sxs-lookup"><span data-stu-id="daf36-142">isDefault</span></span>|<span data-ttu-id="daf36-143">boolean</span><span class="sxs-lookup"><span data-stu-id="daf36-143">boolean</span></span>| <span data-ttu-id="daf36-144">指示 connectorGroup 是否为默认值。</span><span class="sxs-lookup"><span data-stu-id="daf36-144">Indicates whether the connectorGroup is the default.</span></span> <span data-ttu-id="daf36-145">只有一个连接器组可以是默认的 connectorGroup，这是由系统预设的。</span><span class="sxs-lookup"><span data-stu-id="daf36-145">Only a single connector group can be the default connectorGroup and this is preset by the system.</span></span> |
|<span data-ttu-id="daf36-146">name</span><span class="sxs-lookup"><span data-stu-id="daf36-146">name</span></span>|<span data-ttu-id="daf36-147">string</span><span class="sxs-lookup"><span data-stu-id="daf36-147">string</span></span>| <span data-ttu-id="daf36-148">与 connectorGroup 关联的名称。</span><span class="sxs-lookup"><span data-stu-id="daf36-148">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="daf36-149">范围</span><span class="sxs-lookup"><span data-stu-id="daf36-149">region</span></span>|<span data-ttu-id="daf36-150">string</span><span class="sxs-lookup"><span data-stu-id="daf36-150">string</span></span>| <span data-ttu-id="daf36-151">向其分配 connectorGroup 的区域并将为其优化流量。</span><span class="sxs-lookup"><span data-stu-id="daf36-151">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="daf36-152">仅当**未**向 connectorGroup 分配连接器或应用程序时，才能设置此区域。</span><span class="sxs-lookup"><span data-stu-id="daf36-152">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="daf36-153">可用区域包括：北美、欧洲、澳大利亚、亚洲和印度。</span><span class="sxs-lookup"><span data-stu-id="daf36-153">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="daf36-154">可取值为：`nam`、`eur`、`aus`、`asia`、`ind`。</span><span class="sxs-lookup"><span data-stu-id="daf36-154">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="daf36-155">响应</span><span class="sxs-lookup"><span data-stu-id="daf36-155">Response</span></span>

<span data-ttu-id="daf36-156">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[connectorGroup](../resources/connectorgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="daf36-156">If successful, this method returns a `201 Created` response code and a [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="daf36-157">示例</span><span class="sxs-lookup"><span data-stu-id="daf36-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="daf36-158">请求</span><span class="sxs-lookup"><span data-stu-id="daf36-158">Request</span></span>
<span data-ttu-id="daf36-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="daf36-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="daf36-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="daf36-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "Connector Group Demo"

}
```
# <a name="c"></a>[<span data-ttu-id="daf36-161">C#</span><span class="sxs-lookup"><span data-stu-id="daf36-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="daf36-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="daf36-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="daf36-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="daf36-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="daf36-164">响应</span><span class="sxs-lookup"><span data-stu-id="daf36-164">Response</span></span>
<span data-ttu-id="daf36-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="daf36-165">The following is an example of the response.</span></span> 

><span data-ttu-id="daf36-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="daf36-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "3e6f4c35-a04b-4d03-b98a-66fff89b72e6",
  "name": "Connector Group Demo",
  "connectorGroupType": "applicationProxy",
  "isDefault": true,
  "region": "nam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
