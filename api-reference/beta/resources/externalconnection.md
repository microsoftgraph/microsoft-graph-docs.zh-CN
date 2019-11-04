---
title: externalConnection 资源类型
description: 从外部源到 Microsoft 搜索的连接。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3e56b40a4ce91fa1b70aa01060c7ad5272fc1087
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939058"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="67656-103">externalConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="67656-103">externalConnection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67656-104">从外部源到 Microsoft 搜索的连接。</span><span class="sxs-lookup"><span data-stu-id="67656-104">A connection to Microsoft Search from an external source.</span></span>

## <a name="methods"></a><span data-ttu-id="67656-105">方法</span><span class="sxs-lookup"><span data-stu-id="67656-105">Methods</span></span>

| <span data-ttu-id="67656-106">方法</span><span class="sxs-lookup"><span data-stu-id="67656-106">Method</span></span>                                                           | <span data-ttu-id="67656-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="67656-107">Return Type</span></span>                                   | <span data-ttu-id="67656-108">说明</span><span class="sxs-lookup"><span data-stu-id="67656-108">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="67656-109">创建 externalConnection</span><span class="sxs-lookup"><span data-stu-id="67656-109">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="67656-110">externalConnection</span><span class="sxs-lookup"><span data-stu-id="67656-110">externalConnection</span></span>                            | <span data-ttu-id="67656-111">通过发布到 connections 集合创建新的 externalConnection。</span><span class="sxs-lookup"><span data-stu-id="67656-111">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="67656-112">列出 externalConnections</span><span class="sxs-lookup"><span data-stu-id="67656-112">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="67656-113">externalConnection 集合</span><span class="sxs-lookup"><span data-stu-id="67656-113">externalConnection collection</span></span>                 | <span data-ttu-id="67656-114">获取 externalConnection 对象集合。</span><span class="sxs-lookup"><span data-stu-id="67656-114">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="67656-115">获取 externalConnection</span><span class="sxs-lookup"><span data-stu-id="67656-115">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="67656-116">externalConnection</span><span class="sxs-lookup"><span data-stu-id="67656-116">externalConnection</span></span>                            | <span data-ttu-id="67656-117">读取 externalConnection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="67656-117">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="67656-118">更新 externalConnection</span><span class="sxs-lookup"><span data-stu-id="67656-118">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="67656-119">externalConnection</span><span class="sxs-lookup"><span data-stu-id="67656-119">externalConnection</span></span>                            | <span data-ttu-id="67656-120">更新 externalConnection 对象。</span><span class="sxs-lookup"><span data-stu-id="67656-120">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="67656-121">删除 externalConnection</span><span class="sxs-lookup"><span data-stu-id="67656-121">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="67656-122">无</span><span class="sxs-lookup"><span data-stu-id="67656-122">None</span></span>                                          | <span data-ttu-id="67656-123">删除 externalConnection 对象。</span><span class="sxs-lookup"><span data-stu-id="67656-123">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="67656-124">创建架构</span><span class="sxs-lookup"><span data-stu-id="67656-124">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="67656-125">无*或*[架构](schema.md)</span><span class="sxs-lookup"><span data-stu-id="67656-125">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="67656-126">注册连接架构。</span><span class="sxs-lookup"><span data-stu-id="67656-126">Register connection schema.</span></span> |
| [<span data-ttu-id="67656-127">Get 操作</span><span class="sxs-lookup"><span data-stu-id="67656-127">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="67656-128">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="67656-128">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="67656-129">获取用于创建连接架构的异步请求的状态。</span><span class="sxs-lookup"><span data-stu-id="67656-129">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="67656-130">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="67656-130">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="67656-131">externalItem</span><span class="sxs-lookup"><span data-stu-id="67656-131">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="67656-132">通过发布到 items 集合创建新的 externalItem。</span><span class="sxs-lookup"><span data-stu-id="67656-132">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="67656-133">属性</span><span class="sxs-lookup"><span data-stu-id="67656-133">Properties</span></span>

| <span data-ttu-id="67656-134">属性</span><span class="sxs-lookup"><span data-stu-id="67656-134">Property</span></span>      | <span data-ttu-id="67656-135">类型</span><span class="sxs-lookup"><span data-stu-id="67656-135">Type</span></span>                              | <span data-ttu-id="67656-136">描述</span><span class="sxs-lookup"><span data-stu-id="67656-136">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="67656-137">设置</span><span class="sxs-lookup"><span data-stu-id="67656-137">configuration</span></span> | [<span data-ttu-id="67656-138">configuration</span><span class="sxs-lookup"><span data-stu-id="67656-138">configuration</span></span>](configuration.md) | <span data-ttu-id="67656-139">指定允许管理连接和索引连接中的内容的其他应用程序 Id。</span><span class="sxs-lookup"><span data-stu-id="67656-139">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="67656-140">可选。</span><span class="sxs-lookup"><span data-stu-id="67656-140">Optional.</span></span> |
| <span data-ttu-id="67656-141">description</span><span class="sxs-lookup"><span data-stu-id="67656-141">description</span></span>   | <span data-ttu-id="67656-142">String</span><span class="sxs-lookup"><span data-stu-id="67656-142">String</span></span>                            | <span data-ttu-id="67656-143">Microsoft 365 管理中心显示的连接的说明。</span><span class="sxs-lookup"><span data-stu-id="67656-143">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="67656-144">可选。</span><span class="sxs-lookup"><span data-stu-id="67656-144">Optional.</span></span> |
| <span data-ttu-id="67656-145">id</span><span class="sxs-lookup"><span data-stu-id="67656-145">id</span></span>            | <span data-ttu-id="67656-146">String</span><span class="sxs-lookup"><span data-stu-id="67656-146">String</span></span>                            | <span data-ttu-id="67656-147">在 Azure Active Directory 租户中，开发人员提供的连接的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="67656-147">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="67656-148">最大长度为32个字符。</span><span class="sxs-lookup"><span data-stu-id="67656-148">Maximum length of 32 characters.</span></span> <span data-ttu-id="67656-149">必须仅包含字母数字字符。</span><span class="sxs-lookup"><span data-stu-id="67656-149">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="67656-150">不能以`Microsoft`下列值开头，也不能为`None`下列`Directory`值`Exchange`之一`ExchangeArchive`： `LinkedIn`、 `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer`、、、、、、 `Connectors`、、、。</span><span class="sxs-lookup"><span data-stu-id="67656-150">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="67656-151">必填。</span><span class="sxs-lookup"><span data-stu-id="67656-151">Required.</span></span> |
| <span data-ttu-id="67656-152">name</span><span class="sxs-lookup"><span data-stu-id="67656-152">name</span></span>          | <span data-ttu-id="67656-153">字符串</span><span class="sxs-lookup"><span data-stu-id="67656-153">String</span></span>                            | <span data-ttu-id="67656-154">要显示在 Microsoft 365 管理中心中的连接的显示名称。</span><span class="sxs-lookup"><span data-stu-id="67656-154">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="67656-155">最大长度为128个字符。</span><span class="sxs-lookup"><span data-stu-id="67656-155">Maximum length of 128 characters.</span></span> <span data-ttu-id="67656-156">必填。</span><span class="sxs-lookup"><span data-stu-id="67656-156">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="67656-157">关系</span><span class="sxs-lookup"><span data-stu-id="67656-157">Relationships</span></span>

| <span data-ttu-id="67656-158">关系</span><span class="sxs-lookup"><span data-stu-id="67656-158">Relationship</span></span> | <span data-ttu-id="67656-159">类型</span><span class="sxs-lookup"><span data-stu-id="67656-159">Type</span></span>                                                     | <span data-ttu-id="67656-160">描述</span><span class="sxs-lookup"><span data-stu-id="67656-160">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="67656-161">items</span><span class="sxs-lookup"><span data-stu-id="67656-161">items</span></span>        | <span data-ttu-id="67656-162">[externalItem](externalitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="67656-162">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="67656-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="67656-p105">Read-only. Nullable.</span></span> |
| <span data-ttu-id="67656-165">operations</span><span class="sxs-lookup"><span data-stu-id="67656-165">operations</span></span>   | <span data-ttu-id="67656-166">[connectionOperation](connectionoperation.md)集合</span><span class="sxs-lookup"><span data-stu-id="67656-166">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="67656-167">只读。</span><span class="sxs-lookup"><span data-stu-id="67656-167">Read-only.</span></span> <span data-ttu-id="67656-168">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="67656-168">Nullable.</span></span> |
| <span data-ttu-id="67656-169">架构</span><span class="sxs-lookup"><span data-stu-id="67656-169">schema</span></span>       | [<span data-ttu-id="67656-170">架构</span><span class="sxs-lookup"><span data-stu-id="67656-170">schema</span></span>](schema.md)                                      | <span data-ttu-id="67656-p107">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="67656-p107">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="67656-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67656-173">JSON representation</span></span>

<span data-ttu-id="67656-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67656-174">The following is a JSON representation of the resource.</span></span>

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
