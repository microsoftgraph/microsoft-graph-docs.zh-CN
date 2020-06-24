---
title: 创建 connectorGroup
description: 创建 connectorGroup 对象。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2ddc1aebfeb64e4dd596f94dd8a91f3718a29fb7
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863262"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="31a9c-103">创建 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="31a9c-103">Create connectorGroup</span></span>

<span data-ttu-id="31a9c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31a9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31a9c-105">创建[connectorGroup](../resources/connectorgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="31a9c-105">Create a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="31a9c-106">权限</span><span class="sxs-lookup"><span data-stu-id="31a9c-106">Permissions</span></span>
<span data-ttu-id="31a9c-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="31a9c-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="31a9c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31a9c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31a9c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="31a9c-109">Permission type</span></span>      | <span data-ttu-id="31a9c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31a9c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31a9c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31a9c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="31a9c-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="31a9c-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="31a9c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31a9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31a9c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="31a9c-114">Not supported.</span></span>    |
|<span data-ttu-id="31a9c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="31a9c-115">Application</span></span> | <span data-ttu-id="31a9c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="31a9c-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="31a9c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31a9c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-request-headers"></a><span data-ttu-id="31a9c-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="31a9c-118">Optional request headers</span></span>
| <span data-ttu-id="31a9c-119">名称</span><span class="sxs-lookup"><span data-stu-id="31a9c-119">Name</span></span>       | <span data-ttu-id="31a9c-120">说明</span><span class="sxs-lookup"><span data-stu-id="31a9c-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="31a9c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="31a9c-121">Authorization</span></span>  | <span data-ttu-id="31a9c-122">负载.</span><span class="sxs-lookup"><span data-stu-id="31a9c-122">Bearer.</span></span> <span data-ttu-id="31a9c-123">必需。</span><span class="sxs-lookup"><span data-stu-id="31a9c-123">Required.</span></span>|
| <span data-ttu-id="31a9c-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="31a9c-124">Content-type</span></span> | <span data-ttu-id="31a9c-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="31a9c-125">application/json.</span></span> <span data-ttu-id="31a9c-126">Required.</span><span class="sxs-lookup"><span data-stu-id="31a9c-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31a9c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="31a9c-127">Request body</span></span>
<span data-ttu-id="31a9c-128">在请求正文中，提供[connectorGroup](../resources/connectorgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31a9c-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>
<span data-ttu-id="31a9c-129">下表列出了可用于**connectorGroup**的属性。</span><span class="sxs-lookup"><span data-stu-id="31a9c-129">The following table lists the properties available for a **connectorGroup**.</span></span> <span data-ttu-id="31a9c-130">**Name**属性是必需属性。</span><span class="sxs-lookup"><span data-stu-id="31a9c-130">The **name** property is a required property.</span></span>

| <span data-ttu-id="31a9c-131">属性</span><span class="sxs-lookup"><span data-stu-id="31a9c-131">Property</span></span>     | <span data-ttu-id="31a9c-132">类型</span><span class="sxs-lookup"><span data-stu-id="31a9c-132">Type</span></span>   |<span data-ttu-id="31a9c-133">Description</span><span class="sxs-lookup"><span data-stu-id="31a9c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31a9c-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="31a9c-134">connectorGroupType</span></span>|<span data-ttu-id="31a9c-135">字符串</span><span class="sxs-lookup"><span data-stu-id="31a9c-135">string</span></span>| <span data-ttu-id="31a9c-136">指示混合代理的类型。</span><span class="sxs-lookup"><span data-stu-id="31a9c-136">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="31a9c-137">此属性由系统预设。</span><span class="sxs-lookup"><span data-stu-id="31a9c-137">This property is preset by the system.</span></span>|
|<span data-ttu-id="31a9c-138">id</span><span class="sxs-lookup"><span data-stu-id="31a9c-138">id</span></span>|<span data-ttu-id="31a9c-139">string</span><span class="sxs-lookup"><span data-stu-id="31a9c-139">string</span></span>| <span data-ttu-id="31a9c-140">此 connectorGroup 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="31a9c-140">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="31a9c-141">只读。</span><span class="sxs-lookup"><span data-stu-id="31a9c-141">Read-only.</span></span> |
|<span data-ttu-id="31a9c-142">isDefault</span><span class="sxs-lookup"><span data-stu-id="31a9c-142">isDefault</span></span>|<span data-ttu-id="31a9c-143">boolean</span><span class="sxs-lookup"><span data-stu-id="31a9c-143">boolean</span></span>| <span data-ttu-id="31a9c-144">指示 connectorGroup 是否为默认值。</span><span class="sxs-lookup"><span data-stu-id="31a9c-144">Indicates whether the connectorGroup is the default.</span></span> <span data-ttu-id="31a9c-145">只有一个连接器组可以是默认的 connectorGroup，这是由系统预设的。</span><span class="sxs-lookup"><span data-stu-id="31a9c-145">Only a single connector group can be the default connectorGroup and this is preset by the system.</span></span> |
|<span data-ttu-id="31a9c-146">name</span><span class="sxs-lookup"><span data-stu-id="31a9c-146">name</span></span>|<span data-ttu-id="31a9c-147">string</span><span class="sxs-lookup"><span data-stu-id="31a9c-147">string</span></span>| <span data-ttu-id="31a9c-148">与 connectorGroup 关联的名称。</span><span class="sxs-lookup"><span data-stu-id="31a9c-148">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="31a9c-149">范围</span><span class="sxs-lookup"><span data-stu-id="31a9c-149">region</span></span>|<span data-ttu-id="31a9c-150">字符串</span><span class="sxs-lookup"><span data-stu-id="31a9c-150">string</span></span>| <span data-ttu-id="31a9c-151">向其分配 connectorGroup 的区域并将为其优化流量。</span><span class="sxs-lookup"><span data-stu-id="31a9c-151">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="31a9c-152">仅当**未**向 connectorGroup 分配连接器或应用程序时，才能设置此区域。</span><span class="sxs-lookup"><span data-stu-id="31a9c-152">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="31a9c-153">可用区域包括：北美、欧洲、澳大利亚、亚洲和印度。</span><span class="sxs-lookup"><span data-stu-id="31a9c-153">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="31a9c-154">可取值为：`nam`、`eur`、`aus`、`asia`、`ind`。</span><span class="sxs-lookup"><span data-stu-id="31a9c-154">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="31a9c-155">响应</span><span class="sxs-lookup"><span data-stu-id="31a9c-155">Response</span></span>

<span data-ttu-id="31a9c-156">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[connectorGroup](../resources/connectorgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="31a9c-156">If successful, this method returns a `201 Created` response code and a [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31a9c-157">示例</span><span class="sxs-lookup"><span data-stu-id="31a9c-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="31a9c-158">请求</span><span class="sxs-lookup"><span data-stu-id="31a9c-158">Request</span></span>
<span data-ttu-id="31a9c-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="31a9c-159">The following is an example of the request.</span></span>
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
### <a name="response"></a><span data-ttu-id="31a9c-160">响应</span><span class="sxs-lookup"><span data-stu-id="31a9c-160">Response</span></span>
<span data-ttu-id="31a9c-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="31a9c-161">The following is an example of the response.</span></span> 

><span data-ttu-id="31a9c-162">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="31a9c-162">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="31a9c-163">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="31a9c-163">All the properties will be returned from an actual call.</span></span>
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
