---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d6246cfc80e2ecb9d71ce45e333e09bf35521af
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994452"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="e3398-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3398-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="e3398-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e3398-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3398-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e3398-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3398-106">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="e3398-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="e3398-107">属性</span><span class="sxs-lookup"><span data-stu-id="e3398-107">Properties</span></span>
|<span data-ttu-id="e3398-108">属性</span><span class="sxs-lookup"><span data-stu-id="e3398-108">Property</span></span>|<span data-ttu-id="e3398-109">类型</span><span class="sxs-lookup"><span data-stu-id="e3398-109">Type</span></span>|<span data-ttu-id="e3398-110">说明</span><span class="sxs-lookup"><span data-stu-id="e3398-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3398-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e3398-111">displayName</span></span>|<span data-ttu-id="e3398-112">String</span><span class="sxs-lookup"><span data-stu-id="e3398-112">String</span></span>|<span data-ttu-id="e3398-113">显示名称</span><span class="sxs-lookup"><span data-stu-id="e3398-113">Display name</span></span>|
|<span data-ttu-id="e3398-114">ranges</span><span class="sxs-lookup"><span data-stu-id="e3398-114">ranges</span></span>|<span data-ttu-id="e3398-115">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3398-115">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="e3398-116">IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="e3398-116">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3398-117">关系</span><span class="sxs-lookup"><span data-stu-id="e3398-117">Relationships</span></span>
<span data-ttu-id="e3398-118">无</span><span class="sxs-lookup"><span data-stu-id="e3398-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3398-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3398-119">JSON Representation</span></span>
<span data-ttu-id="e3398-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3398-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```





