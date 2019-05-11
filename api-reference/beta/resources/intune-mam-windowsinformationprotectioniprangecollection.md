---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de20421b16eae22130508584b8483085d49ac9d9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940517"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="33faf-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="33faf-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="33faf-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="33faf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33faf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="33faf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33faf-106">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="33faf-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="33faf-107">属性</span><span class="sxs-lookup"><span data-stu-id="33faf-107">Properties</span></span>
|<span data-ttu-id="33faf-108">属性</span><span class="sxs-lookup"><span data-stu-id="33faf-108">Property</span></span>|<span data-ttu-id="33faf-109">类型</span><span class="sxs-lookup"><span data-stu-id="33faf-109">Type</span></span>|<span data-ttu-id="33faf-110">说明</span><span class="sxs-lookup"><span data-stu-id="33faf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33faf-111">displayName</span><span class="sxs-lookup"><span data-stu-id="33faf-111">displayName</span></span>|<span data-ttu-id="33faf-112">String</span><span class="sxs-lookup"><span data-stu-id="33faf-112">String</span></span>|<span data-ttu-id="33faf-113">显示名称</span><span class="sxs-lookup"><span data-stu-id="33faf-113">Display name</span></span>|
|<span data-ttu-id="33faf-114">ranges</span><span class="sxs-lookup"><span data-stu-id="33faf-114">ranges</span></span>|<span data-ttu-id="33faf-115">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="33faf-115">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="33faf-116">IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="33faf-116">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="33faf-117">关系</span><span class="sxs-lookup"><span data-stu-id="33faf-117">Relationships</span></span>
<span data-ttu-id="33faf-118">无</span><span class="sxs-lookup"><span data-stu-id="33faf-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33faf-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33faf-119">JSON Representation</span></span>
<span data-ttu-id="33faf-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33faf-120">Here is a JSON representation of the resource.</span></span>
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




