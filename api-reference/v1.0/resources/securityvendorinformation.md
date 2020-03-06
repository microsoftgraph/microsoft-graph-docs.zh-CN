---
title: securityVendorInformation 资源类型
description: " subProvider = AppLocker）。"
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: bb2b67892f5c1bffbc9844a7d30b9b16ea9cdf6e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533758"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="32cfd-103">securityVendorInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="32cfd-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="32cfd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32cfd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32cfd-105">包含有关安全产品/服务供应商、提供程序和 subprovider 的详细信息（例如，供应商 = Microsoft; provider = Windows Defender ATP; subProvider = AppLocker）。</span><span class="sxs-lookup"><span data-stu-id="32cfd-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="32cfd-106">属性</span><span class="sxs-lookup"><span data-stu-id="32cfd-106">Properties</span></span>

| <span data-ttu-id="32cfd-107">属性</span><span class="sxs-lookup"><span data-stu-id="32cfd-107">Property</span></span>   | <span data-ttu-id="32cfd-108">类型</span><span class="sxs-lookup"><span data-stu-id="32cfd-108">Type</span></span>|<span data-ttu-id="32cfd-109">说明</span><span class="sxs-lookup"><span data-stu-id="32cfd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32cfd-110">provider</span><span class="sxs-lookup"><span data-stu-id="32cfd-110">provider</span></span> |<span data-ttu-id="32cfd-111">字符串</span><span class="sxs-lookup"><span data-stu-id="32cfd-111">String</span></span>|<span data-ttu-id="32cfd-112">特定提供商（产品/服务-非供应商公司）;例如，WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="32cfd-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="32cfd-113">providerVersion</span><span class="sxs-lookup"><span data-stu-id="32cfd-113">providerVersion</span></span>|<span data-ttu-id="32cfd-114">字符串</span><span class="sxs-lookup"><span data-stu-id="32cfd-114">String</span></span>|<span data-ttu-id="32cfd-115">提供程序或 subprovider 的版本（如果存在），它将生成警报。</span><span class="sxs-lookup"><span data-stu-id="32cfd-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="32cfd-116">*Required*</span><span class="sxs-lookup"><span data-stu-id="32cfd-116">*Required*</span></span>|
|<span data-ttu-id="32cfd-117">subProvider</span><span class="sxs-lookup"><span data-stu-id="32cfd-117">subProvider</span></span>|<span data-ttu-id="32cfd-118">字符串</span><span class="sxs-lookup"><span data-stu-id="32cfd-118">String</span></span>|<span data-ttu-id="32cfd-119">特定 subprovider （在聚合提供程序下）;例如，WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="32cfd-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="32cfd-120">提供</span><span class="sxs-lookup"><span data-stu-id="32cfd-120">vendor</span></span> |<span data-ttu-id="32cfd-121">字符串</span><span class="sxs-lookup"><span data-stu-id="32cfd-121">String</span></span>|<span data-ttu-id="32cfd-122">通知供应商的名称（例如，Microsoft、Dell、FireEye）。</span><span class="sxs-lookup"><span data-stu-id="32cfd-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="32cfd-123">*Required*</span><span class="sxs-lookup"><span data-stu-id="32cfd-123">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="32cfd-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32cfd-124">JSON representation</span></span>

<span data-ttu-id="32cfd-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32cfd-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
