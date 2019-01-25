---
title: securityVendorInformation 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e67a5306b1dd08933877dbe3e64cab766ccd6a96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512176"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="ad650-104">securityVendorInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad650-104">securityVendorInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad650-105">包含有关安全产品/服务供应商、 提供商和 subprovider 详细信息 (例如，供应商 = Microsoft; 提供程序 = Windows Defender ATP; subProvider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="ad650-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="ad650-106">属性</span><span class="sxs-lookup"><span data-stu-id="ad650-106">Properties</span></span>

| <span data-ttu-id="ad650-107">属性</span><span class="sxs-lookup"><span data-stu-id="ad650-107">Property</span></span>   | <span data-ttu-id="ad650-108">类型</span><span class="sxs-lookup"><span data-stu-id="ad650-108">Type</span></span>|<span data-ttu-id="ad650-109">说明</span><span class="sxs-lookup"><span data-stu-id="ad650-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad650-110">Provider</span><span class="sxs-lookup"><span data-stu-id="ad650-110">provider</span></span> |<span data-ttu-id="ad650-111">String</span><span class="sxs-lookup"><span data-stu-id="ad650-111">String</span></span>|<span data-ttu-id="ad650-112">特定提供程序 （产品/服务 — 不供应商公司）;例如，WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="ad650-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="ad650-113">providerVersion</span><span class="sxs-lookup"><span data-stu-id="ad650-113">providerVersion</span></span>|<span data-ttu-id="ad650-114">String</span><span class="sxs-lookup"><span data-stu-id="ad650-114">String</span></span>|<span data-ttu-id="ad650-115">提供程序或 subprovider，如果存在，生成警报的版本。</span><span class="sxs-lookup"><span data-stu-id="ad650-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="ad650-116">*Required*</span><span class="sxs-lookup"><span data-stu-id="ad650-116">*Required*</span></span>|
|<span data-ttu-id="ad650-117">subProvider</span><span class="sxs-lookup"><span data-stu-id="ad650-117">subProvider</span></span>|<span data-ttu-id="ad650-118">String</span><span class="sxs-lookup"><span data-stu-id="ad650-118">String</span></span>|<span data-ttu-id="ad650-119">特定 subprovider （下聚合提供程序）;例如，WindowsDefenderATP.SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="ad650-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="ad650-120">供应商</span><span class="sxs-lookup"><span data-stu-id="ad650-120">vendor</span></span> |<span data-ttu-id="ad650-121">String</span><span class="sxs-lookup"><span data-stu-id="ad650-121">String</span></span>|<span data-ttu-id="ad650-122">警报供应商 (例如，Microsoft，Dell FireEye) 的名称。</span><span class="sxs-lookup"><span data-stu-id="ad650-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="ad650-123">*Required*</span><span class="sxs-lookup"><span data-stu-id="ad650-123">*Required*</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad650-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad650-124">JSON representation</span></span>

<span data-ttu-id="ad650-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad650-125">The folllowing is a JSON representation of the resource.</span></span>
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
