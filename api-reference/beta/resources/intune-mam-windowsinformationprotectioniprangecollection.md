---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a972ddf469723acd91e6b122cfef103ab08e24f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785690"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="b240a-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="b240a-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="b240a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b240a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b240a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b240a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b240a-106">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="b240a-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="b240a-107">属性</span><span class="sxs-lookup"><span data-stu-id="b240a-107">Properties</span></span>
|<span data-ttu-id="b240a-108">属性</span><span class="sxs-lookup"><span data-stu-id="b240a-108">Property</span></span>|<span data-ttu-id="b240a-109">类型</span><span class="sxs-lookup"><span data-stu-id="b240a-109">Type</span></span>|<span data-ttu-id="b240a-110">说明</span><span class="sxs-lookup"><span data-stu-id="b240a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b240a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b240a-111">displayName</span></span>|<span data-ttu-id="b240a-112">String</span><span class="sxs-lookup"><span data-stu-id="b240a-112">String</span></span>|<span data-ttu-id="b240a-113">显示名称</span><span class="sxs-lookup"><span data-stu-id="b240a-113">Display name</span></span>|
|<span data-ttu-id="b240a-114">ranges</span><span class="sxs-lookup"><span data-stu-id="b240a-114">ranges</span></span>|<span data-ttu-id="b240a-115">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b240a-115">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="b240a-116">IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="b240a-116">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="b240a-117">关系</span><span class="sxs-lookup"><span data-stu-id="b240a-117">Relationships</span></span>
<span data-ttu-id="b240a-118">无</span><span class="sxs-lookup"><span data-stu-id="b240a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b240a-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b240a-119">JSON Representation</span></span>
<span data-ttu-id="b240a-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b240a-120">Here is a JSON representation of the resource.</span></span>
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





