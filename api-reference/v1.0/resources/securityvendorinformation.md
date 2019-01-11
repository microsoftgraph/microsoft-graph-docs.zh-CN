---
title: securityVendorInformation 资源类型
description: " subProvider = AppLocker)。"
localization_priority: Normal
ms.openlocfilehash: e9d8551c085c05007388bf0c6e33143994c6969b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820144"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="ca12c-103">securityVendorInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca12c-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="ca12c-104">包含有关安全产品/服务供应商、 提供商和 subprovider 详细信息 (例如，供应商 = Microsoft; 提供程序 = Windows Defender ATP; subProvider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="ca12c-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="ca12c-105">属性</span><span class="sxs-lookup"><span data-stu-id="ca12c-105">Properties</span></span>

| <span data-ttu-id="ca12c-106">属性</span><span class="sxs-lookup"><span data-stu-id="ca12c-106">Property</span></span>   | <span data-ttu-id="ca12c-107">类型</span><span class="sxs-lookup"><span data-stu-id="ca12c-107">Type</span></span>|<span data-ttu-id="ca12c-108">Description</span><span class="sxs-lookup"><span data-stu-id="ca12c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca12c-109">提供程序</span><span class="sxs-lookup"><span data-stu-id="ca12c-109">provider</span></span> |<span data-ttu-id="ca12c-110">字符串</span><span class="sxs-lookup"><span data-stu-id="ca12c-110">String</span></span>|<span data-ttu-id="ca12c-111">特定提供程序 （产品/服务 — 不供应商公司）;例如，WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="ca12c-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="ca12c-112">providerVersion</span><span class="sxs-lookup"><span data-stu-id="ca12c-112">providerVersion</span></span>|<span data-ttu-id="ca12c-113">字符串</span><span class="sxs-lookup"><span data-stu-id="ca12c-113">String</span></span>|<span data-ttu-id="ca12c-114">提供程序或 subprovider，如果存在，生成警报的版本。</span><span class="sxs-lookup"><span data-stu-id="ca12c-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="ca12c-115">*Required*</span><span class="sxs-lookup"><span data-stu-id="ca12c-115">*Required*</span></span>|
|<span data-ttu-id="ca12c-116">subProvider</span><span class="sxs-lookup"><span data-stu-id="ca12c-116">subProvider</span></span>|<span data-ttu-id="ca12c-117">字符串</span><span class="sxs-lookup"><span data-stu-id="ca12c-117">String</span></span>|<span data-ttu-id="ca12c-118">特定 subprovider （下聚合提供程序）;例如，WindowsDefenderATP.SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="ca12c-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="ca12c-119">供应商</span><span class="sxs-lookup"><span data-stu-id="ca12c-119">vendor</span></span> |<span data-ttu-id="ca12c-120">字符串</span><span class="sxs-lookup"><span data-stu-id="ca12c-120">String</span></span>|<span data-ttu-id="ca12c-121">警报供应商 (例如，Microsoft，Dell FireEye) 的名称。</span><span class="sxs-lookup"><span data-stu-id="ca12c-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="ca12c-122">*Required*</span><span class="sxs-lookup"><span data-stu-id="ca12c-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ca12c-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca12c-123">JSON representation</span></span>

<span data-ttu-id="ca12c-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca12c-124">The folllowing is a JSON representation of the resource.</span></span>
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
