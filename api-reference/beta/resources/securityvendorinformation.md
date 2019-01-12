---
title: securityVendorInformation 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 0137abd7a9df0df94f73e18d7efa201008031ff6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939922"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="d98cf-104">securityVendorInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d98cf-104">securityVendorInformation resource type</span></span>

 > <span data-ttu-id="d98cf-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d98cf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d98cf-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d98cf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d98cf-107">包含有关安全产品/服务供应商、 提供商和 subprovider 详细信息 (例如，供应商 = Microsoft; 提供程序 = Windows Defender ATP; subProvider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="d98cf-107">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="d98cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="d98cf-108">Properties</span></span>

| <span data-ttu-id="d98cf-109">属性</span><span class="sxs-lookup"><span data-stu-id="d98cf-109">Property</span></span>   | <span data-ttu-id="d98cf-110">类型</span><span class="sxs-lookup"><span data-stu-id="d98cf-110">Type</span></span>|<span data-ttu-id="d98cf-111">说明</span><span class="sxs-lookup"><span data-stu-id="d98cf-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d98cf-112">提供程序</span><span class="sxs-lookup"><span data-stu-id="d98cf-112">provider</span></span> |<span data-ttu-id="d98cf-113">字符串</span><span class="sxs-lookup"><span data-stu-id="d98cf-113">String</span></span>|<span data-ttu-id="d98cf-114">特定提供程序 （产品/服务 — 不供应商公司）;例如，WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="d98cf-114">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="d98cf-115">providerVersion</span><span class="sxs-lookup"><span data-stu-id="d98cf-115">providerVersion</span></span>|<span data-ttu-id="d98cf-116">字符串</span><span class="sxs-lookup"><span data-stu-id="d98cf-116">String</span></span>|<span data-ttu-id="d98cf-117">提供程序或 subprovider，如果存在，生成警报的版本。</span><span class="sxs-lookup"><span data-stu-id="d98cf-117">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="d98cf-118">*Required*</span><span class="sxs-lookup"><span data-stu-id="d98cf-118">*Required*</span></span>|
|<span data-ttu-id="d98cf-119">subProvider</span><span class="sxs-lookup"><span data-stu-id="d98cf-119">subProvider</span></span>|<span data-ttu-id="d98cf-120">字符串</span><span class="sxs-lookup"><span data-stu-id="d98cf-120">String</span></span>|<span data-ttu-id="d98cf-121">特定 subprovider （下聚合提供程序）;例如，WindowsDefenderATP.SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="d98cf-121">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="d98cf-122">供应商</span><span class="sxs-lookup"><span data-stu-id="d98cf-122">vendor</span></span> |<span data-ttu-id="d98cf-123">字符串</span><span class="sxs-lookup"><span data-stu-id="d98cf-123">String</span></span>|<span data-ttu-id="d98cf-124">警报供应商 (例如，Microsoft，Dell FireEye) 的名称。</span><span class="sxs-lookup"><span data-stu-id="d98cf-124">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="d98cf-125">*Required*</span><span class="sxs-lookup"><span data-stu-id="d98cf-125">*Required*</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d98cf-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d98cf-126">JSON representation</span></span>

<span data-ttu-id="d98cf-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d98cf-127">The folllowing is a JSON representation of the resource.</span></span>
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
