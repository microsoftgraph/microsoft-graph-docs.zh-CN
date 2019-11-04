---
title: Contact.personname 资源类型
description: Contact.personname 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: aad97177a06933d2dd98c5cc94744450197f7dcb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939598"
---
# <a name="personname-resource-type"></a><span data-ttu-id="c62fa-103">Contact.personname 资源类型</span><span class="sxs-lookup"><span data-stu-id="c62fa-103">personName resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c62fa-104">表示用户提供的、与其相关联的帐户的扩展名称信息。</span><span class="sxs-lookup"><span data-stu-id="c62fa-104">Represents extended name information provided by the user or which they have associated with their account.</span></span>

<span data-ttu-id="c62fa-105">继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c62fa-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c62fa-106">方法</span><span class="sxs-lookup"><span data-stu-id="c62fa-106">Methods</span></span>

| <span data-ttu-id="c62fa-107">方法</span><span class="sxs-lookup"><span data-stu-id="c62fa-107">Method</span></span>                                     | <span data-ttu-id="c62fa-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c62fa-108">Return Type</span></span>                 | <span data-ttu-id="c62fa-109">说明</span><span class="sxs-lookup"><span data-stu-id="c62fa-109">Description</span></span>                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [<span data-ttu-id="c62fa-110">获取 Contact.personname</span><span class="sxs-lookup"><span data-stu-id="c62fa-110">Get personName</span></span>](../api/personname-get.md) | [<span data-ttu-id="c62fa-111">Contact.personname</span><span class="sxs-lookup"><span data-stu-id="c62fa-111">personName</span></span>](personname.md) | <span data-ttu-id="c62fa-112">读取 Contact.personname 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c62fa-112">Read properties and relationships of personName object.</span></span> |
| [<span data-ttu-id="c62fa-113">Update</span><span class="sxs-lookup"><span data-stu-id="c62fa-113">Update</span></span>](../api/personname-update.md)      | [<span data-ttu-id="c62fa-114">Contact.personname</span><span class="sxs-lookup"><span data-stu-id="c62fa-114">personName</span></span>](personname.md) | <span data-ttu-id="c62fa-115">更新 Contact.personname 对象。</span><span class="sxs-lookup"><span data-stu-id="c62fa-115">Update personName object.</span></span>                               |
| [<span data-ttu-id="c62fa-116">删除</span><span class="sxs-lookup"><span data-stu-id="c62fa-116">Delete</span></span>](../api/personname-delete.md)      | <span data-ttu-id="c62fa-117">无</span><span class="sxs-lookup"><span data-stu-id="c62fa-117">None</span></span>                        | <span data-ttu-id="c62fa-118">删除 Contact.personname 对象。</span><span class="sxs-lookup"><span data-stu-id="c62fa-118">Delete personName object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="c62fa-119">属性</span><span class="sxs-lookup"><span data-stu-id="c62fa-119">Properties</span></span>

| <span data-ttu-id="c62fa-120">属性</span><span class="sxs-lookup"><span data-stu-id="c62fa-120">Property</span></span>     | <span data-ttu-id="c62fa-121">类型</span><span class="sxs-lookup"><span data-stu-id="c62fa-121">Type</span></span>                              | <span data-ttu-id="c62fa-122">说明</span><span class="sxs-lookup"><span data-stu-id="c62fa-122">Description</span></span> |
|:-------------|:----------------------------------|:------------|
|<span data-ttu-id="c62fa-123">displayName</span><span class="sxs-lookup"><span data-stu-id="c62fa-123">displayName</span></span>   |<span data-ttu-id="c62fa-124">String</span><span class="sxs-lookup"><span data-stu-id="c62fa-124">String</span></span>                             | <span data-ttu-id="c62fa-125">根据用户或其设备的区域设置，提供 firstName 和 lastName 的顺序呈现。</span><span class="sxs-lookup"><span data-stu-id="c62fa-125">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span> |
|<span data-ttu-id="c62fa-126">前</span><span class="sxs-lookup"><span data-stu-id="c62fa-126">first</span></span>         |<span data-ttu-id="c62fa-127">字符串</span><span class="sxs-lookup"><span data-stu-id="c62fa-127">String</span></span>                             | <span data-ttu-id="c62fa-128">用户的名字。</span><span class="sxs-lookup"><span data-stu-id="c62fa-128">First Name of the user.</span></span>                                                                                      |
|<span data-ttu-id="c62fa-129">initials</span><span class="sxs-lookup"><span data-stu-id="c62fa-129">initials</span></span>      |<span data-ttu-id="c62fa-130">String</span><span class="sxs-lookup"><span data-stu-id="c62fa-130">String</span></span>                             | <span data-ttu-id="c62fa-131">用户的首字母缩写。</span><span class="sxs-lookup"><span data-stu-id="c62fa-131">Initials of the user.</span></span>                                                                                        |
|<span data-ttu-id="c62fa-132">languageTag</span><span class="sxs-lookup"><span data-stu-id="c62fa-132">languageTag</span></span>   |<span data-ttu-id="c62fa-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c62fa-133">String</span></span>                             | <span data-ttu-id="c62fa-134">包含遵循 IETF BCP47 格式的语言（en-us，无 NB，en-us）的名称。</span><span class="sxs-lookup"><span data-stu-id="c62fa-134">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>                        |
|<span data-ttu-id="c62fa-135">末</span><span class="sxs-lookup"><span data-stu-id="c62fa-135">last</span></span>          |<span data-ttu-id="c62fa-136">字符串</span><span class="sxs-lookup"><span data-stu-id="c62fa-136">String</span></span>                             | <span data-ttu-id="c62fa-137">用户的姓氏。</span><span class="sxs-lookup"><span data-stu-id="c62fa-137">Last Name of the user.</span></span>                                                                                       |
|<span data-ttu-id="c62fa-138">maiden</span><span class="sxs-lookup"><span data-stu-id="c62fa-138">maiden</span></span>        |<span data-ttu-id="c62fa-139">字符串</span><span class="sxs-lookup"><span data-stu-id="c62fa-139">String</span></span>                             | <span data-ttu-id="c62fa-140">Maiden 用户的名称。</span><span class="sxs-lookup"><span data-stu-id="c62fa-140">Maiden Name of the user.</span></span>                                                                                     |
|<span data-ttu-id="c62fa-141">中间</span><span class="sxs-lookup"><span data-stu-id="c62fa-141">middle</span></span>        |<span data-ttu-id="c62fa-142">字符串</span><span class="sxs-lookup"><span data-stu-id="c62fa-142">String</span></span>                             | <span data-ttu-id="c62fa-143">Middlie 用户的名称。</span><span class="sxs-lookup"><span data-stu-id="c62fa-143">Middlie Name of the user.</span></span>                                                                                    | 
|<span data-ttu-id="c62fa-144">昵称</span><span class="sxs-lookup"><span data-stu-id="c62fa-144">nickname</span></span>      |<span data-ttu-id="c62fa-145">字符串</span><span class="sxs-lookup"><span data-stu-id="c62fa-145">String</span></span>                             | <span data-ttu-id="c62fa-146">用户的昵称。</span><span class="sxs-lookup"><span data-stu-id="c62fa-146">Nickname of the user.</span></span>                                                                                        |
|<span data-ttu-id="c62fa-147">拼音</span><span class="sxs-lookup"><span data-stu-id="c62fa-147">pronunciation</span></span> |[<span data-ttu-id="c62fa-148">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="c62fa-148">yomiPersonName</span></span>](yomipersonname.md)| <span data-ttu-id="c62fa-149">有关如何对用户名称进行发音的指南。</span><span class="sxs-lookup"><span data-stu-id="c62fa-149">Guidance on how to pronounce the users name.</span></span>                                                                 |
|<span data-ttu-id="c62fa-150">后缀</span><span class="sxs-lookup"><span data-stu-id="c62fa-150">suffix</span></span>        |<span data-ttu-id="c62fa-151">字符串</span><span class="sxs-lookup"><span data-stu-id="c62fa-151">String</span></span>                             | <span data-ttu-id="c62fa-152">Users 名称之后使用的指示符（例如：博士）。</span><span class="sxs-lookup"><span data-stu-id="c62fa-152">Designators used after the users name (eg: PhD.)</span></span>                                                             |
|<span data-ttu-id="c62fa-153">title</span><span class="sxs-lookup"><span data-stu-id="c62fa-153">title</span></span>         |<span data-ttu-id="c62fa-154">字符串</span><span class="sxs-lookup"><span data-stu-id="c62fa-154">String</span></span>                             | <span data-ttu-id="c62fa-155">Honorifics 用于为用户名称加前缀（例如： Dr.、罗德、Madam、Mrs）</span><span class="sxs-lookup"><span data-stu-id="c62fa-155">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>                                            |

## <a name="relationships"></a><span data-ttu-id="c62fa-156">关系</span><span class="sxs-lookup"><span data-stu-id="c62fa-156">Relationships</span></span>

<span data-ttu-id="c62fa-157">无</span><span class="sxs-lookup"><span data-stu-id="c62fa-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c62fa-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c62fa-158">JSON representation</span></span>

<span data-ttu-id="c62fa-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c62fa-159">The following is a JSON representation of the resource.</span></span>

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