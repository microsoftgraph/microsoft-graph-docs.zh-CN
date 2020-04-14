---
title: extensionProperty 资源类型
description: 表示目录扩展
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3d6f6e89ca6e54e1c74e43c6201766aa199f454d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43423795"
---
# <a name="extensionproperty-resource-type"></a><span data-ttu-id="67b6a-103">extensionProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="67b6a-103">extensionProperty resource type</span></span>

<span data-ttu-id="67b6a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67b6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67b6a-105">表示可用于将自定义属性添加到目录对象而不需要外部数据存储区的目录扩展。</span><span class="sxs-lookup"><span data-stu-id="67b6a-105">Represents a directory extension that can be used to add a custom property to directory objects without requiring an external data store.</span></span> <span data-ttu-id="67b6a-106">例如，如果组织具有需要目录中每个用户的 Skype ID 的业务线（LOB）应用程序，则可以使用 Microsoft Graph 在目录的 User 对象上注册一个名为 skypeId 的新属性，然后为特定用户的新属性写入一个值。</span><span class="sxs-lookup"><span data-stu-id="67b6a-106">For example, if an organization has a line of business (LOB) application that requires a Skype ID for each user in the directory, Microsoft Graph can be used to register a new property named skypeId on the directory’s User object, and then write a value to the new property for a specific user.</span></span>

<span data-ttu-id="67b6a-107">可以将扩展添加到[用户](user.md)、[组](group.md)、[组织](organization.md)、[设备](device.md)、[应用程序](application.md)资源。</span><span class="sxs-lookup"><span data-stu-id="67b6a-107">Extensions can be added to [user](user.md), [group](group.md), [organization](organization.md), [device](device.md), [application](application.md) resources.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="67b6a-108">此处介绍的 Azure AD 架构扩展在 Microsoft Graph 中可用，仅用于向后兼容的原因。</span><span class="sxs-lookup"><span data-stu-id="67b6a-108">Azure AD schema extensions described here are available in Microsoft Graph for backwards compatibility reasons only.</span></span>
> <span data-ttu-id="67b6a-109">它允许您使用 Microsoft Graph 继续管理通过 Azure AD Graph 或[AZURE Ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect)添加的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="67b6a-109">It allows you to use Microsoft Graph to continue to manage extension properties added through Azure AD Graph or [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).</span></span>
> <span data-ttu-id="67b6a-110">对于新的自定义扩展，我们建议使用 Microsoft Graph 架构扩展[将自定义数据添加到资源](/graph/extensibility-overview)。</span><span class="sxs-lookup"><span data-stu-id="67b6a-110">For new custom extensions, we recommend that you use Microsoft Graph schema extensions for [adding custom data to resources](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="67b6a-111">方法</span><span class="sxs-lookup"><span data-stu-id="67b6a-111">Methods</span></span>

| <span data-ttu-id="67b6a-112">方法</span><span class="sxs-lookup"><span data-stu-id="67b6a-112">Method</span></span>       | <span data-ttu-id="67b6a-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="67b6a-113">Return Type</span></span> | <span data-ttu-id="67b6a-114">说明</span><span class="sxs-lookup"><span data-stu-id="67b6a-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="67b6a-115">列出扩展</span><span class="sxs-lookup"><span data-stu-id="67b6a-115">List extensions</span></span>](../api/application-list-extensionproperty.md) | <span data-ttu-id="67b6a-116">[extensionProperty](extensionProperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67b6a-116">[extensionProperty](extensionProperty.md) collection</span></span> | <span data-ttu-id="67b6a-117">列出应用程序对象上的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="67b6a-117">List extension properties on an application object.</span></span> |
| [<span data-ttu-id="67b6a-118">创建扩展</span><span class="sxs-lookup"><span data-stu-id="67b6a-118">Create extension</span></span>](../api/application-post-extensionproperty.md) | [<span data-ttu-id="67b6a-119">extensionProperty</span><span class="sxs-lookup"><span data-stu-id="67b6a-119">extensionProperty</span></span>](extensionProperty.md) | <span data-ttu-id="67b6a-120">在应用程序对象上创建扩展属性。</span><span class="sxs-lookup"><span data-stu-id="67b6a-120">Create an extension property on an application object.</span></span> |
| [<span data-ttu-id="67b6a-121">删除扩展</span><span class="sxs-lookup"><span data-stu-id="67b6a-121">Delete extension</span></span>](../api/application-delete-extensionproperty.md) | <span data-ttu-id="67b6a-122">无</span><span class="sxs-lookup"><span data-stu-id="67b6a-122">None</span></span> | <span data-ttu-id="67b6a-123">从应用程序对象删除扩展属性。</span><span class="sxs-lookup"><span data-stu-id="67b6a-123">Delete an extension property from an application object.</span></span> |

## <a name="properties"></a><span data-ttu-id="67b6a-124">属性</span><span class="sxs-lookup"><span data-stu-id="67b6a-124">Properties</span></span>

| <span data-ttu-id="67b6a-125">属性</span><span class="sxs-lookup"><span data-stu-id="67b6a-125">Property</span></span>     | <span data-ttu-id="67b6a-126">类型</span><span class="sxs-lookup"><span data-stu-id="67b6a-126">Type</span></span>        | <span data-ttu-id="67b6a-127">说明</span><span class="sxs-lookup"><span data-stu-id="67b6a-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="67b6a-128">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="67b6a-128">appDisplayName</span></span>|<span data-ttu-id="67b6a-129">String</span><span class="sxs-lookup"><span data-stu-id="67b6a-129">String</span></span>| <span data-ttu-id="67b6a-130">在其上定义此扩展属性的 application 对象的显示名称。</span><span class="sxs-lookup"><span data-stu-id="67b6a-130">Display name of the application object on which this extension property is defined.</span></span> <span data-ttu-id="67b6a-131">只读。</span><span class="sxs-lookup"><span data-stu-id="67b6a-131">Read-only.</span></span> |
|<span data-ttu-id="67b6a-132">DataType</span><span class="sxs-lookup"><span data-stu-id="67b6a-132">dataType</span></span>|<span data-ttu-id="67b6a-133">String</span><span class="sxs-lookup"><span data-stu-id="67b6a-133">String</span></span>| <span data-ttu-id="67b6a-134">指定 extension 属性可以包含的值的数据类型。</span><span class="sxs-lookup"><span data-stu-id="67b6a-134">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="67b6a-135">支持以下值。</span><span class="sxs-lookup"><span data-stu-id="67b6a-135">Following values are supported.</span></span> <span data-ttu-id="67b6a-136">不可为空。</span><span class="sxs-lookup"><span data-stu-id="67b6a-136">Not nullable.</span></span> <ul><li><span data-ttu-id="67b6a-137">`Binary`-最多为256字节</span><span class="sxs-lookup"><span data-stu-id="67b6a-137">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="67b6a-138">`DateTime`-必须以 ISO 8601 格式指定。</span><span class="sxs-lookup"><span data-stu-id="67b6a-138">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="67b6a-139">存储为 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="67b6a-139">Will be stored in UTC.</span></span></li><li><span data-ttu-id="67b6a-140">`Integer`-32-位值。</span><span class="sxs-lookup"><span data-stu-id="67b6a-140">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="67b6a-141">`LargeInteger`-64-位值。</span><span class="sxs-lookup"><span data-stu-id="67b6a-141">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="67b6a-142">`String`-最多为-256 个字符</span><span class="sxs-lookup"><span data-stu-id="67b6a-142">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="67b6a-143">isSyncedFromOnPremises</span><span class="sxs-lookup"><span data-stu-id="67b6a-143">isSyncedFromOnPremises</span></span>|<span data-ttu-id="67b6a-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="67b6a-144">Boolean</span></span>| <span data-ttu-id="67b6a-145">指示是否使用 Azure AD Connect 从 onpremises 目录中 sycned 此扩展属性。</span><span class="sxs-lookup"><span data-stu-id="67b6a-145">Indicates if this extension property was sycned from onpremises directory using Azure AD Connect.</span></span> <span data-ttu-id="67b6a-146">只读。</span><span class="sxs-lookup"><span data-stu-id="67b6a-146">Read-only.</span></span> |
|<span data-ttu-id="67b6a-147">name</span><span class="sxs-lookup"><span data-stu-id="67b6a-147">name</span></span>|<span data-ttu-id="67b6a-148">字符串</span><span class="sxs-lookup"><span data-stu-id="67b6a-148">String</span></span>| <span data-ttu-id="67b6a-149">扩展属性的名称。</span><span class="sxs-lookup"><span data-stu-id="67b6a-149">Name of the extension property.</span></span> <span data-ttu-id="67b6a-150">不可为空。</span><span class="sxs-lookup"><span data-stu-id="67b6a-150">Not nullable.</span></span> |
|<span data-ttu-id="67b6a-151">targetObjects</span><span class="sxs-lookup"><span data-stu-id="67b6a-151">targetObjects</span></span>|<span data-ttu-id="67b6a-152">String 集合</span><span class="sxs-lookup"><span data-stu-id="67b6a-152">String collection</span></span>| <span data-ttu-id="67b6a-153">支持以下值。</span><span class="sxs-lookup"><span data-stu-id="67b6a-153">Following values are supported.</span></span> <span data-ttu-id="67b6a-154">不可为空。</span><span class="sxs-lookup"><span data-stu-id="67b6a-154">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a><span data-ttu-id="67b6a-155">关系</span><span class="sxs-lookup"><span data-stu-id="67b6a-155">Relationships</span></span>

<span data-ttu-id="67b6a-156">无</span><span class="sxs-lookup"><span data-stu-id="67b6a-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67b6a-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67b6a-157">JSON representation</span></span>

<span data-ttu-id="67b6a-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67b6a-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionProperty",
  "baseType": "",
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
