---
title: Contact.personname 资源类型
description: Contact.personname 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e4927ba05443d4b54eaac3f54b7e0d3a8cd62159
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227688"
---
# <a name="personname-resource-type"></a><span data-ttu-id="5b27b-103">Contact.personname 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b27b-103">personName resource type</span></span>

<span data-ttu-id="5b27b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b27b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b27b-105">表示用户提供的、与其相关联的帐户的扩展名称信息。</span><span class="sxs-lookup"><span data-stu-id="5b27b-105">Represents extended name information provided by the user or which they have associated with their account.</span></span>

<span data-ttu-id="5b27b-106">继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="5b27b-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5b27b-107">方法</span><span class="sxs-lookup"><span data-stu-id="5b27b-107">Methods</span></span>

| <span data-ttu-id="5b27b-108">方法</span><span class="sxs-lookup"><span data-stu-id="5b27b-108">Method</span></span>                                     | <span data-ttu-id="5b27b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5b27b-109">Return Type</span></span>                 | <span data-ttu-id="5b27b-110">说明</span><span class="sxs-lookup"><span data-stu-id="5b27b-110">Description</span></span>                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [<span data-ttu-id="5b27b-111">获取 Contact.personname</span><span class="sxs-lookup"><span data-stu-id="5b27b-111">Get personName</span></span>](../api/personname-get.md) | [<span data-ttu-id="5b27b-112">Contact.personname</span><span class="sxs-lookup"><span data-stu-id="5b27b-112">personName</span></span>](personname.md) | <span data-ttu-id="5b27b-113">读取 Contact.personname 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5b27b-113">Read properties and relationships of personName object.</span></span> |
| [<span data-ttu-id="5b27b-114">更新</span><span class="sxs-lookup"><span data-stu-id="5b27b-114">Update</span></span>](../api/personname-update.md)      | [<span data-ttu-id="5b27b-115">Contact.personname</span><span class="sxs-lookup"><span data-stu-id="5b27b-115">personName</span></span>](personname.md) | <span data-ttu-id="5b27b-116">更新 Contact.personname 对象。</span><span class="sxs-lookup"><span data-stu-id="5b27b-116">Update personName object.</span></span>                               |
| [<span data-ttu-id="5b27b-117">删除</span><span class="sxs-lookup"><span data-stu-id="5b27b-117">Delete</span></span>](../api/personname-delete.md)      | <span data-ttu-id="5b27b-118">无</span><span class="sxs-lookup"><span data-stu-id="5b27b-118">None</span></span>                        | <span data-ttu-id="5b27b-119">删除 Contact.personname 对象。</span><span class="sxs-lookup"><span data-stu-id="5b27b-119">Delete personName object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="5b27b-120">属性</span><span class="sxs-lookup"><span data-stu-id="5b27b-120">Properties</span></span>

| <span data-ttu-id="5b27b-121">属性</span><span class="sxs-lookup"><span data-stu-id="5b27b-121">Property</span></span>     | <span data-ttu-id="5b27b-122">类型</span><span class="sxs-lookup"><span data-stu-id="5b27b-122">Type</span></span>                              | <span data-ttu-id="5b27b-123">说明</span><span class="sxs-lookup"><span data-stu-id="5b27b-123">Description</span></span>                                                                                                  |
|:-------------|:----------------------------------|:-------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="5b27b-124">displayName</span><span class="sxs-lookup"><span data-stu-id="5b27b-124">displayName</span></span>   |<span data-ttu-id="5b27b-125">String</span><span class="sxs-lookup"><span data-stu-id="5b27b-125">String</span></span>                             | <span data-ttu-id="5b27b-126">根据用户或其设备的区域设置，提供 firstName 和 lastName 的顺序呈现。</span><span class="sxs-lookup"><span data-stu-id="5b27b-126">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span> |
|<span data-ttu-id="5b27b-127">前</span><span class="sxs-lookup"><span data-stu-id="5b27b-127">first</span></span>         |<span data-ttu-id="5b27b-128">String</span><span class="sxs-lookup"><span data-stu-id="5b27b-128">String</span></span>                             | <span data-ttu-id="5b27b-129">用户的名字。</span><span class="sxs-lookup"><span data-stu-id="5b27b-129">First Name of the user.</span></span>                                                                                      |
|<span data-ttu-id="5b27b-130">initials</span><span class="sxs-lookup"><span data-stu-id="5b27b-130">initials</span></span>      |<span data-ttu-id="5b27b-131">String</span><span class="sxs-lookup"><span data-stu-id="5b27b-131">String</span></span>                             | <span data-ttu-id="5b27b-132">用户的首字母缩写。</span><span class="sxs-lookup"><span data-stu-id="5b27b-132">Initials of the user.</span></span>                                                                                        |
|<span data-ttu-id="5b27b-133">languageTag</span><span class="sxs-lookup"><span data-stu-id="5b27b-133">languageTag</span></span>   |<span data-ttu-id="5b27b-134">String</span><span class="sxs-lookup"><span data-stu-id="5b27b-134">String</span></span>                             | <span data-ttu-id="5b27b-135">包含遵循 IETF BCP47 格式的语言（en-us，无 NB，en-us）的名称。</span><span class="sxs-lookup"><span data-stu-id="5b27b-135">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>                        |
|<span data-ttu-id="5b27b-136">末</span><span class="sxs-lookup"><span data-stu-id="5b27b-136">last</span></span>          |<span data-ttu-id="5b27b-137">String</span><span class="sxs-lookup"><span data-stu-id="5b27b-137">String</span></span>                             | <span data-ttu-id="5b27b-138">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="5b27b-138">Last Name of the user.</span></span>                                                                                       |
|<span data-ttu-id="5b27b-139">maiden</span><span class="sxs-lookup"><span data-stu-id="5b27b-139">maiden</span></span>        |<span data-ttu-id="5b27b-140">String</span><span class="sxs-lookup"><span data-stu-id="5b27b-140">String</span></span>                             | <span data-ttu-id="5b27b-141">Maiden 用户的名称。</span><span class="sxs-lookup"><span data-stu-id="5b27b-141">Maiden Name of the user.</span></span>                                                                                     |
|<span data-ttu-id="5b27b-142">中间</span><span class="sxs-lookup"><span data-stu-id="5b27b-142">middle</span></span>        |<span data-ttu-id="5b27b-143">String</span><span class="sxs-lookup"><span data-stu-id="5b27b-143">String</span></span>                             | <span data-ttu-id="5b27b-144">Middlie 用户的名称。</span><span class="sxs-lookup"><span data-stu-id="5b27b-144">Middlie Name of the user.</span></span>                                                                                    |
|<span data-ttu-id="5b27b-145">昵称</span><span class="sxs-lookup"><span data-stu-id="5b27b-145">nickname</span></span>      |<span data-ttu-id="5b27b-146">String</span><span class="sxs-lookup"><span data-stu-id="5b27b-146">String</span></span>                             | <span data-ttu-id="5b27b-147">用户的昵称。</span><span class="sxs-lookup"><span data-stu-id="5b27b-147">Nickname of the user.</span></span>                                                                                        |
|<span data-ttu-id="5b27b-148">拼音</span><span class="sxs-lookup"><span data-stu-id="5b27b-148">pronunciation</span></span> |[<span data-ttu-id="5b27b-149">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="5b27b-149">yomiPersonName</span></span>](yomipersonname.md)| <span data-ttu-id="5b27b-150">有关如何对用户名称进行发音的指南。</span><span class="sxs-lookup"><span data-stu-id="5b27b-150">Guidance on how to pronounce the users name.</span></span>                                                                 |
|<span data-ttu-id="5b27b-151">后缀</span><span class="sxs-lookup"><span data-stu-id="5b27b-151">suffix</span></span>        |<span data-ttu-id="5b27b-152">String</span><span class="sxs-lookup"><span data-stu-id="5b27b-152">String</span></span>                             | <span data-ttu-id="5b27b-153">Users 名称之后使用的指示符（例如：博士）。</span><span class="sxs-lookup"><span data-stu-id="5b27b-153">Designators used after the users name (eg: PhD.)</span></span>                                                             |
|<span data-ttu-id="5b27b-154">title</span><span class="sxs-lookup"><span data-stu-id="5b27b-154">title</span></span>         |<span data-ttu-id="5b27b-155">字符串</span><span class="sxs-lookup"><span data-stu-id="5b27b-155">String</span></span>                             | <span data-ttu-id="5b27b-156">Honorifics 用于为用户名称加前缀（例如： Dr.、罗德、Madam、Mrs）</span><span class="sxs-lookup"><span data-stu-id="5b27b-156">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>                                            |

## <a name="relationships"></a><span data-ttu-id="5b27b-157">关系</span><span class="sxs-lookup"><span data-stu-id="5b27b-157">Relationships</span></span>

<span data-ttu-id="5b27b-158">无</span><span class="sxs-lookup"><span data-stu-id="5b27b-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b27b-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b27b-159">JSON representation</span></span>

<span data-ttu-id="5b27b-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b27b-160">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personName",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "first": "String",
  "initials": "String",
  "languageTag": "String",
  "last": "String",
  "maiden": "String",
  "middle": "String",
  "nickname": "String",
  "pronunciation": {"@odata.type": "microsoft.graph.yomiPersonName"},
  "suffix": "String",
  "title": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personName resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->