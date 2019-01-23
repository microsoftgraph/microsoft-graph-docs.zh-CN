---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e844c2da60babdcad5fad4a522a750bb2f013721
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418783"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="27927-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="27927-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="27927-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="27927-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="27927-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="27927-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27927-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27927-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27927-107">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="27927-107">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="27927-108">属性</span><span class="sxs-lookup"><span data-stu-id="27927-108">Properties</span></span>
|<span data-ttu-id="27927-109">属性</span><span class="sxs-lookup"><span data-stu-id="27927-109">Property</span></span>|<span data-ttu-id="27927-110">类型</span><span class="sxs-lookup"><span data-stu-id="27927-110">Type</span></span>|<span data-ttu-id="27927-111">说明</span><span class="sxs-lookup"><span data-stu-id="27927-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27927-112">displayName</span><span class="sxs-lookup"><span data-stu-id="27927-112">displayName</span></span>|<span data-ttu-id="27927-113">String</span><span class="sxs-lookup"><span data-stu-id="27927-113">String</span></span>|<span data-ttu-id="27927-114">显示名称</span><span class="sxs-lookup"><span data-stu-id="27927-114">Display name</span></span>|
|<span data-ttu-id="27927-115">ranges</span><span class="sxs-lookup"><span data-stu-id="27927-115">ranges</span></span>|<span data-ttu-id="27927-116">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="27927-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="27927-117">IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="27927-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="27927-118">关系</span><span class="sxs-lookup"><span data-stu-id="27927-118">Relationships</span></span>
<span data-ttu-id="27927-119">无</span><span class="sxs-lookup"><span data-stu-id="27927-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27927-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27927-120">JSON Representation</span></span>
<span data-ttu-id="27927-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27927-121">Here is a JSON representation of the resource.</span></span>
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




