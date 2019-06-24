---
title: applicationTemplate 资源类型
description: 表示 Azure AD 应用程序库中的应用程序
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a8e1f4cb365f86df32e32ed568aa3a96d1c090f
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147897"
---
# <a name="applicationtemplate-resource-type"></a><span data-ttu-id="18d2b-103">applicationTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="18d2b-103">applicationTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18d2b-104">表示[AZURE AD 应用程序库](https://docs.microsoft.com/en-us/azure/active-directory/saas-apps/tutorial-list)中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="18d2b-104">Represents an application in the [Azure AD application gallery](https://docs.microsoft.com/en-us/azure/active-directory/saas-apps/tutorial-list).</span></span>

## <a name="methods"></a><span data-ttu-id="18d2b-105">方法</span><span class="sxs-lookup"><span data-stu-id="18d2b-105">Methods</span></span>

| <span data-ttu-id="18d2b-106">方法</span><span class="sxs-lookup"><span data-stu-id="18d2b-106">Method</span></span>       | <span data-ttu-id="18d2b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="18d2b-107">Return Type</span></span> | <span data-ttu-id="18d2b-108">说明</span><span class="sxs-lookup"><span data-stu-id="18d2b-108">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="18d2b-109">列出 applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="18d2b-109">List applicationTemplate</span></span>](../api/applicationtemplate-list.md)|[<span data-ttu-id="18d2b-110">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="18d2b-110">applicationTemplate</span></span>](applicationtemplate.md)|<span data-ttu-id="18d2b-111">检索 applicationTemplate 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="18d2b-111">Retrieve a list of applicationTemplate objects.</span></span>|
| [<span data-ttu-id="18d2b-112">获取 applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="18d2b-112">Get applicationTemplate</span></span>](../api/applicationtemplate-get.md) | [<span data-ttu-id="18d2b-113">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="18d2b-113">applicationTemplate</span></span>](applicationtemplate.md) | <span data-ttu-id="18d2b-114">读取 applicationTemplate 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="18d2b-114">Read properties and relationships of applicationTemplate object.</span></span> |
|[<span data-ttu-id="18d2b-115">实例化 applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="18d2b-115">Instantiate applicationTemplate</span></span>](../api/applicationtemplate-instantiate.md)|[<span data-ttu-id="18d2b-116">applicationServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="18d2b-116">applicationServicePrincipal</span></span>](applicationserviceprincipal.md)| <span data-ttu-id="18d2b-117">将 Azure AD 应用程序库中的应用程序实例添加到目录中。</span><span class="sxs-lookup"><span data-stu-id="18d2b-117">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>|


## <a name="properties"></a><span data-ttu-id="18d2b-118">属性</span><span class="sxs-lookup"><span data-stu-id="18d2b-118">Properties</span></span>

| <span data-ttu-id="18d2b-119">属性</span><span class="sxs-lookup"><span data-stu-id="18d2b-119">Property</span></span>     | <span data-ttu-id="18d2b-120">类型</span><span class="sxs-lookup"><span data-stu-id="18d2b-120">Type</span></span>        | <span data-ttu-id="18d2b-121">说明</span><span class="sxs-lookup"><span data-stu-id="18d2b-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="18d2b-122">categories</span><span class="sxs-lookup"><span data-stu-id="18d2b-122">categories</span></span>|<span data-ttu-id="18d2b-123">String collection</span><span class="sxs-lookup"><span data-stu-id="18d2b-123">String collection</span></span>|<span data-ttu-id="18d2b-124">应用程序的类别列表。</span><span class="sxs-lookup"><span data-stu-id="18d2b-124">The list of categories for the application.</span></span> <span data-ttu-id="18d2b-125">受支持的值可以`Collaboration`是`Business Management`: `Consumer`、`Content management`、 `CRM` `Data services` `Developer services` `E-commerce` `Education` `ERP` `Finance` `Health` `Human resources` `IT infrastructure`、、、、、、、、、、、、、、、、 `Mail` `Management` `Marketing` `Media` `Productivity`、 `Project management`、 `Telecommunications` `Tools, Travel`、和`Web design & hosting`。</span><span class="sxs-lookup"><span data-stu-id="18d2b-125">Supported values can be: `Collaboration`, `Business Management`, `Consumer`,`Content management`, `CRM`, `Data services`, `Developer services`, `E-commerce`, `Education`, `ERP`, `Finance`, `Health`, `Human resources`, `IT infrastructure`, `Mail`, `Management`, `Marketing`, `Media`, `Productivity`, `Project management`, `Telecommunications`, `Tools, Travel`, and `Web design & hosting`.</span></span>|
|<span data-ttu-id="18d2b-126">说明</span><span class="sxs-lookup"><span data-stu-id="18d2b-126">description</span></span>|<span data-ttu-id="18d2b-127">String</span><span class="sxs-lookup"><span data-stu-id="18d2b-127">String</span></span>|<span data-ttu-id="18d2b-128">应用程序的说明。</span><span class="sxs-lookup"><span data-stu-id="18d2b-128">A description of the application.</span></span>|
|<span data-ttu-id="18d2b-129">displayName</span><span class="sxs-lookup"><span data-stu-id="18d2b-129">displayName</span></span>|<span data-ttu-id="18d2b-130">字符串</span><span class="sxs-lookup"><span data-stu-id="18d2b-130">String</span></span>|<span data-ttu-id="18d2b-131">应用程序名。</span><span class="sxs-lookup"><span data-stu-id="18d2b-131">The name of the application.</span></span>|
|<span data-ttu-id="18d2b-132">homePageUrl</span><span class="sxs-lookup"><span data-stu-id="18d2b-132">homePageUrl</span></span>|<span data-ttu-id="18d2b-133">String</span><span class="sxs-lookup"><span data-stu-id="18d2b-133">String</span></span>|<span data-ttu-id="18d2b-134">应用程序的主页 URL。</span><span class="sxs-lookup"><span data-stu-id="18d2b-134">The home page URL of the application.</span></span>|
|<span data-ttu-id="18d2b-135">id</span><span class="sxs-lookup"><span data-stu-id="18d2b-135">id</span></span>|<span data-ttu-id="18d2b-136">字符串</span><span class="sxs-lookup"><span data-stu-id="18d2b-136">String</span></span>| <span data-ttu-id="18d2b-137">应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="18d2b-137">Unique identifier for the application.</span></span> <span data-ttu-id="18d2b-138">只读。</span><span class="sxs-lookup"><span data-stu-id="18d2b-138">Read-only.</span></span>|
|<span data-ttu-id="18d2b-139">logoUrl</span><span class="sxs-lookup"><span data-stu-id="18d2b-139">logoUrl</span></span>|<span data-ttu-id="18d2b-140">String</span><span class="sxs-lookup"><span data-stu-id="18d2b-140">String</span></span>|<span data-ttu-id="18d2b-141">用于获取此应用程序徽标的 URL。</span><span class="sxs-lookup"><span data-stu-id="18d2b-141">The URL to get the logo for this application.</span></span>|
|<span data-ttu-id="18d2b-142">发布者</span><span class="sxs-lookup"><span data-stu-id="18d2b-142">publisher</span></span>|<span data-ttu-id="18d2b-143">String</span><span class="sxs-lookup"><span data-stu-id="18d2b-143">String</span></span>|<span data-ttu-id="18d2b-144">此应用程序的发布者的名称。</span><span class="sxs-lookup"><span data-stu-id="18d2b-144">The name of the publisher for this application.</span></span>|
|<span data-ttu-id="18d2b-145">supportedProvisioningTypes</span><span class="sxs-lookup"><span data-stu-id="18d2b-145">supportedProvisioningTypes</span></span>|<span data-ttu-id="18d2b-146">String collection</span><span class="sxs-lookup"><span data-stu-id="18d2b-146">String collection</span></span>|<span data-ttu-id="18d2b-147">此应用程序支持的预配模式的列表。</span><span class="sxs-lookup"><span data-stu-id="18d2b-147">The list of provisioning modes supported by this application.</span></span> <span data-ttu-id="18d2b-148">唯一有效的值为`sync`。</span><span class="sxs-lookup"><span data-stu-id="18d2b-148">The only valid value is `sync`.</span></span>|
|<span data-ttu-id="18d2b-149">supportedSingleSignOnModes</span><span class="sxs-lookup"><span data-stu-id="18d2b-149">supportedSingleSignOnModes</span></span>|<span data-ttu-id="18d2b-150">String collection</span><span class="sxs-lookup"><span data-stu-id="18d2b-150">String collection</span></span>|<span data-ttu-id="18d2b-151">此应用程序支持的单一登录模式列表。</span><span class="sxs-lookup"><span data-stu-id="18d2b-151">The list of single sign-on modes supported by this application.</span></span> <span data-ttu-id="18d2b-152">受支持的值`password`为`saml`、 `external`、和`oidc`。</span><span class="sxs-lookup"><span data-stu-id="18d2b-152">The supported values are `password`, `saml`, `external`, and `oidc`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18d2b-153">关系</span><span class="sxs-lookup"><span data-stu-id="18d2b-153">Relationships</span></span>

<span data-ttu-id="18d2b-154">无。</span><span class="sxs-lookup"><span data-stu-id="18d2b-154">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="18d2b-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18d2b-155">JSON representation</span></span>

<span data-ttu-id="18d2b-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18d2b-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
