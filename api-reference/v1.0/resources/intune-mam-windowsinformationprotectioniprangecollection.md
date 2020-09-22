---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b243f8923ac44b516a93608fd5c7d82c9cb1296f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074893"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="f3e61-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3e61-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="f3e61-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3e61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3e61-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3e61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3e61-106">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="f3e61-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="f3e61-107">属性</span><span class="sxs-lookup"><span data-stu-id="f3e61-107">Properties</span></span>
|<span data-ttu-id="f3e61-108">属性</span><span class="sxs-lookup"><span data-stu-id="f3e61-108">Property</span></span>|<span data-ttu-id="f3e61-109">类型</span><span class="sxs-lookup"><span data-stu-id="f3e61-109">Type</span></span>|<span data-ttu-id="f3e61-110">说明</span><span class="sxs-lookup"><span data-stu-id="f3e61-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3e61-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f3e61-111">displayName</span></span>|<span data-ttu-id="f3e61-112">String</span><span class="sxs-lookup"><span data-stu-id="f3e61-112">String</span></span>|<span data-ttu-id="f3e61-113">显示名称</span><span class="sxs-lookup"><span data-stu-id="f3e61-113">Display name</span></span>|
|<span data-ttu-id="f3e61-114">ranges</span><span class="sxs-lookup"><span data-stu-id="f3e61-114">ranges</span></span>|<span data-ttu-id="f3e61-115">[ipRange](../resources/intune-mam-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f3e61-115">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="f3e61-116">Internet 协议地址范围的集合</span><span class="sxs-lookup"><span data-stu-id="f3e61-116">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3e61-117">关系</span><span class="sxs-lookup"><span data-stu-id="f3e61-117">Relationships</span></span>
<span data-ttu-id="f3e61-118">无</span><span class="sxs-lookup"><span data-stu-id="f3e61-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3e61-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3e61-119">JSON Representation</span></span>
<span data-ttu-id="f3e61-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3e61-120">Here is a JSON representation of the resource.</span></span>
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









