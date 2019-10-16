---
title: securityVendorInformation 资源类型
description: " subProvider = AppLocker）。"
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d7af6e0903e3d178bacdd7c86b4a2cab04285171
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536095"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="85c84-103">securityVendorInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="85c84-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="85c84-104">包含有关安全产品/服务供应商、提供程序和 subprovider 的详细信息（例如，供应商 = Microsoft; provider = Windows Defender ATP; subProvider = AppLocker）。</span><span class="sxs-lookup"><span data-stu-id="85c84-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="85c84-105">属性</span><span class="sxs-lookup"><span data-stu-id="85c84-105">Properties</span></span>

| <span data-ttu-id="85c84-106">属性</span><span class="sxs-lookup"><span data-stu-id="85c84-106">Property</span></span>   | <span data-ttu-id="85c84-107">类型</span><span class="sxs-lookup"><span data-stu-id="85c84-107">Type</span></span>|<span data-ttu-id="85c84-108">说明</span><span class="sxs-lookup"><span data-stu-id="85c84-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85c84-109">provider</span><span class="sxs-lookup"><span data-stu-id="85c84-109">provider</span></span> |<span data-ttu-id="85c84-110">字符串</span><span class="sxs-lookup"><span data-stu-id="85c84-110">String</span></span>|<span data-ttu-id="85c84-111">特定提供商（产品/服务-非供应商公司）;例如，WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="85c84-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="85c84-112">providerVersion</span><span class="sxs-lookup"><span data-stu-id="85c84-112">providerVersion</span></span>|<span data-ttu-id="85c84-113">字符串</span><span class="sxs-lookup"><span data-stu-id="85c84-113">String</span></span>|<span data-ttu-id="85c84-114">提供程序或 subprovider 的版本（如果存在），它将生成警报。</span><span class="sxs-lookup"><span data-stu-id="85c84-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="85c84-115">*Required*</span><span class="sxs-lookup"><span data-stu-id="85c84-115">*Required*</span></span>|
|<span data-ttu-id="85c84-116">subProvider</span><span class="sxs-lookup"><span data-stu-id="85c84-116">subProvider</span></span>|<span data-ttu-id="85c84-117">字符串</span><span class="sxs-lookup"><span data-stu-id="85c84-117">String</span></span>|<span data-ttu-id="85c84-118">特定 subprovider （在聚合提供程序下）;例如，WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="85c84-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="85c84-119">提供</span><span class="sxs-lookup"><span data-stu-id="85c84-119">vendor</span></span> |<span data-ttu-id="85c84-120">字符串</span><span class="sxs-lookup"><span data-stu-id="85c84-120">String</span></span>|<span data-ttu-id="85c84-121">通知供应商的名称（例如，Microsoft、Dell、FireEye）。</span><span class="sxs-lookup"><span data-stu-id="85c84-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="85c84-122">*Required*</span><span class="sxs-lookup"><span data-stu-id="85c84-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="85c84-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85c84-123">JSON representation</span></span>

<span data-ttu-id="85c84-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85c84-124">The following is a JSON representation of the resource.</span></span>
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
