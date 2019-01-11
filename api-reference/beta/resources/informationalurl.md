---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
ms.openlocfilehash: 78fd03a2673b342d1a0c904f521fe5a0f8cba205
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816980"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="d5c61-103">informationalUrl 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5c61-103">informationalUrl resource type</span></span>

> <span data-ttu-id="d5c61-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d5c61-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5c61-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d5c61-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d5c61-106">应用程序的基本配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="d5c61-106">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="d5c61-107">属性</span><span class="sxs-lookup"><span data-stu-id="d5c61-107">Properties</span></span>

| <span data-ttu-id="d5c61-108">属性</span><span class="sxs-lookup"><span data-stu-id="d5c61-108">Property</span></span> | <span data-ttu-id="d5c61-109">类型</span><span class="sxs-lookup"><span data-stu-id="d5c61-109">Type</span></span> | <span data-ttu-id="d5c61-110">Description</span><span class="sxs-lookup"><span data-stu-id="d5c61-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d5c61-111">市场营销</span><span class="sxs-lookup"><span data-stu-id="d5c61-111">marketing</span></span>|<span data-ttu-id="d5c61-112">字符串</span><span class="sxs-lookup"><span data-stu-id="d5c61-112">String</span></span>| <span data-ttu-id="d5c61-113">链接到应用程序的市场营销页。</span><span class="sxs-lookup"><span data-stu-id="d5c61-113">Link to the application's marketing page.</span></span> <span data-ttu-id="d5c61-114">例如，https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="d5c61-114">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="d5c61-115">隐私</span><span class="sxs-lookup"><span data-stu-id="d5c61-115">privacy</span></span>|<span data-ttu-id="d5c61-116">字符串</span><span class="sxs-lookup"><span data-stu-id="d5c61-116">String</span></span>| <span data-ttu-id="d5c61-117">链接到应用程序的隐私声明。</span><span class="sxs-lookup"><span data-stu-id="d5c61-117">Link to the application's privacy statement.</span></span> <span data-ttu-id="d5c61-118">例如，https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="d5c61-118">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="d5c61-119">支持</span><span class="sxs-lookup"><span data-stu-id="d5c61-119">support</span></span>|<span data-ttu-id="d5c61-120">字符串</span><span class="sxs-lookup"><span data-stu-id="d5c61-120">String</span></span>| <span data-ttu-id="d5c61-121">链接到应用程序的支持网页。</span><span class="sxs-lookup"><span data-stu-id="d5c61-121">Link to the application's support page.</span></span> <span data-ttu-id="d5c61-122">例如，https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="d5c61-122">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="d5c61-123">termsOfService</span><span class="sxs-lookup"><span data-stu-id="d5c61-123">termsOfService</span></span>|<span data-ttu-id="d5c61-124">字符串</span><span class="sxs-lookup"><span data-stu-id="d5c61-124">String</span></span>| <span data-ttu-id="d5c61-125">链接到的服务语句的应用程序的术语。</span><span class="sxs-lookup"><span data-stu-id="d5c61-125">Link to the application's terms of service statement.</span></span> <span data-ttu-id="d5c61-126">例如，https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="d5c61-126">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d5c61-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5c61-127">JSON representation</span></span>
<span data-ttu-id="d5c61-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5c61-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "marketing": "String",
  "privacy": "String",
  "support": "String",
  "termsOfService": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
