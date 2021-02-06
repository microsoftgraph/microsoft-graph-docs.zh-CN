---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: d17ce96d1f714845d07bee3505a28d5a4e7e3978
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130239"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="3b025-103">informationalUrl 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b025-103">informationalUrl resource type</span></span>

<span data-ttu-id="3b025-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b025-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b025-105">应用程序的基本配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="3b025-105">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="3b025-106">属性</span><span class="sxs-lookup"><span data-stu-id="3b025-106">Properties</span></span>

| <span data-ttu-id="3b025-107">属性</span><span class="sxs-lookup"><span data-stu-id="3b025-107">Property</span></span> | <span data-ttu-id="3b025-108">类型</span><span class="sxs-lookup"><span data-stu-id="3b025-108">Type</span></span> | <span data-ttu-id="3b025-109">说明</span><span class="sxs-lookup"><span data-stu-id="3b025-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3b025-110">logoUrl</span><span class="sxs-lookup"><span data-stu-id="3b025-110">logoUrl</span></span>|<span data-ttu-id="3b025-111">字符串</span><span class="sxs-lookup"><span data-stu-id="3b025-111">String</span></span>|<span data-ttu-id="3b025-112">应用程序徽标的 CDN URL，只读。</span><span class="sxs-lookup"><span data-stu-id="3b025-112">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="3b025-113">marketingUrl</span><span class="sxs-lookup"><span data-stu-id="3b025-113">marketingUrl</span></span>|<span data-ttu-id="3b025-114">字符串</span><span class="sxs-lookup"><span data-stu-id="3b025-114">String</span></span>| <span data-ttu-id="3b025-115">指向应用程序的营销页面的链接。</span><span class="sxs-lookup"><span data-stu-id="3b025-115">Link to the application's marketing page.</span></span> <span data-ttu-id="3b025-116">例如，https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="3b025-116">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="3b025-117">privacyStatementUrl</span><span class="sxs-lookup"><span data-stu-id="3b025-117">privacyStatementUrl</span></span>|<span data-ttu-id="3b025-118">字符串</span><span class="sxs-lookup"><span data-stu-id="3b025-118">String</span></span>| <span data-ttu-id="3b025-119">指向应用程序隐私声明的链接。</span><span class="sxs-lookup"><span data-stu-id="3b025-119">Link to the application's privacy statement.</span></span> <span data-ttu-id="3b025-120">例如，https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="3b025-120">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="3b025-121">supportUrl</span><span class="sxs-lookup"><span data-stu-id="3b025-121">supportUrl</span></span>|<span data-ttu-id="3b025-122">字符串</span><span class="sxs-lookup"><span data-stu-id="3b025-122">String</span></span>| <span data-ttu-id="3b025-123">指向应用程序的支持页的链接。</span><span class="sxs-lookup"><span data-stu-id="3b025-123">Link to the application's support page.</span></span> <span data-ttu-id="3b025-124">例如，https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="3b025-124">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="3b025-125">termsOfServiceUrl</span><span class="sxs-lookup"><span data-stu-id="3b025-125">termsOfServiceUrl</span></span>|<span data-ttu-id="3b025-126">字符串</span><span class="sxs-lookup"><span data-stu-id="3b025-126">String</span></span>| <span data-ttu-id="3b025-127">指向应用程序的服务声明条款的链接。</span><span class="sxs-lookup"><span data-stu-id="3b025-127">Link to the application's terms of service statement.</span></span> <span data-ttu-id="3b025-128">例如，https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="3b025-128">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3b025-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b025-129">JSON representation</span></span>
<span data-ttu-id="3b025-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b025-130">Here is a JSON representation of the resource.</span></span>

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


