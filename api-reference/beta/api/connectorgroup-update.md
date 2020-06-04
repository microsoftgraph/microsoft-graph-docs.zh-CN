---
title: 更新 connectorGroups
description: 更新 connectorgroup 对象的属性。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 80565045fa292b09e5c8e98544c466ec784f24f0
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44555799"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="0f06a-103">更新 connectorGroups</span><span class="sxs-lookup"><span data-stu-id="0f06a-103">Update connectorGroups</span></span>

<span data-ttu-id="0f06a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f06a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f06a-105">更新[connectorGroup](../resources/connectorgroup.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0f06a-105">Update the properties of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f06a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0f06a-106">Permissions</span></span>
<span data-ttu-id="0f06a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f06a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f06a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f06a-109">Permission type</span></span>      | <span data-ttu-id="0f06a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f06a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f06a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f06a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0f06a-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0f06a-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0f06a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f06a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f06a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f06a-114">Not supported.</span></span>    |
|<span data-ttu-id="0f06a-115">Application</span><span class="sxs-lookup"><span data-stu-id="0f06a-115">Application</span></span> | <span data-ttu-id="0f06a-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f06a-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f06a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f06a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0f06a-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="0f06a-118">Optional request headers</span></span>
| <span data-ttu-id="0f06a-119">名称</span><span class="sxs-lookup"><span data-stu-id="0f06a-119">Name</span></span>       | <span data-ttu-id="0f06a-120">说明</span><span class="sxs-lookup"><span data-stu-id="0f06a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0f06a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f06a-121">Authorization</span></span>  | <span data-ttu-id="0f06a-122">负载.</span><span class="sxs-lookup"><span data-stu-id="0f06a-122">Bearer.</span></span> <span data-ttu-id="0f06a-123">必需</span><span class="sxs-lookup"><span data-stu-id="0f06a-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f06a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f06a-124">Request body</span></span>
<span data-ttu-id="0f06a-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0f06a-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0f06a-128">属性</span><span class="sxs-lookup"><span data-stu-id="0f06a-128">Property</span></span>     | <span data-ttu-id="0f06a-129">类型</span><span class="sxs-lookup"><span data-stu-id="0f06a-129">Type</span></span>   |<span data-ttu-id="0f06a-130">说明</span><span class="sxs-lookup"><span data-stu-id="0f06a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f06a-131">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="0f06a-131">connectorGroupType</span></span>|<span data-ttu-id="0f06a-132">string</span><span class="sxs-lookup"><span data-stu-id="0f06a-132">string</span></span>| <span data-ttu-id="0f06a-133">指示混合代理的类型。</span><span class="sxs-lookup"><span data-stu-id="0f06a-133">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="0f06a-134">此项预设置的系统。</span><span class="sxs-lookup"><span data-stu-id="0f06a-134">This pre-set by the system.</span></span> |
|<span data-ttu-id="0f06a-135">id</span><span class="sxs-lookup"><span data-stu-id="0f06a-135">id</span></span>|<span data-ttu-id="0f06a-136">string</span><span class="sxs-lookup"><span data-stu-id="0f06a-136">string</span></span>| <span data-ttu-id="0f06a-137">此 connectorGroup 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0f06a-137">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="0f06a-138">只读。</span><span class="sxs-lookup"><span data-stu-id="0f06a-138">Read-only.</span></span> |
|<span data-ttu-id="0f06a-139">isDefault</span><span class="sxs-lookup"><span data-stu-id="0f06a-139">isDefault</span></span>|<span data-ttu-id="0f06a-140">boolean</span><span class="sxs-lookup"><span data-stu-id="0f06a-140">boolean</span></span>| <span data-ttu-id="0f06a-141">指示 connectorGroup 是否为默认的 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="0f06a-141">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="0f06a-142">只有一个连接器组可以是默认的 connectorGroup，这是由系统预设置的。</span><span class="sxs-lookup"><span data-stu-id="0f06a-142">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> |
|<span data-ttu-id="0f06a-143">name</span><span class="sxs-lookup"><span data-stu-id="0f06a-143">name</span></span>|<span data-ttu-id="0f06a-144">string</span><span class="sxs-lookup"><span data-stu-id="0f06a-144">string</span></span>| <span data-ttu-id="0f06a-145">与 connectorGroup 关联的名称。</span><span class="sxs-lookup"><span data-stu-id="0f06a-145">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="0f06a-146">范围</span><span class="sxs-lookup"><span data-stu-id="0f06a-146">region</span></span>|<span data-ttu-id="0f06a-147">string</span><span class="sxs-lookup"><span data-stu-id="0f06a-147">string</span></span>| <span data-ttu-id="0f06a-148">向其分配 connectorGroup 的区域并将为其优化流量。</span><span class="sxs-lookup"><span data-stu-id="0f06a-148">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="0f06a-149">仅当**未**向 connectorGroup 分配连接器或应用程序时，才能设置此区域。</span><span class="sxs-lookup"><span data-stu-id="0f06a-149">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="0f06a-150">可用区域包括：北美、欧洲、澳大利亚、亚洲和印度。</span><span class="sxs-lookup"><span data-stu-id="0f06a-150">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="0f06a-151">可取值为：`nam`、`eur`、`aus`、`asia`、`ind`。</span><span class="sxs-lookup"><span data-stu-id="0f06a-151">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="0f06a-152">响应</span><span class="sxs-lookup"><span data-stu-id="0f06a-152">Response</span></span>

<span data-ttu-id="0f06a-153">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[connectorGroup](../resources/connectorgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0f06a-153">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0f06a-154">示例</span><span class="sxs-lookup"><span data-stu-id="0f06a-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f06a-155">请求</span><span class="sxs-lookup"><span data-stu-id="0f06a-155">Request</span></span>
<span data-ttu-id="0f06a-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0f06a-156">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "region": "region-value"
}
```
##### <a name="response"></a><span data-ttu-id="0f06a-157">响应</span><span class="sxs-lookup"><span data-stu-id="0f06a-157">Response</span></span>
<span data-ttu-id="0f06a-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0f06a-158">The following is an example of the response.</span></span> <span data-ttu-id="0f06a-159">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0f06a-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0f06a-160">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0f06a-160">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": true,
  "region": "region-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
