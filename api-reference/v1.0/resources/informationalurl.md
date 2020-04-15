---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: d783a8c4ad833be0b6dabf9b9405256796b880b7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43397442"
---
# <a name="informationalurl-resource-type"></a><span data-ttu-id="d3475-103">informationalUrl 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3475-103">informationalUrl resource type</span></span>

<span data-ttu-id="d3475-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3475-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3475-105">应用程序的基本配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="d3475-105">Basic profile information of the application.</span></span>

## <a name="properties"></a><span data-ttu-id="d3475-106">属性</span><span class="sxs-lookup"><span data-stu-id="d3475-106">Properties</span></span>

| <span data-ttu-id="d3475-107">属性</span><span class="sxs-lookup"><span data-stu-id="d3475-107">Property</span></span> | <span data-ttu-id="d3475-108">类型</span><span class="sxs-lookup"><span data-stu-id="d3475-108">Type</span></span> | <span data-ttu-id="d3475-109">说明</span><span class="sxs-lookup"><span data-stu-id="d3475-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d3475-110">logoUrl</span><span class="sxs-lookup"><span data-stu-id="d3475-110">logoUrl</span></span>|<span data-ttu-id="d3475-111">String</span><span class="sxs-lookup"><span data-stu-id="d3475-111">String</span></span>|<span data-ttu-id="d3475-112">指向应用程序徽标的 CDN URL，只读。</span><span class="sxs-lookup"><span data-stu-id="d3475-112">CDN URL to the application's logo, Read-only.</span></span>|
|<span data-ttu-id="d3475-113">marketingUrl</span><span class="sxs-lookup"><span data-stu-id="d3475-113">marketingUrl</span></span>|<span data-ttu-id="d3475-114">String</span><span class="sxs-lookup"><span data-stu-id="d3475-114">String</span></span>| <span data-ttu-id="d3475-115">指向应用程序的市场营销页面的链接。</span><span class="sxs-lookup"><span data-stu-id="d3475-115">Link to the application's marketing page.</span></span> <span data-ttu-id="d3475-116">例如，https://www.contoso.com/app/marketing</span><span class="sxs-lookup"><span data-stu-id="d3475-116">For example, https://www.contoso.com/app/marketing</span></span> |
|<span data-ttu-id="d3475-117">privacyStatementUrl</span><span class="sxs-lookup"><span data-stu-id="d3475-117">privacyStatementUrl</span></span>|<span data-ttu-id="d3475-118">String</span><span class="sxs-lookup"><span data-stu-id="d3475-118">String</span></span>| <span data-ttu-id="d3475-119">指向应用程序的隐私声明的链接。</span><span class="sxs-lookup"><span data-stu-id="d3475-119">Link to the application's privacy statement.</span></span> <span data-ttu-id="d3475-120">例如，https://www.contoso.com/app/privacy</span><span class="sxs-lookup"><span data-stu-id="d3475-120">For example, https://www.contoso.com/app/privacy</span></span> |
|<span data-ttu-id="d3475-121">supportUrl</span><span class="sxs-lookup"><span data-stu-id="d3475-121">supportUrl</span></span>|<span data-ttu-id="d3475-122">String</span><span class="sxs-lookup"><span data-stu-id="d3475-122">String</span></span>| <span data-ttu-id="d3475-123">指向应用程序的支持页的链接。</span><span class="sxs-lookup"><span data-stu-id="d3475-123">Link to the application's support page.</span></span> <span data-ttu-id="d3475-124">例如，https://www.contoso.com/app/support</span><span class="sxs-lookup"><span data-stu-id="d3475-124">For example, https://www.contoso.com/app/support</span></span> |
|<span data-ttu-id="d3475-125">termsOfServiceUrl</span><span class="sxs-lookup"><span data-stu-id="d3475-125">termsOfServiceUrl</span></span>|<span data-ttu-id="d3475-126">String</span><span class="sxs-lookup"><span data-stu-id="d3475-126">String</span></span>| <span data-ttu-id="d3475-127">指向应用程序的服务条款声明的链接。</span><span class="sxs-lookup"><span data-stu-id="d3475-127">Link to the application's terms of service statement.</span></span> <span data-ttu-id="d3475-128">例如，https://www.contoso.com/app/termsofservice</span><span class="sxs-lookup"><span data-stu-id="d3475-128">For example, https://www.contoso.com/app/termsofservice</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d3475-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3475-129">JSON representation</span></span>
<span data-ttu-id="d3475-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3475-130">Here is a JSON representation of the resource.</span></span>

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
