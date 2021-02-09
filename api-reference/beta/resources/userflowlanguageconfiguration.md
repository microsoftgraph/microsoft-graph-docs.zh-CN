---
title: userFlowLanguageConfiguration 资源类型
description: userFlowsLanguageConfiguration 对象允许用户流支持多种语言的自定义。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c9c963fcb7f22af34de92d0ad1c9a472974e346f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159792"
---
# <a name="userflowlanguageconfiguration-resource-type"></a><span data-ttu-id="d12bb-103">userFlowLanguageConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d12bb-103">userFlowLanguageConfiguration resource type</span></span>

<span data-ttu-id="d12bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d12bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d12bb-105">用户流语言自定义是允许给定用户流支持多种语言（从所有内置语言到自定义语言）的自定义的功能。</span><span class="sxs-lookup"><span data-stu-id="d12bb-105">User flows language customization is a feature that allows a given user flow to support customization of multiple languages, from all the built-in languages to a custom language.</span></span>

<span data-ttu-id="d12bb-106">对于 [Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-language-customization#supported-languages)用户流，可以利用内置语言或为当前未默认内置语言提供语言自定义。</span><span class="sxs-lookup"><span data-stu-id="d12bb-106">For [Azure Active Directory B2C user flows](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-language-customization#supported-languages), you can leverage the built-in languages or provide the language customizations for a language that is not currently built-in by default.</span></span> <span data-ttu-id="d12bb-107">对于 [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/external-identities/user-flow-customize-language)用户流，只能利用 Microsoft 提供的内置语言。</span><span class="sxs-lookup"><span data-stu-id="d12bb-107">For [Azure Active Directory user flows](https://docs.microsoft.com/azure/active-directory/external-identities/user-flow-customize-language), you can only leverage the built-in languages provided by Microsoft.</span></span> <span data-ttu-id="d12bb-108">Azure Active Directory B2C 和 Azure Active Directory 的用户流都支持在用户完成使用用户流配置的旅程时自定义向用户显示的语言和字符串。</span><span class="sxs-lookup"><span data-stu-id="d12bb-108">Both user flows for Azure Active Directory B2C and Azure Active Directory support customizing the language and strings shown to users as they go through the journeys you configure with your user flows.</span></span>

## <a name="methods"></a><span data-ttu-id="d12bb-109">方法</span><span class="sxs-lookup"><span data-stu-id="d12bb-109">Methods</span></span>

|<span data-ttu-id="d12bb-110">方法</span><span class="sxs-lookup"><span data-stu-id="d12bb-110">Method</span></span>|<span data-ttu-id="d12bb-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d12bb-111">Return type</span></span>|<span data-ttu-id="d12bb-112">说明</span><span class="sxs-lookup"><span data-stu-id="d12bb-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d12bb-113">获取 userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="d12bb-113">Get userFlowLanguageConfiguration</span></span>](../api/userflowlanguageconfiguration-get.md)|[<span data-ttu-id="d12bb-114">userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="d12bb-114">userFlowLanguageConfiguration</span></span>](../resources/userflowlanguageconfiguration.md)|<span data-ttu-id="d12bb-115">读取 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d12bb-115">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="d12bb-116">这些对象表示用户流中可用的语言。</span><span class="sxs-lookup"><span data-stu-id="d12bb-116">These objects represent a language available in a user flow.</span></span>|
|[<span data-ttu-id="d12bb-117">删除 userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="d12bb-117">Delete userFlowLanguageConfiguration</span></span>](../api/userflowlanguageconfiguration-delete.md)|<span data-ttu-id="d12bb-118">无</span><span class="sxs-lookup"><span data-stu-id="d12bb-118">None</span></span>|<span data-ttu-id="d12bb-119">删除自定义 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d12bb-119">Deletes a custom [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="d12bb-120">这些对象表示在用户流中可用的语言，并且只能从 Azure AD B2C 用户流中删除自定义语言。</span><span class="sxs-lookup"><span data-stu-id="d12bb-120">These objects represent a language available in a user flow and only a custom language can be deleted from an Azure AD B2C user flow.</span></span>|
|[<span data-ttu-id="d12bb-121">列出 defaultPages</span><span class="sxs-lookup"><span data-stu-id="d12bb-121">List defaultPages</span></span>](../api/userflowlanguageconfiguration-list-defaultpages.md)|<span data-ttu-id="d12bb-122">[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d12bb-122">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="d12bb-123">从 defaultPages 导航属性获取 userFlowLanguagePage 资源。</span><span class="sxs-lookup"><span data-stu-id="d12bb-123">Get the userFlowLanguagePage resources from the defaultPages navigation property.</span></span> <span data-ttu-id="d12bb-124">表示用户流中的默认用户旅程。</span><span class="sxs-lookup"><span data-stu-id="d12bb-124">Represents the default user journey in a user flow.</span></span>|
|[<span data-ttu-id="d12bb-125">List overridesPages</span><span class="sxs-lookup"><span data-stu-id="d12bb-125">List overridesPages</span></span>](../api/userflowlanguageconfiguration-list-overridespages.md)|<span data-ttu-id="d12bb-126">[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d12bb-126">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="d12bb-127">从 overridesPages 导航属性获取 userFlowLanguagePage 资源。</span><span class="sxs-lookup"><span data-stu-id="d12bb-127">Get the userFlowLanguagePage resources from the overridesPages navigation property.</span></span> <span data-ttu-id="d12bb-128">表示用户流中的用户旅程的自定义体验。</span><span class="sxs-lookup"><span data-stu-id="d12bb-128">Represents a custom experience for a user journey in a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="d12bb-129">属性</span><span class="sxs-lookup"><span data-stu-id="d12bb-129">Properties</span></span>

|<span data-ttu-id="d12bb-130">属性</span><span class="sxs-lookup"><span data-stu-id="d12bb-130">Property</span></span>|<span data-ttu-id="d12bb-131">类型</span><span class="sxs-lookup"><span data-stu-id="d12bb-131">Type</span></span>|<span data-ttu-id="d12bb-132">说明</span><span class="sxs-lookup"><span data-stu-id="d12bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d12bb-133">id</span><span class="sxs-lookup"><span data-stu-id="d12bb-133">id</span></span>|<span data-ttu-id="d12bb-134">String</span><span class="sxs-lookup"><span data-stu-id="d12bb-134">String</span></span>|<span data-ttu-id="d12bb-135">语言的标识符。</span><span class="sxs-lookup"><span data-stu-id="d12bb-135">The identifier of the language.</span></span> <span data-ttu-id="d12bb-136">此字段符合语言 ID 标记 [RFC 5646，](https://tools.ietf.org/html/rfc5646) 并且必须是记录的语言 ID。</span><span class="sxs-lookup"><span data-stu-id="d12bb-136">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span>|
|<span data-ttu-id="d12bb-137">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d12bb-137">isEnabled</span></span>|<span data-ttu-id="d12bb-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="d12bb-138">Boolean</span></span>|<span data-ttu-id="d12bb-139">指示语言是否在用户流中启用。</span><span class="sxs-lookup"><span data-stu-id="d12bb-139">Indicates whether the language is enabled within the user flow.</span></span>|
|<span data-ttu-id="d12bb-140">displayName</span><span class="sxs-lookup"><span data-stu-id="d12bb-140">displayName</span></span>|<span data-ttu-id="d12bb-141">String</span><span class="sxs-lookup"><span data-stu-id="d12bb-141">String</span></span>|<span data-ttu-id="d12bb-142">要显示的语言名称。</span><span class="sxs-lookup"><span data-stu-id="d12bb-142">The language name to display.</span></span> <span data-ttu-id="d12bb-143">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d12bb-143">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d12bb-144">关系</span><span class="sxs-lookup"><span data-stu-id="d12bb-144">Relationships</span></span>

|<span data-ttu-id="d12bb-145">关系</span><span class="sxs-lookup"><span data-stu-id="d12bb-145">Relationship</span></span>|<span data-ttu-id="d12bb-146">类型</span><span class="sxs-lookup"><span data-stu-id="d12bb-146">Type</span></span>|<span data-ttu-id="d12bb-147">说明</span><span class="sxs-lookup"><span data-stu-id="d12bb-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d12bb-148">defaultPages</span><span class="sxs-lookup"><span data-stu-id="d12bb-148">defaultPages</span></span>|<span data-ttu-id="d12bb-149">[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d12bb-149">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="d12bb-150">包含要以指定语言的用户流显示的默认内容的页的集合。</span><span class="sxs-lookup"><span data-stu-id="d12bb-150">Collection of pages with the default content to display in a user flow for a specified language.</span></span> <span data-ttu-id="d12bb-151">此集合不允许任何类型的修改。</span><span class="sxs-lookup"><span data-stu-id="d12bb-151">This collection does not allow any kind of modification.</span></span>|
|<span data-ttu-id="d12bb-152">overridesPages</span><span class="sxs-lookup"><span data-stu-id="d12bb-152">overridesPages</span></span>|<span data-ttu-id="d12bb-153">[userFlowLanguagePage](../resources/userflowlanguagepage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d12bb-153">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="d12bb-154">包含替代消息的页面集合，这些邮件显示在指定语言的用户流中。</span><span class="sxs-lookup"><span data-stu-id="d12bb-154">Collection of pages with the overrides messages to display in a user flow for a specified language.</span></span> <span data-ttu-id="d12bb-155">此集合仅允许修改页面内容，不允许任何其他修改 (或删除页面) 。</span><span class="sxs-lookup"><span data-stu-id="d12bb-155">This collection only allows to modify the content of the page, any other modification is not allowed (creation or deletion of pages).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d12bb-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d12bb-156">JSON representation</span></span>

<span data-ttu-id="d12bb-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d12bb-157">The following is a JSON representation of the resource.</span></span>
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
