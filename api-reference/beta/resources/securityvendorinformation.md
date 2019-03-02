---
title: securityVendorInformation 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 7f48c27ba94d8419ce244143a48cf6ab04dd080e
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30364582"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="2b58b-104">securityVendorInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b58b-104">securityVendorInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b58b-105">包含有关安全产品/服务供应商、提供程序和 subprovider 的详细信息 (例如, 供应商 = Microsoft; provider = Windows Defender ATP; subprovider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="2b58b-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="2b58b-106">属性</span><span class="sxs-lookup"><span data-stu-id="2b58b-106">Properties</span></span>

| <span data-ttu-id="2b58b-107">属性</span><span class="sxs-lookup"><span data-stu-id="2b58b-107">Property</span></span>   | <span data-ttu-id="2b58b-108">类型</span><span class="sxs-lookup"><span data-stu-id="2b58b-108">Type</span></span>|<span data-ttu-id="2b58b-109">说明</span><span class="sxs-lookup"><span data-stu-id="2b58b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b58b-110">provider</span><span class="sxs-lookup"><span data-stu-id="2b58b-110">provider</span></span> |<span data-ttu-id="2b58b-111">String</span><span class="sxs-lookup"><span data-stu-id="2b58b-111">String</span></span>|<span data-ttu-id="2b58b-112">特定提供商 (产品/服务-非供应商公司);例如, WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="2b58b-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="2b58b-113">providerVersion</span><span class="sxs-lookup"><span data-stu-id="2b58b-113">providerVersion</span></span>|<span data-ttu-id="2b58b-114">String</span><span class="sxs-lookup"><span data-stu-id="2b58b-114">String</span></span>|<span data-ttu-id="2b58b-115">提供程序或 subprovider 的版本 (如果存在), 它将生成警报。</span><span class="sxs-lookup"><span data-stu-id="2b58b-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="2b58b-116">**Required**</span><span class="sxs-lookup"><span data-stu-id="2b58b-116">**Required**</span></span>|
|<span data-ttu-id="2b58b-117">subProvider</span><span class="sxs-lookup"><span data-stu-id="2b58b-117">subProvider</span></span>|<span data-ttu-id="2b58b-118">String</span><span class="sxs-lookup"><span data-stu-id="2b58b-118">String</span></span>|<span data-ttu-id="2b58b-119">特定 subprovider (在聚合提供程序下);例如, WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="2b58b-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="2b58b-120">提供</span><span class="sxs-lookup"><span data-stu-id="2b58b-120">vendor</span></span> |<span data-ttu-id="2b58b-121">String</span><span class="sxs-lookup"><span data-stu-id="2b58b-121">String</span></span>|<span data-ttu-id="2b58b-122">通知供应商的名称 (例如, Microsoft、Dell、FireEye)。</span><span class="sxs-lookup"><span data-stu-id="2b58b-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="2b58b-123">**Required**</span><span class="sxs-lookup"><span data-stu-id="2b58b-123">**Required**</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b58b-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b58b-124">JSON representation</span></span>

<span data-ttu-id="2b58b-125">folllowing 是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b58b-125">The folllowing is a JSON representation of the resource.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/resources/securityvendorinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
