---
title: connectorGroup 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: de405d2f0cbe0417271ab54e66c5c30073d8ee7f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517496"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="e6d2e-103">connectorGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6d2e-103">connectorGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="e6d2e-104">方法</span><span class="sxs-lookup"><span data-stu-id="e6d2e-104">Methods</span></span>

| <span data-ttu-id="e6d2e-105">方法</span><span class="sxs-lookup"><span data-stu-id="e6d2e-105">Method</span></span>           | <span data-ttu-id="e6d2e-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="e6d2e-106">Return Type</span></span>    |<span data-ttu-id="e6d2e-107">说明</span><span class="sxs-lookup"><span data-stu-id="e6d2e-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6d2e-108">获取 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="e6d2e-108">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="e6d2e-109">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="e6d2e-109">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="e6d2e-110">读取属性和 connectorGroup 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-110">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="e6d2e-111">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="e6d2e-111">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="e6d2e-112">application</span><span class="sxs-lookup"><span data-stu-id="e6d2e-112">application</span></span>](application.md)| <span data-ttu-id="e6d2e-113">将应用程序关联连接器组与发布到应用程序集合。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-113">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="e6d2e-114">应用程序列表</span><span class="sxs-lookup"><span data-stu-id="e6d2e-114">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="e6d2e-115">[应用程序](application.md)集合</span><span class="sxs-lookup"><span data-stu-id="e6d2e-115">[application](application.md) collection</span></span>| <span data-ttu-id="e6d2e-116">获取关联的应用程序对象集合。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-116">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="e6d2e-117">创建连接器</span><span class="sxs-lookup"><span data-stu-id="e6d2e-117">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="e6d2e-118">Connector</span><span class="sxs-lookup"><span data-stu-id="e6d2e-118">connector</span></span>](connector.md)| <span data-ttu-id="e6d2e-119">通过投递到 members 集合添加到组连接器的连接器。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-119">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="e6d2e-120">List members</span><span class="sxs-lookup"><span data-stu-id="e6d2e-120">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="e6d2e-121">[连接器](connector.md)集合</span><span class="sxs-lookup"><span data-stu-id="e6d2e-121">[connector](connector.md) collection</span></span>| <span data-ttu-id="e6d2e-122">获取一个连接器对象集合。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-122">Get a connector object collection.</span></span>|
|[<span data-ttu-id="e6d2e-123">Update</span><span class="sxs-lookup"><span data-stu-id="e6d2e-123">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="e6d2e-124">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="e6d2e-124">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="e6d2e-125">更新 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-125">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="e6d2e-126">删除</span><span class="sxs-lookup"><span data-stu-id="e6d2e-126">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="e6d2e-127">无</span><span class="sxs-lookup"><span data-stu-id="e6d2e-127">None</span></span> |<span data-ttu-id="e6d2e-128">删除 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-128">Delete connectorGroup object.</span></span> <span data-ttu-id="e6d2e-129">可以删除连接器组之前必须删除所有连接线。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-129">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="e6d2e-130">属性</span><span class="sxs-lookup"><span data-stu-id="e6d2e-130">Properties</span></span>
| <span data-ttu-id="e6d2e-131">属性</span><span class="sxs-lookup"><span data-stu-id="e6d2e-131">Property</span></span>     | <span data-ttu-id="e6d2e-132">类型</span><span class="sxs-lookup"><span data-stu-id="e6d2e-132">Type</span></span>   |<span data-ttu-id="e6d2e-133">说明</span><span class="sxs-lookup"><span data-stu-id="e6d2e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6d2e-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="e6d2e-134">connectorGroupType</span></span>|<span data-ttu-id="e6d2e-135">string</span><span class="sxs-lookup"><span data-stu-id="e6d2e-135">string</span></span>| <span data-ttu-id="e6d2e-136">将使用与组的连接器的类型。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-136">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="e6d2e-137">可能的值为： `applicationProxy`。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-137">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="e6d2e-138">id</span><span class="sxs-lookup"><span data-stu-id="e6d2e-138">id</span></span>|<span data-ttu-id="e6d2e-139">String</span><span class="sxs-lookup"><span data-stu-id="e6d2e-139">String</span></span>| <span data-ttu-id="e6d2e-140">ConnectorGroup 对象 id</span><span class="sxs-lookup"><span data-stu-id="e6d2e-140">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="e6d2e-141">isDefault</span><span class="sxs-lookup"><span data-stu-id="e6d2e-141">isDefault</span></span>|<span data-ttu-id="e6d2e-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6d2e-142">Boolean</span></span>| <span data-ttu-id="e6d2e-143">指示 connectorGroup 是默认连接器组。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-143">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="e6d2e-144">仅限单个连接器组可以是默认 connectorGroup 并且由系统设置。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-144">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="e6d2e-145">name</span><span class="sxs-lookup"><span data-stu-id="e6d2e-145">name</span></span>|<span data-ttu-id="e6d2e-146">String</span><span class="sxs-lookup"><span data-stu-id="e6d2e-146">String</span></span>| <span data-ttu-id="e6d2e-147">与 connectorGroup 关联的名称。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-147">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6d2e-148">关系</span><span class="sxs-lookup"><span data-stu-id="e6d2e-148">Relationships</span></span>
| <span data-ttu-id="e6d2e-149">关系</span><span class="sxs-lookup"><span data-stu-id="e6d2e-149">Relationship</span></span> | <span data-ttu-id="e6d2e-150">类型</span><span class="sxs-lookup"><span data-stu-id="e6d2e-150">Type</span></span>   |<span data-ttu-id="e6d2e-151">说明</span><span class="sxs-lookup"><span data-stu-id="e6d2e-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6d2e-152">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6d2e-152">applications</span></span>|<span data-ttu-id="e6d2e-153">[应用程序](application.md)集合</span><span class="sxs-lookup"><span data-stu-id="e6d2e-153">[application](application.md) collection</span></span>| <span data-ttu-id="e6d2e-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="e6d2e-156">members</span><span class="sxs-lookup"><span data-stu-id="e6d2e-156">members</span></span>|<span data-ttu-id="e6d2e-157">[连接器](connector.md)集合</span><span class="sxs-lookup"><span data-stu-id="e6d2e-157">[connector](connector.md) collection</span></span>| <span data-ttu-id="e6d2e-p105">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6d2e-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6d2e-160">JSON representation</span></span>

<span data-ttu-id="e6d2e-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6d2e-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "connectorGroupType": "string",
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connectorgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
