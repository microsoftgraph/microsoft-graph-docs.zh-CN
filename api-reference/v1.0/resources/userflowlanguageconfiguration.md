---
title: userFlowLanguageConfiguration 资源类型
description: 允许用户流支持多种语言。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 556860eb77c4707f1d180b7924ae3126958a4799
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547202"
---
# <a name="userflowlanguageconfiguration-resource-type"></a><span data-ttu-id="88404-103">userFlowLanguageConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="88404-103">userFlowLanguageConfiguration resource type</span></span>

<span data-ttu-id="88404-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88404-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="88404-105">允许用户流来支持多种语言的使用。</span><span class="sxs-lookup"><span data-stu-id="88404-105">Allows a user flow to support the use of multiple languages.</span></span>

<span data-ttu-id="88404-106">For [Azure Active Directory user flows](/azure/active-directory/external-identities/user-flow-customize-language)， you can only leverage the built-in languages provided by Microsoft.</span><span class="sxs-lookup"><span data-stu-id="88404-106">For [Azure Active Directory user flows](/azure/active-directory/external-identities/user-flow-customize-language), you can only leverage the built-in languages provided by Microsoft.</span></span> <span data-ttu-id="88404-107">用户流Azure Active Directory定义当用户通过用户流配置的旅程时向用户显示的语言和字符串。</span><span class="sxs-lookup"><span data-stu-id="88404-107">User flows for Azure Active Directory support defining the language and strings shown to users as they go through the journeys you configure with your user flows.</span></span>

## <a name="methods"></a><span data-ttu-id="88404-108">方法</span><span class="sxs-lookup"><span data-stu-id="88404-108">Methods</span></span>

|<span data-ttu-id="88404-109">方法</span><span class="sxs-lookup"><span data-stu-id="88404-109">Method</span></span>|<span data-ttu-id="88404-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="88404-110">Return type</span></span>|<span data-ttu-id="88404-111">说明</span><span class="sxs-lookup"><span data-stu-id="88404-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88404-112">获取 userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="88404-112">Get userFlowLanguageConfiguration</span></span>](../api/userflowlanguageconfiguration-get.md)|[<span data-ttu-id="88404-113">userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="88404-113">userFlowLanguageConfiguration</span></span>](../resources/userflowlanguageconfiguration.md)|<span data-ttu-id="88404-114">读取 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88404-114">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="88404-115">这些对象表示用户流中可用的语言。</span><span class="sxs-lookup"><span data-stu-id="88404-115">These objects represent a language available in a user flow.</span></span>|
|[<span data-ttu-id="88404-116">列出 defaultPages</span><span class="sxs-lookup"><span data-stu-id="88404-116">List defaultPages</span></span>](../api/userflowlanguageconfiguration-list-defaultpages.md)|<span data-ttu-id="88404-117">[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88404-117">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="88404-118">从 defaultPages 导航属性获取 userFlowLanguagePage 资源。</span><span class="sxs-lookup"><span data-stu-id="88404-118">Get the userFlowLanguagePage resources from the defaultPages navigation property.</span></span> <span data-ttu-id="88404-119">表示用户流中的默认用户旅程。</span><span class="sxs-lookup"><span data-stu-id="88404-119">Represents the default user journey in a user flow.</span></span>|
|[<span data-ttu-id="88404-120">List overridesPages</span><span class="sxs-lookup"><span data-stu-id="88404-120">List overridesPages</span></span>](../api/userflowlanguageconfiguration-list-overridespages.md)|<span data-ttu-id="88404-121">[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88404-121">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="88404-122">从 overridesPages 导航属性获取 userFlowLanguagePage 资源。</span><span class="sxs-lookup"><span data-stu-id="88404-122">Get the userFlowLanguagePage resources from the overridesPages navigation property.</span></span> <span data-ttu-id="88404-123">表示用户流中的用户旅程的自定义体验。</span><span class="sxs-lookup"><span data-stu-id="88404-123">Represents a custom experience for a user journey in a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="88404-124">属性</span><span class="sxs-lookup"><span data-stu-id="88404-124">Properties</span></span>

|<span data-ttu-id="88404-125">属性</span><span class="sxs-lookup"><span data-stu-id="88404-125">Property</span></span>|<span data-ttu-id="88404-126">类型</span><span class="sxs-lookup"><span data-stu-id="88404-126">Type</span></span>|<span data-ttu-id="88404-127">说明</span><span class="sxs-lookup"><span data-stu-id="88404-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88404-128">id</span><span class="sxs-lookup"><span data-stu-id="88404-128">id</span></span>|<span data-ttu-id="88404-129">字符串</span><span class="sxs-lookup"><span data-stu-id="88404-129">String</span></span>|<span data-ttu-id="88404-130">语言的标识符。</span><span class="sxs-lookup"><span data-stu-id="88404-130">The identifier of the language.</span></span> <span data-ttu-id="88404-131">此字段与语言 ID 标记 [RFC 5646](https://tools.ietf.org/html/rfc5646) 兼容，并且必须是记录的语言 ID。</span><span class="sxs-lookup"><span data-stu-id="88404-131">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span>|
|<span data-ttu-id="88404-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="88404-132">isEnabled</span></span>|<span data-ttu-id="88404-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="88404-133">Boolean</span></span>|<span data-ttu-id="88404-134">指示语言是否在用户流中启用。</span><span class="sxs-lookup"><span data-stu-id="88404-134">Indicates whether the language is enabled within the user flow.</span></span>|
|<span data-ttu-id="88404-135">displayName</span><span class="sxs-lookup"><span data-stu-id="88404-135">displayName</span></span>|<span data-ttu-id="88404-136">字符串</span><span class="sxs-lookup"><span data-stu-id="88404-136">String</span></span>|<span data-ttu-id="88404-137">要显示的语言名称。</span><span class="sxs-lookup"><span data-stu-id="88404-137">The language name to display.</span></span> <span data-ttu-id="88404-138">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="88404-138">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88404-139">关系</span><span class="sxs-lookup"><span data-stu-id="88404-139">Relationships</span></span>

|<span data-ttu-id="88404-140">关系</span><span class="sxs-lookup"><span data-stu-id="88404-140">Relationship</span></span>|<span data-ttu-id="88404-141">类型</span><span class="sxs-lookup"><span data-stu-id="88404-141">Type</span></span>|<span data-ttu-id="88404-142">描述</span><span class="sxs-lookup"><span data-stu-id="88404-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88404-143">defaultPages</span><span class="sxs-lookup"><span data-stu-id="88404-143">defaultPages</span></span>|<span data-ttu-id="88404-144">[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88404-144">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="88404-145">包含要以指定语言的用户流显示的默认内容的页面集合。</span><span class="sxs-lookup"><span data-stu-id="88404-145">Collection of pages with the default content to display in a user flow for a specified language.</span></span> <span data-ttu-id="88404-146">此集合不允许任何类型的修改。</span><span class="sxs-lookup"><span data-stu-id="88404-146">This collection does not allow any kind of modification.</span></span>|
|<span data-ttu-id="88404-147">overridesPages</span><span class="sxs-lookup"><span data-stu-id="88404-147">overridesPages</span></span>|<span data-ttu-id="88404-148">[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88404-148">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="88404-149">包含覆盖消息的页面集合，这些消息显示在指定语言的用户流中。</span><span class="sxs-lookup"><span data-stu-id="88404-149">Collection of pages with the overrides messages to display in a user flow for a specified language.</span></span> <span data-ttu-id="88404-150">此集合仅允许修改页面的内容，不允许在页面创建 (删除页面时进行任何其他) 。</span><span class="sxs-lookup"><span data-stu-id="88404-150">This collection only allows to modify the content of the page, any other modification is not allowed (creation or deletion of pages).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88404-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88404-151">JSON representation</span></span>

<span data-ttu-id="88404-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88404-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguageConfiguration",
  "id": "String (identifier)",
  "isEnabled": "Boolean",
  "displayName": "String"
}
```
