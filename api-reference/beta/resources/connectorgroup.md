---
title: connectorGroup 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: de405d2f0cbe0417271ab54e66c5c30073d8ee7f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543390"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="9ca29-103">connectorGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ca29-103">connectorGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="9ca29-104">方法</span><span class="sxs-lookup"><span data-stu-id="9ca29-104">Methods</span></span>

| <span data-ttu-id="9ca29-105">方法</span><span class="sxs-lookup"><span data-stu-id="9ca29-105">Method</span></span>           | <span data-ttu-id="9ca29-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="9ca29-106">Return Type</span></span>    |<span data-ttu-id="9ca29-107">说明</span><span class="sxs-lookup"><span data-stu-id="9ca29-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9ca29-108">获取 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="9ca29-108">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="9ca29-109">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="9ca29-109">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="9ca29-110">读取 connectorGroup 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9ca29-110">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="9ca29-111">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="9ca29-111">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="9ca29-112">application</span><span class="sxs-lookup"><span data-stu-id="9ca29-112">application</span></span>](application.md)| <span data-ttu-id="9ca29-113">将应用程序与连接器组关联, 方法是发布到应用程序集合。</span><span class="sxs-lookup"><span data-stu-id="9ca29-113">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="9ca29-114">列出应用程序</span><span class="sxs-lookup"><span data-stu-id="9ca29-114">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="9ca29-115">[应用程序](application.md)集合</span><span class="sxs-lookup"><span data-stu-id="9ca29-115">[application](application.md) collection</span></span>| <span data-ttu-id="9ca29-116">获取关联的应用程序对象集合。</span><span class="sxs-lookup"><span data-stu-id="9ca29-116">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="9ca29-117">创建连接器</span><span class="sxs-lookup"><span data-stu-id="9ca29-117">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="9ca29-118">连接器</span><span class="sxs-lookup"><span data-stu-id="9ca29-118">connector</span></span>](connector.md)| <span data-ttu-id="9ca29-119">通过发布到 members 集合, 将连接器添加到连接器组。</span><span class="sxs-lookup"><span data-stu-id="9ca29-119">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="9ca29-120">List members</span><span class="sxs-lookup"><span data-stu-id="9ca29-120">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="9ca29-121">[连接器](connector.md)集合</span><span class="sxs-lookup"><span data-stu-id="9ca29-121">[connector](connector.md) collection</span></span>| <span data-ttu-id="9ca29-122">获取连接器对象集合。</span><span class="sxs-lookup"><span data-stu-id="9ca29-122">Get a connector object collection.</span></span>|
|[<span data-ttu-id="9ca29-123">更新</span><span class="sxs-lookup"><span data-stu-id="9ca29-123">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="9ca29-124">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="9ca29-124">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="9ca29-125">更新 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="9ca29-125">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="9ca29-126">删除</span><span class="sxs-lookup"><span data-stu-id="9ca29-126">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="9ca29-127">无</span><span class="sxs-lookup"><span data-stu-id="9ca29-127">None</span></span> |<span data-ttu-id="9ca29-128">删除 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="9ca29-128">Delete connectorGroup object.</span></span> <span data-ttu-id="9ca29-129">必须删除所有连接器, 然后才能删除 conector 组。</span><span class="sxs-lookup"><span data-stu-id="9ca29-129">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="9ca29-130">属性</span><span class="sxs-lookup"><span data-stu-id="9ca29-130">Properties</span></span>
| <span data-ttu-id="9ca29-131">属性</span><span class="sxs-lookup"><span data-stu-id="9ca29-131">Property</span></span>     | <span data-ttu-id="9ca29-132">类型</span><span class="sxs-lookup"><span data-stu-id="9ca29-132">Type</span></span>   |<span data-ttu-id="9ca29-133">说明</span><span class="sxs-lookup"><span data-stu-id="9ca29-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ca29-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="9ca29-134">connectorGroupType</span></span>|<span data-ttu-id="9ca29-135">string</span><span class="sxs-lookup"><span data-stu-id="9ca29-135">string</span></span>| <span data-ttu-id="9ca29-136">将与组一起使用的连接器的类型。</span><span class="sxs-lookup"><span data-stu-id="9ca29-136">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="9ca29-137">可能的值是`applicationProxy`:。</span><span class="sxs-lookup"><span data-stu-id="9ca29-137">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="9ca29-138">id</span><span class="sxs-lookup"><span data-stu-id="9ca29-138">id</span></span>|<span data-ttu-id="9ca29-139">字符串</span><span class="sxs-lookup"><span data-stu-id="9ca29-139">String</span></span>| <span data-ttu-id="9ca29-140">connectorGroup 的对象 id</span><span class="sxs-lookup"><span data-stu-id="9ca29-140">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="9ca29-141">isDefault</span><span class="sxs-lookup"><span data-stu-id="9ca29-141">isDefault</span></span>|<span data-ttu-id="9ca29-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ca29-142">Boolean</span></span>| <span data-ttu-id="9ca29-143">指示 connectorGroup 是否为默认的连接器组。</span><span class="sxs-lookup"><span data-stu-id="9ca29-143">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="9ca29-144">只有一个连接器组可以是默认的 connectorGroup, 并由系统进行设置。</span><span class="sxs-lookup"><span data-stu-id="9ca29-144">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="9ca29-145">name</span><span class="sxs-lookup"><span data-stu-id="9ca29-145">name</span></span>|<span data-ttu-id="9ca29-146">String</span><span class="sxs-lookup"><span data-stu-id="9ca29-146">String</span></span>| <span data-ttu-id="9ca29-147">与 connectorGroup 关联的名称。</span><span class="sxs-lookup"><span data-stu-id="9ca29-147">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ca29-148">关系</span><span class="sxs-lookup"><span data-stu-id="9ca29-148">Relationships</span></span>
| <span data-ttu-id="9ca29-149">关系</span><span class="sxs-lookup"><span data-stu-id="9ca29-149">Relationship</span></span> | <span data-ttu-id="9ca29-150">类型</span><span class="sxs-lookup"><span data-stu-id="9ca29-150">Type</span></span>   |<span data-ttu-id="9ca29-151">说明</span><span class="sxs-lookup"><span data-stu-id="9ca29-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ca29-152">来说</span><span class="sxs-lookup"><span data-stu-id="9ca29-152">applications</span></span>|<span data-ttu-id="9ca29-153">[应用程序](application.md)集合</span><span class="sxs-lookup"><span data-stu-id="9ca29-153">[application](application.md) collection</span></span>| <span data-ttu-id="9ca29-154">只读。</span><span class="sxs-lookup"><span data-stu-id="9ca29-154">Read-only.</span></span> <span data-ttu-id="9ca29-155">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9ca29-155">Nullable.</span></span>|
|<span data-ttu-id="9ca29-156">members</span><span class="sxs-lookup"><span data-stu-id="9ca29-156">members</span></span>|<span data-ttu-id="9ca29-157">[连接器](connector.md)集合</span><span class="sxs-lookup"><span data-stu-id="9ca29-157">[connector](connector.md) collection</span></span>| <span data-ttu-id="9ca29-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="9ca29-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ca29-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ca29-160">JSON representation</span></span>

<span data-ttu-id="9ca29-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ca29-161">Here is a JSON representation of the resource.</span></span>

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
