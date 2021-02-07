---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: d249c150870a3a7149b92ad7aab55a84c23896dd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132102"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="87481-103">informationalUrl 资源类型</span><span class="sxs-lookup"><span data-stu-id="87481-103">informationalUrl resource type</span></span>

<span data-ttu-id="87481-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87481-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="87481-105">应用程序的基本配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="87481-105">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="87481-106">属性</span><span class="sxs-lookup"><span data-stu-id="87481-106">Properties</span></span>

| <span data-ttu-id="87481-107">属性</span><span class="sxs-lookup"><span data-stu-id="87481-107">Property</span></span> | <span data-ttu-id="87481-108">类型</span><span class="sxs-lookup"><span data-stu-id="87481-108">Type</span></span> | <span data-ttu-id="87481-109">说明</span><span class="sxs-lookup"><span data-stu-id="87481-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="87481-110">logoUrl</span><span class="sxs-lookup"><span data-stu-id="87481-110">logoUrl</span></span>|<span data-ttu-id="87481-111">String</span><span class="sxs-lookup"><span data-stu-id="87481-111">String</span></span>|<span data-ttu-id="87481-112">应用程序徽标的 CDN URL，只读。</span><span class="sxs-lookup"><span data-stu-id="87481-112">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="87481-113">marketingUrl</span><span class="sxs-lookup"><span data-stu-id="87481-113">marketingUrl</span></span>|<span data-ttu-id="87481-114">String</span><span class="sxs-lookup"><span data-stu-id="87481-114">String</span></span>| <span data-ttu-id="87481-115">指向应用程序的营销页面的链接。</span><span class="sxs-lookup"><span data-stu-id="87481-115">Link to the application's marketing page.</span></span> <span data-ttu-id="87481-116">例如，https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="87481-116">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="87481-117">privacyStatementUrl</span><span class="sxs-lookup"><span data-stu-id="87481-117">privacyStatementUrl</span></span>|<span data-ttu-id="87481-118">String</span><span class="sxs-lookup"><span data-stu-id="87481-118">String</span></span>| <span data-ttu-id="87481-119">指向应用程序隐私声明的链接。</span><span class="sxs-lookup"><span data-stu-id="87481-119">Link to the application's privacy statement.</span></span> <span data-ttu-id="87481-120">例如，https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="87481-120">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="87481-121">supportUrl</span><span class="sxs-lookup"><span data-stu-id="87481-121">supportUrl</span></span>|<span data-ttu-id="87481-122">String</span><span class="sxs-lookup"><span data-stu-id="87481-122">String</span></span>| <span data-ttu-id="87481-123">指向应用程序的支持页的链接。</span><span class="sxs-lookup"><span data-stu-id="87481-123">Link to the application's support page.</span></span> <span data-ttu-id="87481-124">例如，https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="87481-124">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="87481-125">termsOfServiceUrl</span><span class="sxs-lookup"><span data-stu-id="87481-125">termsOfServiceUrl</span></span>|<span data-ttu-id="87481-126">String</span><span class="sxs-lookup"><span data-stu-id="87481-126">String</span></span>| <span data-ttu-id="87481-127">指向应用程序的服务声明条款的链接。</span><span class="sxs-lookup"><span data-stu-id="87481-127">Link to the application's terms of service statement.</span></span> <span data-ttu-id="87481-128">例如，https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="87481-128">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="87481-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87481-129">JSON representation</span></span>
<span data-ttu-id="87481-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87481-130">Here is a JSON representation of the resource.</span></span>

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

