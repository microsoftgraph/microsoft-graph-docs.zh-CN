---
title: externalConnection 资源类型
description: 连接是 Microsoft 服务中外部内容的逻辑Graph
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 76fa391d1ce9937bc1799e9bc4ae9470c0794497
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467640"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="2815c-103">externalConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="2815c-103">externalConnection resource type</span></span>

<span data-ttu-id="2815c-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="2815c-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2815c-105">一个逻辑容器，用于将外部源中的内容添加到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="2815c-105">A logical container to add content from an external source into Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="2815c-106">方法</span><span class="sxs-lookup"><span data-stu-id="2815c-106">Methods</span></span>

| <span data-ttu-id="2815c-107">方法</span><span class="sxs-lookup"><span data-stu-id="2815c-107">Method</span></span>                                                           | <span data-ttu-id="2815c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2815c-108">Return Type</span></span>                                   | <span data-ttu-id="2815c-109">说明</span><span class="sxs-lookup"><span data-stu-id="2815c-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="2815c-110">创建 externalConnection</span><span class="sxs-lookup"><span data-stu-id="2815c-110">Create externalConnection</span></span>](../api/externalconnectors-external-post-connections.md) | <span data-ttu-id="2815c-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="2815c-111">externalConnection</span></span>                            | <span data-ttu-id="2815c-112">通过发布到 connections 集合创建新的 externalConnection。</span><span class="sxs-lookup"><span data-stu-id="2815c-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="2815c-113">列出 externalConnections</span><span class="sxs-lookup"><span data-stu-id="2815c-113">List externalConnections</span></span>](../api/externalconnectors-externalconnection-list.md)    | <span data-ttu-id="2815c-114">externalConnection 集合</span><span class="sxs-lookup"><span data-stu-id="2815c-114">externalConnection collection</span></span>                 | <span data-ttu-id="2815c-115">获取 externalConnection 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2815c-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="2815c-116">获取 externalConnection</span><span class="sxs-lookup"><span data-stu-id="2815c-116">Get externalConnection</span></span>](../api/externalconnectors-externalconnection-get.md)       | <span data-ttu-id="2815c-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="2815c-117">externalConnection</span></span>                            | <span data-ttu-id="2815c-118">读取 externalConnection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2815c-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="2815c-119">更新 externalConnection</span><span class="sxs-lookup"><span data-stu-id="2815c-119">Update externalConnection</span></span>](../api/externalconnectors-externalconnection-update.md) | <span data-ttu-id="2815c-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="2815c-120">externalConnection</span></span>                            | <span data-ttu-id="2815c-121">更新 externalConnection 对象。</span><span class="sxs-lookup"><span data-stu-id="2815c-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="2815c-122">删除 externalConnection</span><span class="sxs-lookup"><span data-stu-id="2815c-122">Delete externalConnection</span></span>](../api/externalconnectors-externalconnection-delete.md) | <span data-ttu-id="2815c-123">无</span><span class="sxs-lookup"><span data-stu-id="2815c-123">None</span></span>                                          | <span data-ttu-id="2815c-124">删除 externalConnection 对象。</span><span class="sxs-lookup"><span data-stu-id="2815c-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="2815c-125">创建架构</span><span class="sxs-lookup"><span data-stu-id="2815c-125">Create schema</span></span>](../api/externalconnectors-externalconnection-post-schema.md)        | <span data-ttu-id="2815c-126">无 *或*[架构](externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="2815c-126">None *or* [schema](externalconnectors-schema.md)</span></span>                 | <span data-ttu-id="2815c-127">注册连接架构。</span><span class="sxs-lookup"><span data-stu-id="2815c-127">Register connection schema.</span></span> |
| [<span data-ttu-id="2815c-128">获取操作</span><span class="sxs-lookup"><span data-stu-id="2815c-128">Get operation</span></span>](../api/externalconnectors-connectionoperation-get.md)               | [<span data-ttu-id="2815c-129">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="2815c-129">connectionOperation</span></span>](externalconnectors-connectionoperation.md) | <span data-ttu-id="2815c-130">获取用于创建连接架构的异步请求的状态。</span><span class="sxs-lookup"><span data-stu-id="2815c-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="2815c-131">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="2815c-131">Create externalItem</span></span>](../api/externalconnectors-externalconnection-put-items.md)    | [<span data-ttu-id="2815c-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="2815c-132">externalItem</span></span>](externalconnectors-externalitem.md)               | <span data-ttu-id="2815c-133">通过发布到项目集合创建新的 externalItem。</span><span class="sxs-lookup"><span data-stu-id="2815c-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="2815c-134">属性</span><span class="sxs-lookup"><span data-stu-id="2815c-134">Properties</span></span>

| <span data-ttu-id="2815c-135">属性</span><span class="sxs-lookup"><span data-stu-id="2815c-135">Property</span></span>      | <span data-ttu-id="2815c-136">类型</span><span class="sxs-lookup"><span data-stu-id="2815c-136">Type</span></span>                              | <span data-ttu-id="2815c-137">说明</span><span class="sxs-lookup"><span data-stu-id="2815c-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="2815c-138">configuration</span><span class="sxs-lookup"><span data-stu-id="2815c-138">configuration</span></span> | [<span data-ttu-id="2815c-139">microsoft.graph.externalConnectors.configuration</span><span class="sxs-lookup"><span data-stu-id="2815c-139">microsoft.graph.externalConnectors.configuration</span></span>](externalconnectors-configuration.md) | <span data-ttu-id="2815c-140">指定允许管理连接和索引连接内容的其他应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="2815c-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="2815c-141">可选。</span><span class="sxs-lookup"><span data-stu-id="2815c-141">Optional.</span></span> |
| <span data-ttu-id="2815c-142">说明</span><span class="sxs-lookup"><span data-stu-id="2815c-142">description</span></span>   | <span data-ttu-id="2815c-143">String</span><span class="sxs-lookup"><span data-stu-id="2815c-143">String</span></span>                            | <span data-ttu-id="2815c-144">网站中显示的连接Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="2815c-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="2815c-145">可选。</span><span class="sxs-lookup"><span data-stu-id="2815c-145">Optional.</span></span> |
| <span data-ttu-id="2815c-146">id</span><span class="sxs-lookup"><span data-stu-id="2815c-146">id</span></span>            | <span data-ttu-id="2815c-147">String</span><span class="sxs-lookup"><span data-stu-id="2815c-147">String</span></span>                            | <span data-ttu-id="2815c-148">开发人员为租户内的连接提供的唯Azure Active Directory ID。</span><span class="sxs-lookup"><span data-stu-id="2815c-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="2815c-149">长度必须在 3 到 32 个字符之间。</span><span class="sxs-lookup"><span data-stu-id="2815c-149">Must be between 3 and 32 characters in length.</span></span> <span data-ttu-id="2815c-150">只能包含字母数字字符。</span><span class="sxs-lookup"><span data-stu-id="2815c-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="2815c-151">不能以 `Microsoft` 或 作为下列值之一： `None` 、 、 `Directory` `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` `TaskFabric` `PowerBI` `Assistant` `TopicEngine` `MSFT_All_Connectors` 。</span><span class="sxs-lookup"><span data-stu-id="2815c-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`, `TaskFabric`, `PowerBI`, `Assistant`, `TopicEngine`, `MSFT_All_Connectors`.</span></span> <span data-ttu-id="2815c-152">必需项。</span><span class="sxs-lookup"><span data-stu-id="2815c-152">Required.</span></span> |
| <span data-ttu-id="2815c-153">name</span><span class="sxs-lookup"><span data-stu-id="2815c-153">name</span></span>          | <span data-ttu-id="2815c-154">String</span><span class="sxs-lookup"><span data-stu-id="2815c-154">String</span></span>                            | <span data-ttu-id="2815c-155">要显示名称中显示的连接的Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="2815c-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="2815c-156">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="2815c-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="2815c-157">必需项。</span><span class="sxs-lookup"><span data-stu-id="2815c-157">Required.</span></span> |
| <span data-ttu-id="2815c-158">state</span><span class="sxs-lookup"><span data-stu-id="2815c-158">state</span></span>         | <span data-ttu-id="2815c-159">microsoft.graph.externalConnectors.connectionState</span><span class="sxs-lookup"><span data-stu-id="2815c-159">microsoft.graph.externalConnectors.connectionState</span></span>                   | <span data-ttu-id="2815c-160">指示连接的当前状态。</span><span class="sxs-lookup"><span data-stu-id="2815c-160">Indicates the current state of the connection.</span></span> <span data-ttu-id="2815c-161">可能的值为 `draft` `ready` 、、 `obsolete` 和 `limitExceeded` 。</span><span class="sxs-lookup"><span data-stu-id="2815c-161">Possible values are `draft`, `ready`, `obsolete`, and `limitExceeded`.</span></span> <span data-ttu-id="2815c-162">必填。</span><span class="sxs-lookup"><span data-stu-id="2815c-162">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2815c-163">关系</span><span class="sxs-lookup"><span data-stu-id="2815c-163">Relationships</span></span>

| <span data-ttu-id="2815c-164">关系</span><span class="sxs-lookup"><span data-stu-id="2815c-164">Relationship</span></span> | <span data-ttu-id="2815c-165">类型</span><span class="sxs-lookup"><span data-stu-id="2815c-165">Type</span></span>                                                     | <span data-ttu-id="2815c-166">说明</span><span class="sxs-lookup"><span data-stu-id="2815c-166">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="2815c-167">items</span><span class="sxs-lookup"><span data-stu-id="2815c-167">items</span></span>        | <span data-ttu-id="2815c-168">[microsoft.graph.externalConnectors.externalItem](externalconnectors-externalitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2815c-168">[microsoft.graph.externalConnectors.externalItem](externalconnectors-externalitem.md) collection</span></span>               | <span data-ttu-id="2815c-p106">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="2815c-p106">Read-only. Nullable.</span></span> |
| <span data-ttu-id="2815c-171">operations</span><span class="sxs-lookup"><span data-stu-id="2815c-171">operations</span></span>   | <span data-ttu-id="2815c-172">[microsoft.graph.externalConnectors.connectionOperation](externalconnectors-connectionoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2815c-172">[microsoft.graph.externalConnectors.connectionOperation](externalconnectors-connectionoperation.md) collection</span></span> | <span data-ttu-id="2815c-p107">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="2815c-p107">Read-only. Nullable.</span></span> |
| <span data-ttu-id="2815c-175">schema</span><span class="sxs-lookup"><span data-stu-id="2815c-175">schema</span></span>       | [<span data-ttu-id="2815c-176">microsoft.graph.externalConnectors.schema</span><span class="sxs-lookup"><span data-stu-id="2815c-176">microsoft.graph.externalConnectors.schema</span></span>](externalconnectors-schema.md)                                      | <span data-ttu-id="2815c-p108">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="2815c-p108">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2815c-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2815c-179">JSON representation</span></span>

<span data-ttu-id="2815c-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2815c-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "name": "String",
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
