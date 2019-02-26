---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6a2f52613eae9d8e06751672c95230dfc3b00c4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253895"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="1d777-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d777-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="1d777-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d777-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d777-105">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="1d777-105">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="1d777-106">属性</span><span class="sxs-lookup"><span data-stu-id="1d777-106">Properties</span></span>
|<span data-ttu-id="1d777-107">属性</span><span class="sxs-lookup"><span data-stu-id="1d777-107">Property</span></span>|<span data-ttu-id="1d777-108">类型</span><span class="sxs-lookup"><span data-stu-id="1d777-108">Type</span></span>|<span data-ttu-id="1d777-109">说明</span><span class="sxs-lookup"><span data-stu-id="1d777-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d777-110">displayName</span><span class="sxs-lookup"><span data-stu-id="1d777-110">displayName</span></span>|<span data-ttu-id="1d777-111">String</span><span class="sxs-lookup"><span data-stu-id="1d777-111">String</span></span>|<span data-ttu-id="1d777-112">显示名称</span><span class="sxs-lookup"><span data-stu-id="1d777-112">Display name</span></span>|
|<span data-ttu-id="1d777-113">ranges</span><span class="sxs-lookup"><span data-stu-id="1d777-113">ranges</span></span>|<span data-ttu-id="1d777-114">[ipRange](../resources/intune-mam-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d777-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="1d777-115">Internet 协议地址范围的集合</span><span class="sxs-lookup"><span data-stu-id="1d777-115">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d777-116">关系</span><span class="sxs-lookup"><span data-stu-id="1d777-116">Relationships</span></span>
<span data-ttu-id="1d777-117">无</span><span class="sxs-lookup"><span data-stu-id="1d777-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d777-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d777-118">JSON Representation</span></span>
<span data-ttu-id="1d777-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d777-119">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.ipRange",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```



