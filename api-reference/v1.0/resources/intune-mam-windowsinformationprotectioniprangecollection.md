---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fb77a9a359ebd06b788470cf5948c6f4b92780c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448226"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="81685-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="81685-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="81685-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="81685-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81685-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81685-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81685-106">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="81685-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="81685-107">属性</span><span class="sxs-lookup"><span data-stu-id="81685-107">Properties</span></span>
|<span data-ttu-id="81685-108">属性</span><span class="sxs-lookup"><span data-stu-id="81685-108">Property</span></span>|<span data-ttu-id="81685-109">类型</span><span class="sxs-lookup"><span data-stu-id="81685-109">Type</span></span>|<span data-ttu-id="81685-110">说明</span><span class="sxs-lookup"><span data-stu-id="81685-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81685-111">displayName</span><span class="sxs-lookup"><span data-stu-id="81685-111">displayName</span></span>|<span data-ttu-id="81685-112">String</span><span class="sxs-lookup"><span data-stu-id="81685-112">String</span></span>|<span data-ttu-id="81685-113">显示名称</span><span class="sxs-lookup"><span data-stu-id="81685-113">Display name</span></span>|
|<span data-ttu-id="81685-114">ranges</span><span class="sxs-lookup"><span data-stu-id="81685-114">ranges</span></span>|<span data-ttu-id="81685-115">[ipRange](../resources/intune-mam-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81685-115">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="81685-116">Internet 协议地址范围的集合</span><span class="sxs-lookup"><span data-stu-id="81685-116">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="81685-117">关系</span><span class="sxs-lookup"><span data-stu-id="81685-117">Relationships</span></span>
<span data-ttu-id="81685-118">无</span><span class="sxs-lookup"><span data-stu-id="81685-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81685-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81685-119">JSON Representation</span></span>
<span data-ttu-id="81685-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81685-120">Here is a JSON representation of the resource.</span></span>
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




