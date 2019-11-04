---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: e81d8cc4a1ef25364727049269b420cf426eb0c8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939479"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="2b6f5-103">informationalUrl 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b6f5-103">informationalUrl resource type</span></span>

<span data-ttu-id="2b6f5-104">应用程序的基本配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="2b6f5-104">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="2b6f5-105">属性</span><span class="sxs-lookup"><span data-stu-id="2b6f5-105">Properties</span></span>

| <span data-ttu-id="2b6f5-106">属性</span><span class="sxs-lookup"><span data-stu-id="2b6f5-106">Property</span></span> | <span data-ttu-id="2b6f5-107">类型</span><span class="sxs-lookup"><span data-stu-id="2b6f5-107">Type</span></span> | <span data-ttu-id="2b6f5-108">描述</span><span class="sxs-lookup"><span data-stu-id="2b6f5-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2b6f5-109">logoUrl</span><span class="sxs-lookup"><span data-stu-id="2b6f5-109">logoUrl</span></span>|<span data-ttu-id="2b6f5-110">String</span><span class="sxs-lookup"><span data-stu-id="2b6f5-110">String</span></span>|<span data-ttu-id="2b6f5-111">指向应用程序徽标的 CDN URL，只读。</span><span class="sxs-lookup"><span data-stu-id="2b6f5-111">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="2b6f5-112">marketingUrl</span><span class="sxs-lookup"><span data-stu-id="2b6f5-112">marketingUrl</span></span>|<span data-ttu-id="2b6f5-113">String</span><span class="sxs-lookup"><span data-stu-id="2b6f5-113">String</span></span>| <span data-ttu-id="2b6f5-114">指向应用程序的市场营销页面的链接。</span><span class="sxs-lookup"><span data-stu-id="2b6f5-114">Link to the application's marketing page.</span></span> <span data-ttu-id="2b6f5-115">例如，https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="2b6f5-115">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="2b6f5-116">privacyStatementUrl</span><span class="sxs-lookup"><span data-stu-id="2b6f5-116">privacyStatementUrl</span></span>|<span data-ttu-id="2b6f5-117">String</span><span class="sxs-lookup"><span data-stu-id="2b6f5-117">String</span></span>| <span data-ttu-id="2b6f5-118">指向应用程序的隐私声明的链接。</span><span class="sxs-lookup"><span data-stu-id="2b6f5-118">Link to the application's privacy statement.</span></span> <span data-ttu-id="2b6f5-119">例如，https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="2b6f5-119">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="2b6f5-120">supportUrl</span><span class="sxs-lookup"><span data-stu-id="2b6f5-120">supportUrl</span></span>|<span data-ttu-id="2b6f5-121">String</span><span class="sxs-lookup"><span data-stu-id="2b6f5-121">String</span></span>| <span data-ttu-id="2b6f5-122">指向应用程序的支持页的链接。</span><span class="sxs-lookup"><span data-stu-id="2b6f5-122">Link to the application's support page.</span></span> <span data-ttu-id="2b6f5-123">例如，https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="2b6f5-123">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="2b6f5-124">termsOfServiceUrl</span><span class="sxs-lookup"><span data-stu-id="2b6f5-124">termsOfServiceUrl</span></span>|<span data-ttu-id="2b6f5-125">String</span><span class="sxs-lookup"><span data-stu-id="2b6f5-125">String</span></span>| <span data-ttu-id="2b6f5-126">指向应用程序的服务条款声明的链接。</span><span class="sxs-lookup"><span data-stu-id="2b6f5-126">Link to the application's terms of service statement.</span></span> <span data-ttu-id="2b6f5-127">例如，https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="2b6f5-127">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2b6f5-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b6f5-128">JSON representation</span></span>
<span data-ttu-id="2b6f5-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b6f5-129">Here is a JSON representation of the resource.</span></span>

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
