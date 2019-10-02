---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1774a52b6dd5535443bb24dea5e786fc2c8cff34
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360641"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="3927d-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="3927d-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="3927d-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3927d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3927d-105">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="3927d-105">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="3927d-106">属性</span><span class="sxs-lookup"><span data-stu-id="3927d-106">Properties</span></span>
|<span data-ttu-id="3927d-107">属性</span><span class="sxs-lookup"><span data-stu-id="3927d-107">Property</span></span>|<span data-ttu-id="3927d-108">类型</span><span class="sxs-lookup"><span data-stu-id="3927d-108">Type</span></span>|<span data-ttu-id="3927d-109">说明</span><span class="sxs-lookup"><span data-stu-id="3927d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3927d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="3927d-110">displayName</span></span>|<span data-ttu-id="3927d-111">String</span><span class="sxs-lookup"><span data-stu-id="3927d-111">String</span></span>|<span data-ttu-id="3927d-112">显示名称</span><span class="sxs-lookup"><span data-stu-id="3927d-112">Display name</span></span>|
|<span data-ttu-id="3927d-113">ranges</span><span class="sxs-lookup"><span data-stu-id="3927d-113">ranges</span></span>|<span data-ttu-id="3927d-114">[ipRange](../resources/intune-mam-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3927d-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="3927d-115">Internet 协议地址范围的集合</span><span class="sxs-lookup"><span data-stu-id="3927d-115">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="3927d-116">关系</span><span class="sxs-lookup"><span data-stu-id="3927d-116">Relationships</span></span>
<span data-ttu-id="3927d-117">无</span><span class="sxs-lookup"><span data-stu-id="3927d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3927d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3927d-118">JSON Representation</span></span>
<span data-ttu-id="3927d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3927d-119">Here is a JSON representation of the resource.</span></span>
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




