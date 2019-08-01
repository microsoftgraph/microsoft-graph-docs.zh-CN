---
title: securityVendorInformation 资源类型
description: " subProvider = AppLocker)。"
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 3fb959da2d6af10632f9113a33eb942492b679ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034424"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="f7d93-103">securityVendorInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7d93-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="f7d93-104">包含有关安全产品/服务供应商、提供程序和 subprovider 的详细信息 (例如, 供应商 = Microsoft; provider = Windows Defender ATP; subProvider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="f7d93-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="f7d93-105">属性</span><span class="sxs-lookup"><span data-stu-id="f7d93-105">Properties</span></span>

| <span data-ttu-id="f7d93-106">属性</span><span class="sxs-lookup"><span data-stu-id="f7d93-106">Property</span></span>   | <span data-ttu-id="f7d93-107">类型</span><span class="sxs-lookup"><span data-stu-id="f7d93-107">Type</span></span>|<span data-ttu-id="f7d93-108">说明</span><span class="sxs-lookup"><span data-stu-id="f7d93-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7d93-109">provider</span><span class="sxs-lookup"><span data-stu-id="f7d93-109">provider</span></span> |<span data-ttu-id="f7d93-110">String</span><span class="sxs-lookup"><span data-stu-id="f7d93-110">String</span></span>|<span data-ttu-id="f7d93-111">特定提供商 (产品/服务-非供应商公司);例如, WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="f7d93-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="f7d93-112">providerVersion</span><span class="sxs-lookup"><span data-stu-id="f7d93-112">providerVersion</span></span>|<span data-ttu-id="f7d93-113">String</span><span class="sxs-lookup"><span data-stu-id="f7d93-113">String</span></span>|<span data-ttu-id="f7d93-114">提供程序或 subprovider 的版本 (如果存在), 它将生成警报。</span><span class="sxs-lookup"><span data-stu-id="f7d93-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="f7d93-115">*Required*</span><span class="sxs-lookup"><span data-stu-id="f7d93-115">*Required*</span></span>|
|<span data-ttu-id="f7d93-116">subProvider</span><span class="sxs-lookup"><span data-stu-id="f7d93-116">subProvider</span></span>|<span data-ttu-id="f7d93-117">String</span><span class="sxs-lookup"><span data-stu-id="f7d93-117">String</span></span>|<span data-ttu-id="f7d93-118">特定 subprovider (在聚合提供程序下);例如, WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="f7d93-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="f7d93-119">提供</span><span class="sxs-lookup"><span data-stu-id="f7d93-119">vendor</span></span> |<span data-ttu-id="f7d93-120">String</span><span class="sxs-lookup"><span data-stu-id="f7d93-120">String</span></span>|<span data-ttu-id="f7d93-121">通知供应商的名称 (例如, Microsoft、Dell、FireEye)。</span><span class="sxs-lookup"><span data-stu-id="f7d93-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="f7d93-122">*Required*</span><span class="sxs-lookup"><span data-stu-id="f7d93-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f7d93-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7d93-123">JSON representation</span></span>

<span data-ttu-id="f7d93-124">Folllowing 是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7d93-124">The folllowing is a JSON representation of the resource.</span></span>
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
