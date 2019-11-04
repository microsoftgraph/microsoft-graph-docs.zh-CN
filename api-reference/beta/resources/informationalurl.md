---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: c8cf7bcc40480042b4cd43230ca0245bd690fd7b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938840"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="6d631-103">informationalUrl 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d631-103">informationalUrl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d631-104">应用程序的基本配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="6d631-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="6d631-105">属性</span><span class="sxs-lookup"><span data-stu-id="6d631-105">Properties</span></span>

| <span data-ttu-id="6d631-106">属性</span><span class="sxs-lookup"><span data-stu-id="6d631-106">Property</span></span> | <span data-ttu-id="6d631-107">类型</span><span class="sxs-lookup"><span data-stu-id="6d631-107">Type</span></span> | <span data-ttu-id="6d631-108">描述</span><span class="sxs-lookup"><span data-stu-id="6d631-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6d631-109">logoUrl</span><span class="sxs-lookup"><span data-stu-id="6d631-109">logoUrl</span></span>|<span data-ttu-id="6d631-110">字符串</span><span class="sxs-lookup"><span data-stu-id="6d631-110">String</span></span>|<span data-ttu-id="6d631-111">指向应用程序徽标的 CDN URL，只读。</span><span class="sxs-lookup"><span data-stu-id="6d631-111">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="6d631-112">marketingUrl</span><span class="sxs-lookup"><span data-stu-id="6d631-112">marketingUrl</span></span>|<span data-ttu-id="6d631-113">字符串</span><span class="sxs-lookup"><span data-stu-id="6d631-113">String</span></span>| <span data-ttu-id="6d631-114">指向应用程序的市场营销页面的链接。</span><span class="sxs-lookup"><span data-stu-id="6d631-114">Link to the application's marketing page.</span></span> <span data-ttu-id="6d631-115">例如，https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="6d631-115">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="6d631-116">privacyStatementUrl</span><span class="sxs-lookup"><span data-stu-id="6d631-116">privacyStatementUrl</span></span>|<span data-ttu-id="6d631-117">字符串</span><span class="sxs-lookup"><span data-stu-id="6d631-117">String</span></span>| <span data-ttu-id="6d631-118">指向应用程序的隐私声明的链接。</span><span class="sxs-lookup"><span data-stu-id="6d631-118">Link to the application's privacy statement.</span></span> <span data-ttu-id="6d631-119">例如，https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="6d631-119">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="6d631-120">supportUrl</span><span class="sxs-lookup"><span data-stu-id="6d631-120">supportUrl</span></span>|<span data-ttu-id="6d631-121">字符串</span><span class="sxs-lookup"><span data-stu-id="6d631-121">String</span></span>| <span data-ttu-id="6d631-122">指向应用程序的支持页的链接。</span><span class="sxs-lookup"><span data-stu-id="6d631-122">Link to the application's support page.</span></span> <span data-ttu-id="6d631-123">例如，https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="6d631-123">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="6d631-124">termsOfServiceUrl</span><span class="sxs-lookup"><span data-stu-id="6d631-124">termsOfServiceUrl</span></span>|<span data-ttu-id="6d631-125">字符串</span><span class="sxs-lookup"><span data-stu-id="6d631-125">String</span></span>| <span data-ttu-id="6d631-126">指向应用程序的服务条款声明的链接。</span><span class="sxs-lookup"><span data-stu-id="6d631-126">Link to the application's terms of service statement.</span></span> <span data-ttu-id="6d631-127">例如，https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="6d631-127">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6d631-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d631-128">JSON representation</span></span>
<span data-ttu-id="6d631-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d631-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "logoUrl": "String",
  "marketingUrl": "String",
  "privacyStatementUrl": "String",
  "supportUrl": "String",
  "termsOfServiceUrl": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
