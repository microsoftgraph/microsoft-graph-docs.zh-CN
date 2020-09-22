---
title: externalConnection 资源类型
description: 从外部源到 Microsoft 搜索的连接。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a5db824fabc1cedb27d15c4b2cbfbce08bd59191
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026927"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="dd28c-103">externalConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd28c-103">externalConnection resource type</span></span>

<span data-ttu-id="dd28c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd28c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd28c-105">从外部源到 Microsoft 搜索的连接。</span><span class="sxs-lookup"><span data-stu-id="dd28c-105">A connection to Microsoft Search from an external source.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="dd28c-106">方法</span><span class="sxs-lookup"><span data-stu-id="dd28c-106">Methods</span></span>

| <span data-ttu-id="dd28c-107">方法</span><span class="sxs-lookup"><span data-stu-id="dd28c-107">Method</span></span>                                                           | <span data-ttu-id="dd28c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="dd28c-108">Return Type</span></span>                                   | <span data-ttu-id="dd28c-109">说明</span><span class="sxs-lookup"><span data-stu-id="dd28c-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="dd28c-110">创建 externalConnection</span><span class="sxs-lookup"><span data-stu-id="dd28c-110">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="dd28c-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="dd28c-111">externalConnection</span></span>                            | <span data-ttu-id="dd28c-112">通过发布到 connections 集合创建新的 externalConnection。</span><span class="sxs-lookup"><span data-stu-id="dd28c-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="dd28c-113">列出 externalConnections</span><span class="sxs-lookup"><span data-stu-id="dd28c-113">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="dd28c-114">externalConnection 集合</span><span class="sxs-lookup"><span data-stu-id="dd28c-114">externalConnection collection</span></span>                 | <span data-ttu-id="dd28c-115">获取 externalConnection 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dd28c-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="dd28c-116">获取 externalConnection</span><span class="sxs-lookup"><span data-stu-id="dd28c-116">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="dd28c-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="dd28c-117">externalConnection</span></span>                            | <span data-ttu-id="dd28c-118">读取 externalConnection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dd28c-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="dd28c-119">更新 externalConnection</span><span class="sxs-lookup"><span data-stu-id="dd28c-119">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="dd28c-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="dd28c-120">externalConnection</span></span>                            | <span data-ttu-id="dd28c-121">更新 externalConnection 对象。</span><span class="sxs-lookup"><span data-stu-id="dd28c-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="dd28c-122">删除 externalConnection</span><span class="sxs-lookup"><span data-stu-id="dd28c-122">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="dd28c-123">无</span><span class="sxs-lookup"><span data-stu-id="dd28c-123">None</span></span>                                          | <span data-ttu-id="dd28c-124">删除 externalConnection 对象。</span><span class="sxs-lookup"><span data-stu-id="dd28c-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="dd28c-125">创建架构</span><span class="sxs-lookup"><span data-stu-id="dd28c-125">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="dd28c-126">无*或*[架构](schema.md)</span><span class="sxs-lookup"><span data-stu-id="dd28c-126">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="dd28c-127">注册连接架构。</span><span class="sxs-lookup"><span data-stu-id="dd28c-127">Register connection schema.</span></span> |
| [<span data-ttu-id="dd28c-128">Get 操作</span><span class="sxs-lookup"><span data-stu-id="dd28c-128">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="dd28c-129">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="dd28c-129">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="dd28c-130">获取用于创建连接架构的异步请求的状态。</span><span class="sxs-lookup"><span data-stu-id="dd28c-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="dd28c-131">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="dd28c-131">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="dd28c-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="dd28c-132">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="dd28c-133">通过发布到 items 集合创建新的 externalItem。</span><span class="sxs-lookup"><span data-stu-id="dd28c-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="dd28c-134">属性</span><span class="sxs-lookup"><span data-stu-id="dd28c-134">Properties</span></span>

| <span data-ttu-id="dd28c-135">属性</span><span class="sxs-lookup"><span data-stu-id="dd28c-135">Property</span></span>      | <span data-ttu-id="dd28c-136">类型</span><span class="sxs-lookup"><span data-stu-id="dd28c-136">Type</span></span>                              | <span data-ttu-id="dd28c-137">说明</span><span class="sxs-lookup"><span data-stu-id="dd28c-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="dd28c-138">configuration</span><span class="sxs-lookup"><span data-stu-id="dd28c-138">configuration</span></span> | [<span data-ttu-id="dd28c-139">configuration</span><span class="sxs-lookup"><span data-stu-id="dd28c-139">configuration</span></span>](configuration.md) | <span data-ttu-id="dd28c-140">指定允许管理连接和索引连接中的内容的其他应用程序 Id。</span><span class="sxs-lookup"><span data-stu-id="dd28c-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="dd28c-141">可选。</span><span class="sxs-lookup"><span data-stu-id="dd28c-141">Optional.</span></span> |
| <span data-ttu-id="dd28c-142">description</span><span class="sxs-lookup"><span data-stu-id="dd28c-142">description</span></span>   | <span data-ttu-id="dd28c-143">String</span><span class="sxs-lookup"><span data-stu-id="dd28c-143">String</span></span>                            | <span data-ttu-id="dd28c-144">Microsoft 365 管理中心显示的连接的说明。</span><span class="sxs-lookup"><span data-stu-id="dd28c-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="dd28c-145">可选。</span><span class="sxs-lookup"><span data-stu-id="dd28c-145">Optional.</span></span> |
| <span data-ttu-id="dd28c-146">id</span><span class="sxs-lookup"><span data-stu-id="dd28c-146">id</span></span>            | <span data-ttu-id="dd28c-147">String</span><span class="sxs-lookup"><span data-stu-id="dd28c-147">String</span></span>                            | <span data-ttu-id="dd28c-148">在 Azure Active Directory 租户中，开发人员提供的连接的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="dd28c-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="dd28c-149">最大长度为32个字符。</span><span class="sxs-lookup"><span data-stu-id="dd28c-149">Maximum length of 32 characters.</span></span> <span data-ttu-id="dd28c-150">必须仅包含字母数字字符。</span><span class="sxs-lookup"><span data-stu-id="dd28c-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="dd28c-151">不能以 `Microsoft` 下列值开头，也不能为下列值之一：、、、、、、、、、、 `None` `Directory` `Exchange` `ExchangeArchive` `LinkedIn` `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer` `Connectors` 。</span><span class="sxs-lookup"><span data-stu-id="dd28c-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="dd28c-152">必需。</span><span class="sxs-lookup"><span data-stu-id="dd28c-152">Required.</span></span> |
| <span data-ttu-id="dd28c-153">name</span><span class="sxs-lookup"><span data-stu-id="dd28c-153">name</span></span>          | <span data-ttu-id="dd28c-154">String</span><span class="sxs-lookup"><span data-stu-id="dd28c-154">String</span></span>                            | <span data-ttu-id="dd28c-155">要显示在 Microsoft 365 管理中心中的连接的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dd28c-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="dd28c-156">最大长度为128个字符。</span><span class="sxs-lookup"><span data-stu-id="dd28c-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="dd28c-157">必需。</span><span class="sxs-lookup"><span data-stu-id="dd28c-157">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dd28c-158">关系</span><span class="sxs-lookup"><span data-stu-id="dd28c-158">Relationships</span></span>

| <span data-ttu-id="dd28c-159">关系</span><span class="sxs-lookup"><span data-stu-id="dd28c-159">Relationship</span></span> | <span data-ttu-id="dd28c-160">类型</span><span class="sxs-lookup"><span data-stu-id="dd28c-160">Type</span></span>                                                     | <span data-ttu-id="dd28c-161">说明</span><span class="sxs-lookup"><span data-stu-id="dd28c-161">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="dd28c-162">items</span><span class="sxs-lookup"><span data-stu-id="dd28c-162">items</span></span>        | <span data-ttu-id="dd28c-163">[externalItem](externalitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dd28c-163">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="dd28c-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="dd28c-p105">Read-only. Nullable.</span></span> |
| <span data-ttu-id="dd28c-166">operations</span><span class="sxs-lookup"><span data-stu-id="dd28c-166">operations</span></span>   | <span data-ttu-id="dd28c-167">[connectionOperation](connectionoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dd28c-167">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="dd28c-168">只读。</span><span class="sxs-lookup"><span data-stu-id="dd28c-168">Read-only.</span></span> <span data-ttu-id="dd28c-169">可为空。</span><span class="sxs-lookup"><span data-stu-id="dd28c-169">Nullable.</span></span> |
| <span data-ttu-id="dd28c-170">架构</span><span class="sxs-lookup"><span data-stu-id="dd28c-170">schema</span></span>       | [<span data-ttu-id="dd28c-171">schema</span><span class="sxs-lookup"><span data-stu-id="dd28c-171">schema</span></span>](schema.md)                                      | <span data-ttu-id="dd28c-p107">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="dd28c-p107">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dd28c-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd28c-174">JSON representation</span></span>

<span data-ttu-id="dd28c-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd28c-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnection",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "configuration": {"@odata.type": "microsoft.graph.configuration"},
  "description": "String",
  "id": "String (identifier)",
  "name": "String"
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


