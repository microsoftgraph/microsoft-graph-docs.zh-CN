---
title: applicationTemplate 资源类型
description: 表示 Azure AD 应用程序库中的应用程序
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: dff7319444179dbe66698fa47691369ef3901340
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476423"
---
# <a name="applicationtemplate-resource-type"></a><span data-ttu-id="8f54b-103">applicationTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f54b-103">applicationTemplate resource type</span></span>

<span data-ttu-id="8f54b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f54b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f54b-105">表示 Azure [AD 应用程序库中的应用程序](/azure/active-directory/saas-apps/tutorial-list)。</span><span class="sxs-lookup"><span data-stu-id="8f54b-105">Represents an application in the [Azure AD application gallery](/azure/active-directory/saas-apps/tutorial-list).</span></span>

## <a name="methods"></a><span data-ttu-id="8f54b-106">Methods</span><span class="sxs-lookup"><span data-stu-id="8f54b-106">Methods</span></span>

| <span data-ttu-id="8f54b-107">方法</span><span class="sxs-lookup"><span data-stu-id="8f54b-107">Method</span></span>                                                                       | <span data-ttu-id="8f54b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8f54b-108">Return Type</span></span>                                                   | <span data-ttu-id="8f54b-109">说明</span><span class="sxs-lookup"><span data-stu-id="8f54b-109">Description</span></span>                                                                                  |
| :--------------------------------------------------------------------------- | :------------------------------------------------------------ | :------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="8f54b-110">列出 applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="8f54b-110">List applicationTemplate</span></span>](../api/applicationtemplate-list.md)               | [<span data-ttu-id="8f54b-111">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="8f54b-111">applicationTemplate</span></span>](applicationtemplate.md)                 | <span data-ttu-id="8f54b-112">检索 applicationTemplate 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8f54b-112">Retrieve a list of applicationTemplate objects.</span></span>                                              |
| [<span data-ttu-id="8f54b-113">获取 applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="8f54b-113">Get applicationTemplate</span></span>](../api/applicationtemplate-get.md)                 | [<span data-ttu-id="8f54b-114">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="8f54b-114">applicationTemplate</span></span>](applicationtemplate.md)                 | <span data-ttu-id="8f54b-115">读取 applicationTemplate 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8f54b-115">Read properties and relationships of applicationTemplate object.</span></span>                             |
| [<span data-ttu-id="8f54b-116">实例化 applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="8f54b-116">Instantiate applicationTemplate</span></span>](../api/applicationtemplate-instantiate.md) | [<span data-ttu-id="8f54b-117">applicationServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="8f54b-117">applicationServicePrincipal</span></span>](applicationserviceprincipal.md) | <span data-ttu-id="8f54b-118">将 Azure AD 应用程序库中的应用程序实例添加到目录中。</span><span class="sxs-lookup"><span data-stu-id="8f54b-118">Add an instance of an application from the Azure AD application gallery into your directory.</span></span> |

## <a name="properties"></a><span data-ttu-id="8f54b-119">属性</span><span class="sxs-lookup"><span data-stu-id="8f54b-119">Properties</span></span>

| <span data-ttu-id="8f54b-120">属性</span><span class="sxs-lookup"><span data-stu-id="8f54b-120">Property</span></span>                   | <span data-ttu-id="8f54b-121">类型</span><span class="sxs-lookup"><span data-stu-id="8f54b-121">Type</span></span>              | <span data-ttu-id="8f54b-122">说明</span><span class="sxs-lookup"><span data-stu-id="8f54b-122">Description</span></span>                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| :------------------------- | :---------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8f54b-123">categories</span><span class="sxs-lookup"><span data-stu-id="8f54b-123">categories</span></span>                 | <span data-ttu-id="8f54b-124">String collection</span><span class="sxs-lookup"><span data-stu-id="8f54b-124">String collection</span></span> | <span data-ttu-id="8f54b-125">应用程序的类别列表。</span><span class="sxs-lookup"><span data-stu-id="8f54b-125">The list of categories for the application.</span></span> <span data-ttu-id="8f54b-126">支持的值可以是： `Collaboration` ， `Business Management` ， ， ， ， ， ， ， ， ， `Consumer` ， `Content management` `CRM` `Data services` `Developer services` `E-commerce` `Education` `ERP` `Finance` `Health` `Human resources` `IT infrastructure` `Mail` `Management` `Marketing` `Media` `Productivity` `Project management` `Telecommunications` `Tools, Travel` `Web design & hosting` 。</span><span class="sxs-lookup"><span data-stu-id="8f54b-126">Supported values can be: `Collaboration`, `Business Management`, `Consumer`,`Content management`, `CRM`, `Data services`, `Developer services`, `E-commerce`, `Education`, `ERP`, `Finance`, `Health`, `Human resources`, `IT infrastructure`, `Mail`, `Management`, `Marketing`, `Media`, `Productivity`, `Project management`, `Telecommunications`, `Tools, Travel`, and `Web design & hosting`.</span></span> |
| <span data-ttu-id="8f54b-127">说明</span><span class="sxs-lookup"><span data-stu-id="8f54b-127">description</span></span>                | <span data-ttu-id="8f54b-128">String</span><span class="sxs-lookup"><span data-stu-id="8f54b-128">String</span></span>            | <span data-ttu-id="8f54b-129">应用程序的说明。</span><span class="sxs-lookup"><span data-stu-id="8f54b-129">A description of the application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                               |
| <span data-ttu-id="8f54b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="8f54b-130">displayName</span></span>                | <span data-ttu-id="8f54b-131">String</span><span class="sxs-lookup"><span data-stu-id="8f54b-131">String</span></span>            | <span data-ttu-id="8f54b-132">应用程序名。</span><span class="sxs-lookup"><span data-stu-id="8f54b-132">The name of the application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                                    |
| <span data-ttu-id="8f54b-133">homePageUrl</span><span class="sxs-lookup"><span data-stu-id="8f54b-133">homePageUrl</span></span>                | <span data-ttu-id="8f54b-134">String</span><span class="sxs-lookup"><span data-stu-id="8f54b-134">String</span></span>            | <span data-ttu-id="8f54b-135">应用程序的主页 URL。</span><span class="sxs-lookup"><span data-stu-id="8f54b-135">The home page URL of the application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                           |
| <span data-ttu-id="8f54b-136">id</span><span class="sxs-lookup"><span data-stu-id="8f54b-136">id</span></span>                         | <span data-ttu-id="8f54b-137">String</span><span class="sxs-lookup"><span data-stu-id="8f54b-137">String</span></span>            | <span data-ttu-id="8f54b-138">应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8f54b-138">Unique identifier for the application.</span></span> <span data-ttu-id="8f54b-139">只读。</span><span class="sxs-lookup"><span data-stu-id="8f54b-139">Read-only.</span></span>                                                                                                                                                                                                                                                                                                                                                                                               |
| <span data-ttu-id="8f54b-140">logoUrl</span><span class="sxs-lookup"><span data-stu-id="8f54b-140">logoUrl</span></span>                    | <span data-ttu-id="8f54b-141">String</span><span class="sxs-lookup"><span data-stu-id="8f54b-141">String</span></span>            | <span data-ttu-id="8f54b-142">获取此应用程序徽标的 URL。</span><span class="sxs-lookup"><span data-stu-id="8f54b-142">The URL to get the logo for this application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="8f54b-143">发布者</span><span class="sxs-lookup"><span data-stu-id="8f54b-143">publisher</span></span>                  | <span data-ttu-id="8f54b-144">String</span><span class="sxs-lookup"><span data-stu-id="8f54b-144">String</span></span>            | <span data-ttu-id="8f54b-145">此应用程序的发布者的名称。</span><span class="sxs-lookup"><span data-stu-id="8f54b-145">The name of the publisher for this application.</span></span>                                                                                                                                                                                                                                                                                                                                                                                                 |
| <span data-ttu-id="8f54b-146">supportedProvisioningTypes</span><span class="sxs-lookup"><span data-stu-id="8f54b-146">supportedProvisioningTypes</span></span> | <span data-ttu-id="8f54b-147">String collection</span><span class="sxs-lookup"><span data-stu-id="8f54b-147">String collection</span></span> | <span data-ttu-id="8f54b-148">此应用程序支持的预配模式列表。</span><span class="sxs-lookup"><span data-stu-id="8f54b-148">The list of provisioning modes supported by this application.</span></span> <span data-ttu-id="8f54b-149">唯一有效的值为 `sync` 。</span><span class="sxs-lookup"><span data-stu-id="8f54b-149">The only valid value is `sync`.</span></span>                                                                                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="8f54b-150">supportedSingleSignOnModes</span><span class="sxs-lookup"><span data-stu-id="8f54b-150">supportedSingleSignOnModes</span></span> | <span data-ttu-id="8f54b-151">String collection</span><span class="sxs-lookup"><span data-stu-id="8f54b-151">String collection</span></span> | <span data-ttu-id="8f54b-152">此应用程序支持的单一登录模式列表。</span><span class="sxs-lookup"><span data-stu-id="8f54b-152">The list of single sign-on modes supported by this application.</span></span> <span data-ttu-id="8f54b-153">支持的值是：`oidc`、`password`、`saml` 和 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="8f54b-153">The supported values are `oidc`, `password`, `saml`, and `notSupported`.</span></span>                                                                                                                                                                                                                                                                                                            |

## <a name="relationships"></a><span data-ttu-id="8f54b-154">关系</span><span class="sxs-lookup"><span data-stu-id="8f54b-154">Relationships</span></span>

<span data-ttu-id="8f54b-155">无。</span><span class="sxs-lookup"><span data-stu-id="8f54b-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f54b-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f54b-156">JSON representation</span></span>

<span data-ttu-id="8f54b-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f54b-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationTemplate",
  "keyProperty": "id"
}-->

```json
{
  "id": "id-value",
  "displayName": "displayName-value",
  "homePageUrl": "homePageUrl-value",
  "supportedSingleSignOnModes": ["supportedSingleSignOnModes-value"],
  "logoUrl": "logoUrl-value",
  "categories": ["categories-value"],
  "publisher": "publisher-value",
  "description": "description-value"
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
