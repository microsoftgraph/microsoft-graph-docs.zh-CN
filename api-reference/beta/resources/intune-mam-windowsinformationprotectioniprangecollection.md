---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b894318bb0b56bb2e5fc86e47a677dd9709e1092
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524249"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="99be9-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="99be9-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="99be9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="99be9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99be9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="99be9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99be9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99be9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99be9-107">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="99be9-107">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="99be9-108">属性</span><span class="sxs-lookup"><span data-stu-id="99be9-108">Properties</span></span>
|<span data-ttu-id="99be9-109">属性</span><span class="sxs-lookup"><span data-stu-id="99be9-109">Property</span></span>|<span data-ttu-id="99be9-110">类型</span><span class="sxs-lookup"><span data-stu-id="99be9-110">Type</span></span>|<span data-ttu-id="99be9-111">说明</span><span class="sxs-lookup"><span data-stu-id="99be9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99be9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="99be9-112">displayName</span></span>|<span data-ttu-id="99be9-113">String</span><span class="sxs-lookup"><span data-stu-id="99be9-113">String</span></span>|<span data-ttu-id="99be9-114">显示名称</span><span class="sxs-lookup"><span data-stu-id="99be9-114">Display name</span></span>|
|<span data-ttu-id="99be9-115">ranges</span><span class="sxs-lookup"><span data-stu-id="99be9-115">ranges</span></span>|<span data-ttu-id="99be9-116">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="99be9-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="99be9-117">IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="99be9-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="99be9-118">关系</span><span class="sxs-lookup"><span data-stu-id="99be9-118">Relationships</span></span>
<span data-ttu-id="99be9-119">无</span><span class="sxs-lookup"><span data-stu-id="99be9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99be9-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99be9-120">JSON Representation</span></span>
<span data-ttu-id="99be9-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99be9-121">Here is a JSON representation of the resource.</span></span>
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



