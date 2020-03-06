---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: ebf2a79931936e8f45f93cba46b1fefdbf0163b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532885"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="fea51-103">informationalUrl 资源类型</span><span class="sxs-lookup"><span data-stu-id="fea51-103">informationalUrl resource type</span></span>

<span data-ttu-id="fea51-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fea51-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fea51-105">应用程序的基本配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="fea51-105">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="fea51-106">属性</span><span class="sxs-lookup"><span data-stu-id="fea51-106">Properties</span></span>

| <span data-ttu-id="fea51-107">属性</span><span class="sxs-lookup"><span data-stu-id="fea51-107">Property</span></span> | <span data-ttu-id="fea51-108">类型</span><span class="sxs-lookup"><span data-stu-id="fea51-108">Type</span></span> | <span data-ttu-id="fea51-109">说明</span><span class="sxs-lookup"><span data-stu-id="fea51-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fea51-110">logoUrl</span><span class="sxs-lookup"><span data-stu-id="fea51-110">logoUrl</span></span>|<span data-ttu-id="fea51-111">字符串</span><span class="sxs-lookup"><span data-stu-id="fea51-111">String</span></span>|<span data-ttu-id="fea51-112">指向应用程序徽标的 CDN URL，只读。</span><span class="sxs-lookup"><span data-stu-id="fea51-112">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="fea51-113">marketingUrl</span><span class="sxs-lookup"><span data-stu-id="fea51-113">marketingUrl</span></span>|<span data-ttu-id="fea51-114">字符串</span><span class="sxs-lookup"><span data-stu-id="fea51-114">String</span></span>| <span data-ttu-id="fea51-115">指向应用程序的市场营销页面的链接。</span><span class="sxs-lookup"><span data-stu-id="fea51-115">Link to the application's marketing page.</span></span> <span data-ttu-id="fea51-116">例如，https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="fea51-116">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="fea51-117">privacyStatementUrl</span><span class="sxs-lookup"><span data-stu-id="fea51-117">privacyStatementUrl</span></span>|<span data-ttu-id="fea51-118">字符串</span><span class="sxs-lookup"><span data-stu-id="fea51-118">String</span></span>| <span data-ttu-id="fea51-119">指向应用程序的隐私声明的链接。</span><span class="sxs-lookup"><span data-stu-id="fea51-119">Link to the application's privacy statement.</span></span> <span data-ttu-id="fea51-120">例如，https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="fea51-120">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="fea51-121">supportUrl</span><span class="sxs-lookup"><span data-stu-id="fea51-121">supportUrl</span></span>|<span data-ttu-id="fea51-122">字符串</span><span class="sxs-lookup"><span data-stu-id="fea51-122">String</span></span>| <span data-ttu-id="fea51-123">指向应用程序的支持页的链接。</span><span class="sxs-lookup"><span data-stu-id="fea51-123">Link to the application's support page.</span></span> <span data-ttu-id="fea51-124">例如，https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="fea51-124">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="fea51-125">termsOfServiceUrl</span><span class="sxs-lookup"><span data-stu-id="fea51-125">termsOfServiceUrl</span></span>|<span data-ttu-id="fea51-126">字符串</span><span class="sxs-lookup"><span data-stu-id="fea51-126">String</span></span>| <span data-ttu-id="fea51-127">指向应用程序的服务条款声明的链接。</span><span class="sxs-lookup"><span data-stu-id="fea51-127">Link to the application's terms of service statement.</span></span> <span data-ttu-id="fea51-128">例如，https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="fea51-128">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fea51-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fea51-129">JSON representation</span></span>
<span data-ttu-id="fea51-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fea51-130">Here is a JSON representation of the resource.</span></span>

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
