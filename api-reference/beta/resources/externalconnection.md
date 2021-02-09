---
title: externalConnection 资源类型
description: 连接是 Microsoft Graph 中外部内容的逻辑容器
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4355ffe51fe1b160c7fb486272e85f2b2cf0bf2c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161699"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="72df9-103">externalConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="72df9-103">externalConnection resource type</span></span>

<span data-ttu-id="72df9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72df9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72df9-105">将外部源中的内容添加到 Microsoft Graph 的逻辑容器。</span><span class="sxs-lookup"><span data-stu-id="72df9-105">A logical container to add content from an external source into Microsoft Graph.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="72df9-106">方法</span><span class="sxs-lookup"><span data-stu-id="72df9-106">Methods</span></span>

| <span data-ttu-id="72df9-107">方法</span><span class="sxs-lookup"><span data-stu-id="72df9-107">Method</span></span>                                                           | <span data-ttu-id="72df9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="72df9-108">Return Type</span></span>                                   | <span data-ttu-id="72df9-109">说明</span><span class="sxs-lookup"><span data-stu-id="72df9-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="72df9-110">创建 externalConnection</span><span class="sxs-lookup"><span data-stu-id="72df9-110">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="72df9-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="72df9-111">externalConnection</span></span>                            | <span data-ttu-id="72df9-112">通过发布到 connections 集合创建新的 externalConnection。</span><span class="sxs-lookup"><span data-stu-id="72df9-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="72df9-113">列出 externalConnections</span><span class="sxs-lookup"><span data-stu-id="72df9-113">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="72df9-114">externalConnection 集合</span><span class="sxs-lookup"><span data-stu-id="72df9-114">externalConnection collection</span></span>                 | <span data-ttu-id="72df9-115">获取 externalConnection 对象集合。</span><span class="sxs-lookup"><span data-stu-id="72df9-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="72df9-116">获取 externalConnection</span><span class="sxs-lookup"><span data-stu-id="72df9-116">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="72df9-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="72df9-117">externalConnection</span></span>                            | <span data-ttu-id="72df9-118">读取 externalConnection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="72df9-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="72df9-119">更新 externalConnection</span><span class="sxs-lookup"><span data-stu-id="72df9-119">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="72df9-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="72df9-120">externalConnection</span></span>                            | <span data-ttu-id="72df9-121">更新 externalConnection 对象。</span><span class="sxs-lookup"><span data-stu-id="72df9-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="72df9-122">删除 externalConnection</span><span class="sxs-lookup"><span data-stu-id="72df9-122">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="72df9-123">无</span><span class="sxs-lookup"><span data-stu-id="72df9-123">None</span></span>                                          | <span data-ttu-id="72df9-124">删除 externalConnection 对象。</span><span class="sxs-lookup"><span data-stu-id="72df9-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="72df9-125">创建架构</span><span class="sxs-lookup"><span data-stu-id="72df9-125">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="72df9-126">无 *或*[架构](schema.md)</span><span class="sxs-lookup"><span data-stu-id="72df9-126">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="72df9-127">注册连接架构。</span><span class="sxs-lookup"><span data-stu-id="72df9-127">Register connection schema.</span></span> |
| [<span data-ttu-id="72df9-128">获取操作</span><span class="sxs-lookup"><span data-stu-id="72df9-128">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="72df9-129">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="72df9-129">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="72df9-130">获取异步请求的状态以创建连接架构。</span><span class="sxs-lookup"><span data-stu-id="72df9-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="72df9-131">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="72df9-131">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="72df9-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="72df9-132">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="72df9-133">通过发布到项目集合创建新的 externalItem。</span><span class="sxs-lookup"><span data-stu-id="72df9-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="72df9-134">属性</span><span class="sxs-lookup"><span data-stu-id="72df9-134">Properties</span></span>

| <span data-ttu-id="72df9-135">属性</span><span class="sxs-lookup"><span data-stu-id="72df9-135">Property</span></span>      | <span data-ttu-id="72df9-136">类型</span><span class="sxs-lookup"><span data-stu-id="72df9-136">Type</span></span>                              | <span data-ttu-id="72df9-137">说明</span><span class="sxs-lookup"><span data-stu-id="72df9-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="72df9-138">configuration</span><span class="sxs-lookup"><span data-stu-id="72df9-138">configuration</span></span> | [<span data-ttu-id="72df9-139">configuration</span><span class="sxs-lookup"><span data-stu-id="72df9-139">configuration</span></span>](configuration.md) | <span data-ttu-id="72df9-140">指定允许管理连接和索引连接内容的其他应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="72df9-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="72df9-141">可选。</span><span class="sxs-lookup"><span data-stu-id="72df9-141">Optional.</span></span> |
| <span data-ttu-id="72df9-142">说明</span><span class="sxs-lookup"><span data-stu-id="72df9-142">description</span></span>   | <span data-ttu-id="72df9-143">String</span><span class="sxs-lookup"><span data-stu-id="72df9-143">String</span></span>                            | <span data-ttu-id="72df9-144">Microsoft 365 管理中心中显示的连接说明。</span><span class="sxs-lookup"><span data-stu-id="72df9-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="72df9-145">可选。</span><span class="sxs-lookup"><span data-stu-id="72df9-145">Optional.</span></span> |
| <span data-ttu-id="72df9-146">id</span><span class="sxs-lookup"><span data-stu-id="72df9-146">id</span></span>            | <span data-ttu-id="72df9-147">String</span><span class="sxs-lookup"><span data-stu-id="72df9-147">String</span></span>                            | <span data-ttu-id="72df9-148">开发人员提供的 Azure Active Directory 租户内连接的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="72df9-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="72df9-149">最大长度为 32 个字符。</span><span class="sxs-lookup"><span data-stu-id="72df9-149">Maximum length of 32 characters.</span></span> <span data-ttu-id="72df9-150">必须仅包含字母数字字符。</span><span class="sxs-lookup"><span data-stu-id="72df9-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="72df9-151">不能以下列值开头或为下列值之一 `Microsoft` ： ， ， ， ， `None` `Directory` `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` 。 `Connectors`</span><span class="sxs-lookup"><span data-stu-id="72df9-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="72df9-152">必需。</span><span class="sxs-lookup"><span data-stu-id="72df9-152">Required.</span></span> |
| <span data-ttu-id="72df9-153">名称</span><span class="sxs-lookup"><span data-stu-id="72df9-153">name</span></span>          | <span data-ttu-id="72df9-154">String</span><span class="sxs-lookup"><span data-stu-id="72df9-154">String</span></span>                            | <span data-ttu-id="72df9-155">要显示名称 Microsoft 365 管理中心中显示的连接的列表。</span><span class="sxs-lookup"><span data-stu-id="72df9-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="72df9-156">最大长度为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="72df9-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="72df9-157">必需。</span><span class="sxs-lookup"><span data-stu-id="72df9-157">Required.</span></span> |
| <span data-ttu-id="72df9-158">state</span><span class="sxs-lookup"><span data-stu-id="72df9-158">state</span></span>         | <span data-ttu-id="72df9-159">connectionState</span><span class="sxs-lookup"><span data-stu-id="72df9-159">connectionState</span></span>                   | <span data-ttu-id="72df9-160">指示连接的当前状态。</span><span class="sxs-lookup"><span data-stu-id="72df9-160">Indicates the current state of the connection.</span></span> <span data-ttu-id="72df9-161">可能的值是 `draft` ， `ready` 和 `obsolete` `limitExceeded` 。</span><span class="sxs-lookup"><span data-stu-id="72df9-161">Possible values are `draft`, `ready`, `obsolete`, and `limitExceeded`.</span></span> <span data-ttu-id="72df9-162">必填。</span><span class="sxs-lookup"><span data-stu-id="72df9-162">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="72df9-163">关系</span><span class="sxs-lookup"><span data-stu-id="72df9-163">Relationships</span></span>

| <span data-ttu-id="72df9-164">关系</span><span class="sxs-lookup"><span data-stu-id="72df9-164">Relationship</span></span> | <span data-ttu-id="72df9-165">类型</span><span class="sxs-lookup"><span data-stu-id="72df9-165">Type</span></span>                                                     | <span data-ttu-id="72df9-166">说明</span><span class="sxs-lookup"><span data-stu-id="72df9-166">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="72df9-167">items</span><span class="sxs-lookup"><span data-stu-id="72df9-167">items</span></span>        | <span data-ttu-id="72df9-168">[externalItem](externalitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72df9-168">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="72df9-p106">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="72df9-p106">Read-only. Nullable.</span></span> |
| <span data-ttu-id="72df9-171">operations</span><span class="sxs-lookup"><span data-stu-id="72df9-171">operations</span></span>   | <span data-ttu-id="72df9-172">[connectionOperation](connectionoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72df9-172">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="72df9-173">只读。</span><span class="sxs-lookup"><span data-stu-id="72df9-173">Read-only.</span></span> <span data-ttu-id="72df9-174">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="72df9-174">Nullable.</span></span> |
| <span data-ttu-id="72df9-175">架构</span><span class="sxs-lookup"><span data-stu-id="72df9-175">schema</span></span>       | [<span data-ttu-id="72df9-176">schema</span><span class="sxs-lookup"><span data-stu-id="72df9-176">schema</span></span>](schema.md)                                      | <span data-ttu-id="72df9-p108">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="72df9-p108">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="72df9-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72df9-179">JSON representation</span></span>

<span data-ttu-id="72df9-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72df9-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnection",
  "keyProperty": "id"
}-->

```json
{
  "configuration": {"@odata.type": "microsoft.graph.configuration"},
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
