---
title: extensionProperty 资源类型
description: 表示目录扩展
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 33603d0d16cc44fd2f07177da4c6c6bb4208b082
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941783"
---
# <a name="extensionproperty-resource-type"></a><span data-ttu-id="dd8bf-103">extensionProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd8bf-103">extensionProperty resource type</span></span>

<span data-ttu-id="dd8bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd8bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd8bf-105">表示一个目录扩展，可用于向目录对象添加自定义属性，而无需外部数据存储。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-105">Represents a directory extension that can be used to add a custom property to directory objects without requiring an external data store.</span></span> <span data-ttu-id="dd8bf-106">例如，如果组织的业务线 (LOB) 应用程序需要目录中每个用户的 Skype ID，则 Microsoft Graph 可用于在目录的 User 对象上注册名为 skypeId 的新属性，然后为特定用户的新属性写入值。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-106">For example, if an organization has a line of business (LOB) application that requires a Skype ID for each user in the directory, Microsoft Graph can be used to register a new property named skypeId on the directory’s User object, and then write a value to the new property for a specific user.</span></span>

<span data-ttu-id="dd8bf-107">可以将扩展添加到[用户](user.md)、组、[组织、](organization.md)[设备](device.md)[、应用程序](application.md)资源。 [](group.md)</span><span class="sxs-lookup"><span data-stu-id="dd8bf-107">Extensions can be added to [user](user.md), [group](group.md), [organization](organization.md), [device](device.md), [application](application.md) resources.</span></span> <span data-ttu-id="dd8bf-108">所有类型和所有应用程序中只能将 100个扩展值写入任何单个 Azure AD 资源。 </span><span class="sxs-lookup"><span data-stu-id="dd8bf-108">Only 100 extension values, across *all* types and *all* applications, can be written to any single Azure AD resource.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="dd8bf-109">此处所述的 Azure AD 架构扩展仅在出于向后兼容性原因才在 Microsoft Graph 中提供。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-109">Azure AD schema extensions described here are available in Microsoft Graph for backwards compatibility reasons only.</span></span>
> <span data-ttu-id="dd8bf-110">它允许你使用 Microsoft Graph 继续管理通过 Azure AD Graph 或 [Azure AD Connect 添加的扩展属性](/azure/active-directory/hybrid/whatis-azure-ad-connect)。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-110">It allows you to use Microsoft Graph to continue to manage extension properties added through Azure AD Graph or [Azure AD Connect](/azure/active-directory/hybrid/whatis-azure-ad-connect).</span></span>
> <span data-ttu-id="dd8bf-111">对于新的自定义扩展，建议使用 Microsoft Graph 架构扩展向 [资源添加自定义数据](/graph/extensibility-overview)。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-111">For new custom extensions, we recommend that you use Microsoft Graph schema extensions for [adding custom data to resources](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="dd8bf-112">Methods</span><span class="sxs-lookup"><span data-stu-id="dd8bf-112">Methods</span></span>

| <span data-ttu-id="dd8bf-113">方法</span><span class="sxs-lookup"><span data-stu-id="dd8bf-113">Method</span></span>       | <span data-ttu-id="dd8bf-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="dd8bf-114">Return Type</span></span> | <span data-ttu-id="dd8bf-115">说明</span><span class="sxs-lookup"><span data-stu-id="dd8bf-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dd8bf-116">列出扩展</span><span class="sxs-lookup"><span data-stu-id="dd8bf-116">List extensions</span></span>](../api/application-list-extensionproperty.md) | <span data-ttu-id="dd8bf-117">[extensionProperty](extensionProperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dd8bf-117">[extensionProperty](extensionProperty.md) collection</span></span> | <span data-ttu-id="dd8bf-118">列出应用程序对象上的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-118">List extension properties on an application object.</span></span> |
| [<span data-ttu-id="dd8bf-119">创建扩展</span><span class="sxs-lookup"><span data-stu-id="dd8bf-119">Create extension</span></span>](../api/application-post-extensionproperty.md) | [<span data-ttu-id="dd8bf-120">extensionProperty</span><span class="sxs-lookup"><span data-stu-id="dd8bf-120">extensionProperty</span></span>](extensionProperty.md) | <span data-ttu-id="dd8bf-121">在应用程序对象上创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-121">Create an extension property on an application object.</span></span> |
| [<span data-ttu-id="dd8bf-122">删除扩展</span><span class="sxs-lookup"><span data-stu-id="dd8bf-122">Delete extension</span></span>](../api/application-delete-extensionproperty.md) | <span data-ttu-id="dd8bf-123">无</span><span class="sxs-lookup"><span data-stu-id="dd8bf-123">None</span></span> | <span data-ttu-id="dd8bf-124">从应用程序对象删除扩展属性。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-124">Delete an extension property from an application object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dd8bf-125">属性</span><span class="sxs-lookup"><span data-stu-id="dd8bf-125">Properties</span></span>

| <span data-ttu-id="dd8bf-126">属性</span><span class="sxs-lookup"><span data-stu-id="dd8bf-126">Property</span></span>     | <span data-ttu-id="dd8bf-127">类型</span><span class="sxs-lookup"><span data-stu-id="dd8bf-127">Type</span></span>        | <span data-ttu-id="dd8bf-128">说明</span><span class="sxs-lookup"><span data-stu-id="dd8bf-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd8bf-129">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="dd8bf-129">appDisplayName</span></span>|<span data-ttu-id="dd8bf-130">String</span><span class="sxs-lookup"><span data-stu-id="dd8bf-130">String</span></span>| <span data-ttu-id="dd8bf-131">定义此扩展属性的应用程序对象的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-131">Display name of the application object on which this extension property is defined.</span></span> <span data-ttu-id="dd8bf-132">只读。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-132">Read-only.</span></span> |
|<span data-ttu-id="dd8bf-133">DataType</span><span class="sxs-lookup"><span data-stu-id="dd8bf-133">dataType</span></span>|<span data-ttu-id="dd8bf-134">String</span><span class="sxs-lookup"><span data-stu-id="dd8bf-134">String</span></span>| <span data-ttu-id="dd8bf-135">指定数据类型属性可以保留的值的值的值。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-135">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="dd8bf-136">支持以下值。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-136">Following values are supported.</span></span> <span data-ttu-id="dd8bf-137">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-137">Not nullable.</span></span> <ul><li><span data-ttu-id="dd8bf-138">`Binary` - 最多 256 个字节</span><span class="sxs-lookup"><span data-stu-id="dd8bf-138">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="dd8bf-139">`DateTime` - 必须以 ISO 8601 格式指定。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-139">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="dd8bf-140">存储为 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-140">Will be stored in UTC.</span></span></li><li><span data-ttu-id="dd8bf-141">`Integer` - 32 位值。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-141">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="dd8bf-142">`LargeInteger` - 64 位值。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-142">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="dd8bf-143">`String` - 最多 256 个字符</span><span class="sxs-lookup"><span data-stu-id="dd8bf-143">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="dd8bf-144">isSyncedFromOnPremises</span><span class="sxs-lookup"><span data-stu-id="dd8bf-144">isSyncedFromOnPremises</span></span>|<span data-ttu-id="dd8bf-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd8bf-145">Boolean</span></span>| <span data-ttu-id="dd8bf-146">指示此扩展属性是否来自使用 Azure AD Connect 的 onpremises 目录。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-146">Indicates if this extension property was sycned from onpremises directory using Azure AD Connect.</span></span> <span data-ttu-id="dd8bf-147">只读。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-147">Read-only.</span></span> |
|<span data-ttu-id="dd8bf-148">name</span><span class="sxs-lookup"><span data-stu-id="dd8bf-148">name</span></span>|<span data-ttu-id="dd8bf-149">String</span><span class="sxs-lookup"><span data-stu-id="dd8bf-149">String</span></span>| <span data-ttu-id="dd8bf-150">扩展属性的名称。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-150">Name of the extension property.</span></span> <span data-ttu-id="dd8bf-151">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-151">Not nullable.</span></span> |
|<span data-ttu-id="dd8bf-152">targetObjects</span><span class="sxs-lookup"><span data-stu-id="dd8bf-152">targetObjects</span></span>|<span data-ttu-id="dd8bf-153">String collection</span><span class="sxs-lookup"><span data-stu-id="dd8bf-153">String collection</span></span>| <span data-ttu-id="dd8bf-154">支持以下值。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-154">Following values are supported.</span></span> <span data-ttu-id="dd8bf-155">不可为空。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-155">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a><span data-ttu-id="dd8bf-156">关系</span><span class="sxs-lookup"><span data-stu-id="dd8bf-156">Relationships</span></span>

<span data-ttu-id="dd8bf-157">无</span><span class="sxs-lookup"><span data-stu-id="dd8bf-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd8bf-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd8bf-158">JSON representation</span></span>

<span data-ttu-id="dd8bf-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd8bf-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionProperty",
  "keyProperty": "id"
}-->

```json
{
  "appDisplayName": "String",
  "dataType": "String",
  "isSyncedFromOnPremises": true,
  "name": "String",
  "targetObjects": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
