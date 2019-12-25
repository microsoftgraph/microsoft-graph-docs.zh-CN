---
title: externalConnection 资源类型
description: 从外部源到 Microsoft 搜索的连接。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4a77afc0aeef6c68d7bd58e554848068f25e1142
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866838"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="98abc-103">externalConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="98abc-103">externalConnection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98abc-104">从外部源到 Microsoft 搜索的连接。</span><span class="sxs-lookup"><span data-stu-id="98abc-104">A connection to Microsoft Search from an external source.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="98abc-105">方法</span><span class="sxs-lookup"><span data-stu-id="98abc-105">Methods</span></span>

| <span data-ttu-id="98abc-106">方法</span><span class="sxs-lookup"><span data-stu-id="98abc-106">Method</span></span>                                                           | <span data-ttu-id="98abc-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="98abc-107">Return Type</span></span>                                   | <span data-ttu-id="98abc-108">说明</span><span class="sxs-lookup"><span data-stu-id="98abc-108">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="98abc-109">创建 externalConnection</span><span class="sxs-lookup"><span data-stu-id="98abc-109">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="98abc-110">externalConnection</span><span class="sxs-lookup"><span data-stu-id="98abc-110">externalConnection</span></span>                            | <span data-ttu-id="98abc-111">通过发布到 connections 集合创建新的 externalConnection。</span><span class="sxs-lookup"><span data-stu-id="98abc-111">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="98abc-112">列出 externalConnections</span><span class="sxs-lookup"><span data-stu-id="98abc-112">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="98abc-113">externalConnection 集合</span><span class="sxs-lookup"><span data-stu-id="98abc-113">externalConnection collection</span></span>                 | <span data-ttu-id="98abc-114">获取 externalConnection 对象集合。</span><span class="sxs-lookup"><span data-stu-id="98abc-114">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="98abc-115">获取 externalConnection</span><span class="sxs-lookup"><span data-stu-id="98abc-115">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="98abc-116">externalConnection</span><span class="sxs-lookup"><span data-stu-id="98abc-116">externalConnection</span></span>                            | <span data-ttu-id="98abc-117">读取 externalConnection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="98abc-117">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="98abc-118">更新 externalConnection</span><span class="sxs-lookup"><span data-stu-id="98abc-118">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="98abc-119">externalConnection</span><span class="sxs-lookup"><span data-stu-id="98abc-119">externalConnection</span></span>                            | <span data-ttu-id="98abc-120">更新 externalConnection 对象。</span><span class="sxs-lookup"><span data-stu-id="98abc-120">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="98abc-121">删除 externalConnection</span><span class="sxs-lookup"><span data-stu-id="98abc-121">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="98abc-122">无</span><span class="sxs-lookup"><span data-stu-id="98abc-122">None</span></span>                                          | <span data-ttu-id="98abc-123">删除 externalConnection 对象。</span><span class="sxs-lookup"><span data-stu-id="98abc-123">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="98abc-124">创建架构</span><span class="sxs-lookup"><span data-stu-id="98abc-124">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="98abc-125">无*或*[架构](schema.md)</span><span class="sxs-lookup"><span data-stu-id="98abc-125">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="98abc-126">注册连接架构。</span><span class="sxs-lookup"><span data-stu-id="98abc-126">Register connection schema.</span></span> |
| [<span data-ttu-id="98abc-127">Get 操作</span><span class="sxs-lookup"><span data-stu-id="98abc-127">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="98abc-128">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="98abc-128">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="98abc-129">获取用于创建连接架构的异步请求的状态。</span><span class="sxs-lookup"><span data-stu-id="98abc-129">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="98abc-130">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="98abc-130">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="98abc-131">externalItem</span><span class="sxs-lookup"><span data-stu-id="98abc-131">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="98abc-132">通过发布到 items 集合创建新的 externalItem。</span><span class="sxs-lookup"><span data-stu-id="98abc-132">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="98abc-133">属性</span><span class="sxs-lookup"><span data-stu-id="98abc-133">Properties</span></span>

| <span data-ttu-id="98abc-134">属性</span><span class="sxs-lookup"><span data-stu-id="98abc-134">Property</span></span>      | <span data-ttu-id="98abc-135">类型</span><span class="sxs-lookup"><span data-stu-id="98abc-135">Type</span></span>                              | <span data-ttu-id="98abc-136">说明</span><span class="sxs-lookup"><span data-stu-id="98abc-136">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="98abc-137">设置</span><span class="sxs-lookup"><span data-stu-id="98abc-137">configuration</span></span> | [<span data-ttu-id="98abc-138">configuration</span><span class="sxs-lookup"><span data-stu-id="98abc-138">configuration</span></span>](configuration.md) | <span data-ttu-id="98abc-139">指定允许管理连接和索引连接中的内容的其他应用程序 Id。</span><span class="sxs-lookup"><span data-stu-id="98abc-139">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="98abc-140">可选。</span><span class="sxs-lookup"><span data-stu-id="98abc-140">Optional.</span></span> |
| <span data-ttu-id="98abc-141">description</span><span class="sxs-lookup"><span data-stu-id="98abc-141">description</span></span>   | <span data-ttu-id="98abc-142">String</span><span class="sxs-lookup"><span data-stu-id="98abc-142">String</span></span>                            | <span data-ttu-id="98abc-143">Microsoft 365 管理中心显示的连接的说明。</span><span class="sxs-lookup"><span data-stu-id="98abc-143">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="98abc-144">可选。</span><span class="sxs-lookup"><span data-stu-id="98abc-144">Optional.</span></span> |
| <span data-ttu-id="98abc-145">id</span><span class="sxs-lookup"><span data-stu-id="98abc-145">id</span></span>            | <span data-ttu-id="98abc-146">String</span><span class="sxs-lookup"><span data-stu-id="98abc-146">String</span></span>                            | <span data-ttu-id="98abc-147">在 Azure Active Directory 租户中，开发人员提供的连接的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="98abc-147">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="98abc-148">最大长度为32个字符。</span><span class="sxs-lookup"><span data-stu-id="98abc-148">Maximum length of 32 characters.</span></span> <span data-ttu-id="98abc-149">必须仅包含字母数字字符。</span><span class="sxs-lookup"><span data-stu-id="98abc-149">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="98abc-150">不能以`Microsoft`下列值开头，也不能为`None`下列`Directory`值`Exchange`之一`ExchangeArchive`： `LinkedIn`、 `Mailbox` `MicrosoftSearch` `OneDriveBusiness` `SharePoint` `Teams` `Yammer`、、、、、、 `Connectors`、、、。</span><span class="sxs-lookup"><span data-stu-id="98abc-150">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="98abc-151">必需。</span><span class="sxs-lookup"><span data-stu-id="98abc-151">Required.</span></span> |
| <span data-ttu-id="98abc-152">name</span><span class="sxs-lookup"><span data-stu-id="98abc-152">name</span></span>          | <span data-ttu-id="98abc-153">String</span><span class="sxs-lookup"><span data-stu-id="98abc-153">String</span></span>                            | <span data-ttu-id="98abc-154">要显示在 Microsoft 365 管理中心中的连接的显示名称。</span><span class="sxs-lookup"><span data-stu-id="98abc-154">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="98abc-155">最大长度为128个字符。</span><span class="sxs-lookup"><span data-stu-id="98abc-155">Maximum length of 128 characters.</span></span> <span data-ttu-id="98abc-156">必需。</span><span class="sxs-lookup"><span data-stu-id="98abc-156">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="98abc-157">关系</span><span class="sxs-lookup"><span data-stu-id="98abc-157">Relationships</span></span>

| <span data-ttu-id="98abc-158">关系</span><span class="sxs-lookup"><span data-stu-id="98abc-158">Relationship</span></span> | <span data-ttu-id="98abc-159">类型</span><span class="sxs-lookup"><span data-stu-id="98abc-159">Type</span></span>                                                     | <span data-ttu-id="98abc-160">说明</span><span class="sxs-lookup"><span data-stu-id="98abc-160">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="98abc-161">items</span><span class="sxs-lookup"><span data-stu-id="98abc-161">items</span></span>        | <span data-ttu-id="98abc-162">[externalItem](externalitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="98abc-162">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="98abc-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="98abc-p105">Read-only. Nullable.</span></span> |
| <span data-ttu-id="98abc-165">operations</span><span class="sxs-lookup"><span data-stu-id="98abc-165">operations</span></span>   | <span data-ttu-id="98abc-166">[connectionOperation](connectionoperation.md)集合</span><span class="sxs-lookup"><span data-stu-id="98abc-166">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="98abc-167">只读。</span><span class="sxs-lookup"><span data-stu-id="98abc-167">Read-only.</span></span> <span data-ttu-id="98abc-168">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="98abc-168">Nullable.</span></span> |
| <span data-ttu-id="98abc-169">架构</span><span class="sxs-lookup"><span data-stu-id="98abc-169">schema</span></span>       | [<span data-ttu-id="98abc-170">schema</span><span class="sxs-lookup"><span data-stu-id="98abc-170">schema</span></span>](schema.md)                                      | <span data-ttu-id="98abc-p107">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="98abc-p107">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="98abc-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98abc-173">JSON representation</span></span>

<span data-ttu-id="98abc-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98abc-174">The following is a JSON representation of the resource.</span></span>

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
