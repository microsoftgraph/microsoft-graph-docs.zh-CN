---
title: securityVendorInformation 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: f0c0142333237c1c4700353b01f75b9867b85ad7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988826"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="bfbdd-104">securityVendorInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="bfbdd-104">securityVendorInformation resource type</span></span>

<span data-ttu-id="bfbdd-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfbdd-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfbdd-106">包含有关安全产品/服务供应商、提供商和 subprovider 的详细信息 (例如，供应商 = Microsoft;提供程序 = Windows Defender ATP;subProvider = AppLocker) 。</span><span class="sxs-lookup"><span data-stu-id="bfbdd-106">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="bfbdd-107">属性</span><span class="sxs-lookup"><span data-stu-id="bfbdd-107">Properties</span></span>

| <span data-ttu-id="bfbdd-108">属性</span><span class="sxs-lookup"><span data-stu-id="bfbdd-108">Property</span></span>   | <span data-ttu-id="bfbdd-109">类型</span><span class="sxs-lookup"><span data-stu-id="bfbdd-109">Type</span></span>|<span data-ttu-id="bfbdd-110">说明</span><span class="sxs-lookup"><span data-stu-id="bfbdd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfbdd-111">provider</span><span class="sxs-lookup"><span data-stu-id="bfbdd-111">provider</span></span> |<span data-ttu-id="bfbdd-112">String</span><span class="sxs-lookup"><span data-stu-id="bfbdd-112">String</span></span>|<span data-ttu-id="bfbdd-113">特定提供商 (产品/服务-不提供供应商公司) ;例如，WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="bfbdd-113">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="bfbdd-114">providerVersion</span><span class="sxs-lookup"><span data-stu-id="bfbdd-114">providerVersion</span></span>|<span data-ttu-id="bfbdd-115">String</span><span class="sxs-lookup"><span data-stu-id="bfbdd-115">String</span></span>|<span data-ttu-id="bfbdd-116">提供程序或 subprovider 的版本（如果存在），它将生成警报。</span><span class="sxs-lookup"><span data-stu-id="bfbdd-116">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="bfbdd-117">**Required**</span><span class="sxs-lookup"><span data-stu-id="bfbdd-117">**Required**</span></span>|
|<span data-ttu-id="bfbdd-118">subProvider</span><span class="sxs-lookup"><span data-stu-id="bfbdd-118">subProvider</span></span>|<span data-ttu-id="bfbdd-119">String</span><span class="sxs-lookup"><span data-stu-id="bfbdd-119">String</span></span>|<span data-ttu-id="bfbdd-120">聚合提供程序) 下的特定 subprovider (;例如，WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="bfbdd-120">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="bfbdd-121">提供</span><span class="sxs-lookup"><span data-stu-id="bfbdd-121">vendor</span></span> |<span data-ttu-id="bfbdd-122">String</span><span class="sxs-lookup"><span data-stu-id="bfbdd-122">String</span></span>|<span data-ttu-id="bfbdd-123">通知供应商的名称 (例如，Microsoft、Dell、FireEye) 。</span><span class="sxs-lookup"><span data-stu-id="bfbdd-123">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="bfbdd-124">**Required**</span><span class="sxs-lookup"><span data-stu-id="bfbdd-124">**Required**</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bfbdd-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bfbdd-125">JSON representation</span></span>

<span data-ttu-id="bfbdd-126">Folllowing 是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfbdd-126">The folllowing is a JSON representation of the resource.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


